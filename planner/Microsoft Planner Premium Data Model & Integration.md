---
date: 2025-03-23
source: claude
---
# Microsoft Planner Premium Data Model & Integration

## Overview

This guide provides a comprehensive overview of Microsoft Planner Premium (formerly Project for the Web), focusing on its underlying data model in Dataverse and integration options for custom development and reporting.
## Table of Contents

1. [Storage & Architecture](#storage--architecture)
2. [Core Data Model](#core-data-model)
3. [Detailed Entity Reference](#detailed-entity-reference)
4. [Permission Model](#permission-model)
5. [Integration Options](#integration-options)
6. [Working with Unnamed Resources](#working-with-unnamed-resources)
7. [Custom Development Approach](#custom-development-approach)
8. [Sample Mock Data](#sample-mock-data)
## Storage & Architecture

Microsoft Planner Premium schedules are stored in **Microsoft Dataverse** (formerly Common Data Service). This cloud-based storage solution powers many Power Platform applications and provides a structured, relational data model.

Key points about the storage architecture:
- All schedules exist in the same [[Dataverse]] environment within your organization
- Access is controlled through a permission-based security model
- The data can be accessed via the UI, Power Platform tools, or direct API calls
- [[Power Apps]] and [[Power Automate]] can interact with the data via [[Dataverse Connectors]]
## Core Data Model

The [[Microsoft Planner Premium]] data model follows a hierarchical structure:

```
Project
├── Tasks
│   ├── Subtasks
│   └── Dependencies
├── Resources
├── Assignments
└── Project Team
```

Primary entities and their relationships:

- **Project**: The main container for all project data
- **Task**: Individual work items that make up the project
- **Dependency**: Links between tasks that create scheduling relationships
- **Resource**: People or generic resources that can be assigned to tasks
- **Assignment**: The connection between a task and a resource
- **Team Member**: Resources specifically associated with the project
- 
## Detailed Entity Reference

### Project Entity (`msdyn_project`)

- **`msdyn_projectid`**
    - Data Type: `Uniqueidentifier`
    - Description: Primary key
    - Valid Values/Range: System-generated UUID
    - Notes: Auto-generated
- **`msdyn_subject`**
    - Data Type: `String` (500)
    - Description: Project name
    - Valid Values/Range: Any text, max 500 chars
    - Notes: Required field
- **`msdyn_scheduledstart`**
    - Data Type: `DateTime`
    - Description: Project start date
    - Valid Values/Range: Valid date/time
    - Notes: Default to creation date
- **`msdyn_scheduledend`**
    - Data Type: `DateTime`
    - Description: Project end date
    - Valid Values/Range: Valid date/time, must be ≥ start date
    - Notes: Calculated based on tasks
- **`msdyn_effortestimateintotalminutesformula`**
    - Data Type: `Decimal`
    - Description: Total effort
    - Valid Values/Range: ≥ `0`
    - Notes: Calculated from tasks
- **`statecode`**
    - Data Type: `Integer`
    - Description: Activity state
    - Valid Values/Range: `0` = Active, `1` = Inactive
    - Notes: Controls visibility
- **`ownerid`**
    - Data Type: `Lookup`
    - Description: Project owner
    - Valid Values/Range: Valid user or team ID
    - Notes: Security context
- **`msdyn_calendarid`**
    - Data Type: `Lookup`
    - Description: Project calendar
    - Valid Values/Range: Reference to calendar entity
    - Notes: Controls working time
- **`msdyn_projectmanager`**
    - Data Type: `Lookup`
    - Description: Project manager
    - Valid Values/Range: Valid user ID
    - Notes: Optional
- **`msdyn_description`**
    - Data Type: Memo
    - Description: Project description
    - Valid Values/Range: Any text
    - Notes: Optional
- **`msdyn_progress`**
    - Data Type: `Decimal`
    - Description: % complete
    - Valid Values/Range:` 0.0` to `100.0`
    - Notes: Calculated from tasks
- **`msdyn_schedulemode`**
    - Data Type: `OptionSet`
    - Description: Scheduling method
    - Valid Values/Range: `0` = Manual, `1` = Automatic
    - Notes: Controls scheduling engine

### Task Entity (`msdyn_projecttask`)

- **`msdyn_projecttaskid`**
    - Data Type: `Uniqueidentifier`
    - Description: Primary key
    - Valid Values/Range: System-generated UUID
    - Notes: Auto-generated
- **`msdyn_subject`**
    - Data Type: `String (500)`
    - Description: Task name
    - Valid Values/Range: Any text, max 500 chars
    - Notes: Required field
- **`msdyn_projectid`**
    - Data Type: `Lookup`
    - Description: Parent project
    - Valid Values/Range: Valid project ID
    - Notes: Required relationship
- **`msdyn_effort`**
    - Data Type: `Integer`
    - Description: Work estimate
    - Valid Values/Range: ≥ `0` (minutes)
    - Notes: Editable in UI as hours
- **`msdyn_progress`**
    - Data Type: `Decimal`
    - Description: % complete
    - Valid Values/Range:` 0.0` to `100.0`
    - Notes: Manual or calculated
- **`msdyn_scheduledstart`**
    - Data Type: `DateTime`
    - Description: Start time
    - Valid Values/Range: Valid date/time
    - Notes: Updated by scheduler
- **`msdyn_scheduledend`**
    - Data Type: `DateTime`
    - Description: End time
    - Valid Values/Range: Valid date/time, must be ≥ start
    - Notes: Updated by scheduler
- **`msdyn_priority`**
    - Data Type: `Integer`
    - Description: Priority level
    - Valid Values/Range: `0` = Low, `1` = Normal, `2` = High
    - Notes: Default = 1
- **`msdyn_parenttask`**
    - Data Type: `Lookup`
    - Description: Parent task
    - Valid Values/Range: Valid task ID
    - Notes: For subtasks
- **`msdyn_outline`**
    - Data Type: `String (100)`
    - Description: WBS value
    - Valid Values/Range: Numeric hierarchical notation
    - Notes: Auto-generated (`1`,` 1.1`, `1.1.1`)
- **`msdyn_wbsduration`**
    - Data Type: `Integer`
    - Description: Duration
    - Valid Values/Range: ≥ 0 (minutes)
    - Notes: Used in scheduling
- **`msdyn_taskmode`**
    - Data Type: `OptionSet`
    - Description: Task type
    - Valid Values/Range: `0` = Fixed Units, `1` = Fixed Duration
    - Notes: Controls scheduling behavior
- **`msdyn_iscritical`**
    - Data Type: `Boolean`
    - Description: On critical path
    - Valid Values/Range: `true`/`false`
    - Notes: Calculated by engine
- **`msdyn_milestone`**
    - Data Type: `Boolean`
    - Description: Is milestone
    - Valid Values/Range: true/false
    - Notes: Special task type
- **`msdyn_bucketid`**
    - Data Type: `Lookup`
    - Description: Bucket/category
    - Valid Values/Range: Valid bucket ID
    - Notes: Optional grouping
- **`msdyn_constrainttype`**
    - Data Type: `OptionSet`
    - Description: Schedule constraint
    - Valid Values/Range: `0` = ASAP, `1` = ALAP, `2` = Must Start On, etc.
    - Notes: Controls scheduling flexibility
- **`msdyn_constraintdate`**
    - Data Type: `DateTime`
    - Description: Constraint date
    - Valid Values/Range: Valid date/time
    - Notes: Used with constraints

### Task Dependency (msdyn_projecttaskdependency)

- **`msdyn_projecttaskdependencyid`**
	- Data Type: `Uniqueidentifier`
	- Description: Primary key
	- Valid Values/Range: System-generated UUID
	- Notes: Auto-generated
- **`msdyn_predecessortask`**
    - Data Type: `Lookup`
    - Description: Predecessor task
    - Valid Values/Range: Valid task ID
    - Notes: Required relationship
- **`msdyn_successortask`**
    - Data Type: `Lookup`
    - Description: Successor task
    - Valid Values/Range: Valid task ID
    - Notes: Required relationship
- **`msdyn_linktype`**
    - Data Type: `OptionSet`
    - Description: Dependency type
    - Valid Values/Range: `0` = Finish-to-Start, `1` = Start-to-Start, `2` = Finish-to-Finish, `3` = Start-to-Finish
    - Notes: Default = `0` (FS)
- **`msdyn_offset`**
    - Data Type: `Integer`
    - Description: Lead/lag time
    - Valid Values/Range: Any integer (minutes)
    - Notes: Positive = lag, Negative = lead

### Resource Assignment (msdyn_resourceassignment)

- **`msdyn_resourceassignmentid`**
	- Data Type: `Uniqueidentifier`
	- Description: Primary key
	- Valid Values/Range: System-generated UUID
	- Notes: Auto-generated
- **`msdyn_projecttaskid`**
    - Data Type: `Lookup`
    - Description: Task reference
    - Valid Values/Range: Valid task ID
    - Notes: Required relationship
- **`msdyn_resourceid`**
    - Data Type: `Lookup`
    - Description: Resource reference
    - Valid Values/Range: Valid resource ID
    - Notes: Required relationship
- **`msdyn_assignmentpercentage`**
    - Data Type: `Decimal`
    - Description: Allocation %
    - Valid Values/Range: `0.0` to `100.0`
    - Notes: Default = `100%`
- **`msdyn_assignedwork`**
    - Data Type: `Decimal`
    - Description: Work amount
    - Valid Values/Range: ≥ `0` (minutes)
    - Notes: Calculated from task
- **`msdyn_remainingwork`**
    - Data Type: `Decimal`
    - Description: Remaining work
    - Valid Values/Range: ≥ 0 (minutes)
    - Notes: Updated during progress
- **`msdyn_actualwork`**
    - Data Type: `Decimal`
    - Description: Completed work
    - Valid Values/Range: ≥ `0` (minutes)
    - Notes: From time entries
- **`msdyn_assignmentstart`**
    - Data Type: `DateTime`
    - Description: Assignment start
    - Valid Values/Range: Valid date/time
    - Notes: Can differ from task start
- **`msdyn_assignmentend`**
    - Data Type: `DateTime`
    - Description: Assignment end
    - Valid Values/Range: Valid date/time
    - Notes: Can differ from task end

### Project Share (msdyn_projectshare)

- **`msdyn_projectshareid`**
	- Data Type: `Uniqueidentifier`
	- Description: Primary key
	- Valid Values/Range: System-generated UUID
	- Notes: Auto-generated
- **`msdyn_projectid`**
    - Data Type: `Lookup`
    - Description: Project reference
    - Valid Values/Range: Valid project ID
    - Notes: Required relationship
- **`msdyn_sharedwith`**
    - Data Type: `Lookup`
    - Description: User reference
    - Valid Values/Range: Valid user/team ID
    - Notes: Required relationship
- **`msdyn_accessrights`**
    - Data Type: `OptionSet`
    - Description: Permission level
    - Valid Values/Range: `0` = Viewer, `1` = Member, `2` = Owner
    - Notes: Controls access level
- **`statecode`**
    - Data Type: `Integer`
    - Description: Status
    - Valid Values/Range: `0` = Active, `1` = Inactive
    - Notes: Controls if sharing is active

### Project Bucket (msdyn_projectbucket)

- **`msdyn_projectbucketid`**
	- Data Type: `Uniqueidentifier`
	- Description: Primary key
	- Valid Values/Range: System-generated UUID
	- Notes: Auto-generated
- **`msdyn_name`**
    - Data Type: `String (100)`
    - Description: Bucket name
    - Valid Values/Range: Any text, max 100 chars
    - Notes: Required field
- **`msdyn_projectid`**
    - Data Type: `Lookup`
    - Description: Parent project
    - Valid Values/Range: Valid project ID
    - Notes: Required relationship
- **`msdyn_description`**
    - Data Type: `Memo`
    - Description: Description
    - Valid Values/Range: Any text
    - Notes: Optional
- **`msdyn_ordernum`**
    - Data Type: `Integer`
    - Description: Display order
    - Valid Values/Range: Any integer
    - Notes: For UI sorting

## Permission Model

Permission sharing in [[Microsoft Planner Premium]] works at multiple levels:

### Schedule-Level Permissions

Direct schedule sharing from the UI allows adding users/groups with specific permission levels:

- **`Owner`**: Full control (edit, share, delete)
- **`Member`**: Can edit but not share or delete
- **`Viewer`**: Read-only access

### Dataverse Security Model

Underlying the UI, Planner Premium uses Dataverse's security model:

1. **Security roles**:
   - Predefined roles like "`Project Owner`," "`Project Member`," "`Project Viewer`"
   - Each role has different permissions for Dataverse project entities
   - Administrators can customize these roles or create new ones
1. **Row-level security**:
   - Controls access to specific project records
   - Can limit users to only see their own projects or specific projects

3. **Field-level security**:
   - Controls access to specific fields within project entities
   - Can hide sensitive information from certain users
### Service Principal Access

For Power Apps and Power Automate integration:

1. **Connection References**:
   - Power Apps and Power Automate use "`Connection References`"
   - These can leverage service principals for application-to-application authentication

2. **Application Users**:
   - Special non-interactive user accounts in Dataverse
   - Created specifically for application-to-application authentication
   - Assigned security roles that determine what data they can access

## Integration Options

Multiple options exist for integrating with Planner Premium data:

### 1. Direct Table Access

- Connect directly to Dataverse tables via Power Apps/Power Automate
- Provides complete flexibility but requires understanding of the data model
- Microsoft officially supports this approach
- Can be used for both reading and writing data

### 2. Project API

- Microsoft provides a dedicated Project API
- Handles the underlying complexity and maintains data integrity
- Available endpoints include:
  - `/projects` - Create and manage projects
  - `/projects/{id}/tasks` - Manage tasks within projects  
  - `/projects/{id}/sharing` - Manage project sharing

### 3. Power Platform Connectors

- Use official Microsoft Project connector for Power Automate/Power Apps
- Provides a safer abstraction over the direct data model

### 4. Hybrid approach

- Use APIs for core project creation and structure
- Use direct table access for supplemental data not covered by APIs

## Working with Unnamed Resources

Planner Premium supports generic (unnamed) resources in its data model, though this isn't prominently featured in the UI.

### Implementation in Data Model

- Uses the **`bookableresource`** entity with special configuration
- Has a **`resourcetype`** field set to indicate a generic resource
- Can have a name like "`Developer`" or "`Designer`" instead of a person's name

### Usage in the UI

Once created in [[Dataverse]]:

- Generic resources appear in resource selection dropdowns
- Display using whatever "name" value was provided
- Can be assigned to tasks just like regular resources
- No special icon differentiates them from named resources

### Creation Process

Since the UI doesn't support direct creation of generic resources:

1. Create them via direct Dataverse access or API
2. Use Power Apps or Power Automate for a more user-friendly creation process
3. Once created, they become available for selection in the standard UI

## Custom Development Approach

For teams looking to extend Planner Premium with custom functionality:

### Power Apps Development

1. **Canvas Apps**:
   
   - Build custom interfaces for project creation and management
   - Implement advanced resource management not available in standard UI
   - Create specialized views for different stakeholder groups

2. **Model-driven Apps**:

   - Leverage the Dataverse schema more directly
   - Create forms and views tailored to your business processes
   - Extend with custom business logic

### Power Automate Integration

1. **Automation opportunities**:

   - Automate schedule creation based on templates
   - Implement advanced resource allocation logic
   - Create notification workflows for status changes
   - Integrate with other business systems

2. **Security considerations**:
   - Flows run with the permissions of their connection
   - Consider using application users with appropriate security roles
- 
### Developer Sandbox Approach

For learning and experimentation:

1. Use an isolated developer environment
2. Create mock data that mimics the Planner Premium data model
3. Experiment with the schema before implementing in production
4. Test custom applications without security review overhead

## Sample Mock Data

Below is sample mock data for testing in a developer sandbox:

### Project Structure
```json
{
  "msdyn_project": [
    {
      "msdyn_projectid": "f8a7d42e-1c3b-4a9d-8e5f-12b3c4d5e6f7",
      "msdyn_subject": "Website Redesign",
      "msdyn_scheduledstart": "2025-04-15T08:00:00Z",
      "msdyn_scheduledend": "2025-06-30T17:00:00Z",
      "statecode": 0
    }
  ]
}
```

### Tasks and Hierarchy
```json
{
  "msdyn_projecttask": [
    {
      "msdyn_projecttaskid": "a1b2c3d4-e5f6-4a3b-8c7d-9e0f1a2b3c4d",
      "msdyn_subject": "Requirements Gathering",
      "msdyn_projectid": "f8a7d42e-1c3b-4a9d-8e5f-12b3c4d5e6f7",
      "msdyn_outline": "1",
      "msdyn_effort": 2400,
      "msdyn_scheduledstart": "2025-04-15T08:00:00Z",
      "msdyn_scheduledend": "2025-04-20T17:00:00Z"
    },
    {
      "msdyn_projecttaskid": "b2c3d4e5-f6a7-5b4c-9d8e-0f1a2b3c4d5e",
      "msdyn_subject": "User Interviews",
      "msdyn_projectid": "f8a7d42e-1c3b-4a9d-8e5f-12b3c4d5e6f7",
      "msdyn_parenttask": "a1b2c3d4-e5f6-4a3b-8c7d-9e0f1a2b3c4d",
      "msdyn_outline": "1.1",
      "msdyn_effort": 1200
    }
  ]
}
```

### Dependencies
```json
{
  "msdyn_projecttaskdependency": [
    {
      "msdyn_projecttaskdependencyid": "c3d4e5f6-7a8b-6c5d-0e9f-1a2b3c4d5e6f",
      "msdyn_predecessortask": "a1b2c3d4-e5f6-4a3b-8c7d-9e0f1a2b3c4d",
      "msdyn_successortask": "b2c3d4e5-f6a7-5b4c-9d8e-0f1a2b3c4d5e",
      "msdyn_linktype": 0
    }
  ]
}
```

### Resources and Assignments
```json
{
  "bookableresource": [
    {
      "bookableresourceid": "d4e5f6a7-8b9c-7d6e-1f0a-2b3c4d5e6f7a",
      "name": "UX Designer (Generic)"
    }
  ],
  "msdyn_resourceassignment": [
    {
      "msdyn_resourceassignmentid": "e5f6a7b8-9c0d-8e7f-2a1b-3c4d5e6f7a8b",
      "msdyn_projecttaskid": "b2c3d4e5-f6a7-5b4c-9d8e-0f1a2b3c4d5e",
      "msdyn_resourceid": "d4e5f6a7-8b9c-7d6e-1f0a-2b3c4d5e6f7a"
    }
  ]
}
```
## Additional Resources

- [Microsoft Planner Premium Documentation](https://learn.microsoft.com/en-us/project-for-the-web/)
- [Dataverse Documentation](https://learn.microsoft.com/en-us/power-apps/maker/data-platform/)
- [Power Platform Integration Guide](https://learn.microsoft.com/en-us/power-platform/admin/wp-integration)

