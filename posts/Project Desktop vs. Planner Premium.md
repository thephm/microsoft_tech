---
tags:
  - post
url: 
date: 2025-03-16
people: otto
service: ghost
---
# Project Desktop vs. Planner Premium

As part of the rollout of Microsoft Planner Premium, I need to be able to explain the differences to the users.
### Some Background

Microsoft **Project** has been **developed over 40 years** so it has tons of functionality. Version 1.0 which is a Windows desktop application launched in **1984** and has had 31 versions since then. Yes, thirty one versions! A great summary of the history of this tool by Allan Rocha can be found at [Microsoft Project Names and Logos History](https://www.linkedin.com/pulse/microsoft-project-names-logos-history-allan-rocha-e1m7c/). 

Microsoft **Planner** launched in **2016** and built for teams, part of Microsoft 365 work or school subscription. It is not in Office 365 i.e., not for personal use. There are Web, Android, and iOS apps unlike Project Desktop. It was announced at [Ignite 2019](https://lnkd.in/eaJS77JZ) that Planner is now part of the "Microsoft task ecosystem". In the Spring of 2024, the new Planner app in Teams became generally available and "Tasks by Planner" and the [To Do](https://to-do.office.com/) app in Teams were renamed to "Planner".  This app is now called **Planner Basic**.

Project for the web launched in **2019** and was later renamed to "Microsoft Project for the web". It was developed from-scratch as a Web-based project scheduling tool. It was renamed to Microsoft **Planner Premium** in 2014. It was also referred to as "Project Power App" and more recently "New Planner" and was designed to work with Microsoft Teams and Microsoft Dynamics 365. Microsoft is actively working on bringing Project online and Project desktop features to this new product. 

Confused? No kidding, so was I. I have to explain this to people almost daily. 
## Summary of differences

For simplicity I refer to Project Professional or Project Standard as **Project** and to Planner Basic as **Planner**. Where there are differences between **Planner Basic** and **Planner Premium**, I will be explicit in the product names.
## What will Sr. Project Managers miss?

Senior Project Managers will have years of experience using Project and they especially will feel that Planner Premium lacks advanced project management features. My aim is to encourage adoption by identifying the gaps that they’ll miss most to avoid surprises and, at the same time, show them how to bridge those gaps.

The following sections list the features that Senior PMs will likely miss, and where possible, how to mitigate.
### Complex Task Scheduling and Constraints

What they’ll miss

- Project Professional allows defining:
	- Complex dependencies with lead/lag times
	- Task constraints e.g., “Start No Earlier Than”
	- Manually controlled scheduling
	~~- Critical path analysis -- this exists in Planner Premium -- dig into the differences~~

- How to Mitigate:
	- Use predecessors and successors in Planner Premium 
	- Define milestones manually – create key milestones and label them as checkpoints
### Resource Leveling and Capacity Planning

What They’ll Miss:

- Project Professional provides:
	- Automatic resource leveling (to resolve overbooking).
	- Workload balancing across multiple projects
- How to Mitigate:
	- Use People View in Planner Premium – This view shows task assignments and allows rebalancing workload manually
	- Connect Planner to Microsoft Power BI – Build custom reports to visualize overbooking and redistribute resources more effectively
	- Introduce Project for the Web (if needed) – If advanced resource balancing is critical, Project for the Web integrates with Planner
### Cost and Financial Tracking

What They’ll Miss:

- Project Professional supports:
	- Detailed cost tracking for labor and materials
	- Earned value analysis (EVA)
	- Baseline cost comparisons
- How to Mitigate:
	- Track costs in Power BI – Set up a Power BI dashboard to track project costs using task metadata and resource data from Planner
	- Use Excel for detailed costing – Link Planner tasks to an Excel file for more detailed cost analysis
	- Use Microsoft Lists for financial data – Create a List for budgeting and cost tracking alongside Planner.
### Recurring Tasks and Task Automation

What They’ll Miss:

- Project Professional allows setting up complex recurring tasks (e.g., every Monday, last day of the month).
- How to Mitigate:
	- Set up Power Automate triggers – Automate task creation based on a recurring schedule.
	- Use task templates – Create task templates in Planner to quickly recreate recurring tasks.
### Critical Path and Slack Time Analysis

What They’ll Miss:

- Project Professional allows highlighting the critical path and analyzing slack time.
- How to Mitigate:
	- Use Planner’s dependency view – While not as detailed, the Timeline view in Planner Premium shows task sequences and blockers
	- Set up Power BI reports – Use Power BI to analyze task completion timelines and dependency bottlenecks.
### Baseline Comparisons and Versioning

What They’ll Miss:

- Project Professional allows setting project baselines and comparing actual progress against them.

- How to Mitigate:
	- Manually define milestones – Track baseline milestones in Planner
	- Use HAL - under development, will keep snapshots of milestone changes over time
	- Export to Excel – Export task lists to Excel for manual baseline comparisons
### Custom Reporting

What They’ll Miss:

- Project Professional provides customizable, detailed reports on tasks, costs, resource utilization, and more.
- How to Mitigate:
	- Use Power BI for advanced reporting – Create custom dashboards that mirror Project Professional reports
	- Export to Excel – For PMs who prefer Excel-based analysis, exporting from Planner allows further customization.
### Offline Access and Control

What They’ll Miss:

- Project Professional works entirely offline, allowing PMs to plan and analyze without an internet connection.
- How to Mitigate:
	- Encourage the **Planner mobile** app – The Planner app allows task updates and viewing offline, with sync once back online.
	- Framing the Transition to Ease Resistance
	- Use Excel backups – export Planner task data to Excel periodically for offline reference. Just don't make changes in the file as they won't show up in Planner!
## Focus on the benefits

Senior Project Managers may resist moving to Planner Premium because it feels like, and in some cases is, a step down from the control and complexity of Project Professional. To win them over:

1. Planner is a tool for team-based execution - Planner simplifies collaboration, communication, and real-time updates, not extremely detailed scheduling.

2. Hybrid approach – use Planner for team execution and Planner Premium for high-level strategic planning

3. Automation and AI – Copilot and Power Automate can reduce manual effort and improve accuracy.

4. Modern accessibility – Planner is cross-platform, integrated with Teams, and cloud-based which means there are fewer barriers to adoption

5. Ongoing training and support – make sure senior PMs feel comfortable with Planner’s interface
## Strategic Message

Encourage PMs to offload tactical execution to Planner, freeing them to focus on strategic oversight. By showing how the broader Microsoft ecosystem (Teams and Power BI) can fill the gaps left by Project Professional, you’ll make the transition more appealing.
## Detailed comparison

Here’s a detailed comparison between Microsoft Project Professional (standalone) and Microsoft - Planner Premium, organized by feature category. This assumes that Project Professional is being used strictly as a standalone desktop tool without connection to Project Online or Project Server - which reflects the most limited collaboration setup and the one we have at work.
### Summary of Differences

| **Feature**         | **Project Professional (Standalone)** | **- Planner Premium**                    |
| ------------------- | ------------------------------------- | ---------------------------------------- |
| Collaboration       | None                                  | Real-time with Teams integration         |
| File Sharing        | Manual                                | Live sharing via OneDrive/SharePoint     |
| Task Scheduling     | Complex, highly detailed              | Flexible but simplified                  |
| Resource Management | Detailed, no real-time sync           | Real-time workload balancing             |
| Reporting           | Advanced, custom reports              | Prebuilt and interactive dashboards      |
| Agile Planning      | Basic                                 | Built-in backlogs, sprints               |
| Automation          | VBA (complex)                         | Power Automate (intuitive)               |
| AI Support          | None                                  | Copilot for task generation and tracking |
### Tasks

- Project Professional:
	❌ Tasks can be created and assigned within the project file, but the file is not shared in real time.
	❌ Task updates must be manually saved and redistributed to stakeholders.

- Planner Premium:
	✔️ Tasks can be created, assigned to team members, and updated in real time.
	✔️ Task changes are reflected instantly for all team members.
	✔️ Multiple task categories (e.g., priority, labels) are available.
	✔️ Timeline Views in addition to Gantt Charts
### ### Agile and Sprint Planning

- Project Professional:
	❌ doesn't really support Agile methods 

- Planner Premium:
	✔️ Native support for Agile planning with backlogs and sprints.
	✔️ Tasks can be moved between sprints and progress tracked automatically.
### Gantt charts

- Project Professional:
	✔️ Full Gantt chart support with task dependencies, lead/lag times, and critical path analysis.
	✔️ Highly detailed control over task scheduling and constraints.

- Planner Premium:
	✔️ Provides a Timeline (Gantt) view with task dependencies.
	✔️ Suitable for most task tracking but lacks the complex scheduling flexibility of Project Professional.
	✔️ Task Dependencies
### Task dependencies

- Project Professional:
	✔️ Supports task dependencies: Finish-to-Start, Start-to-Start, Finish-to-Finish, Start-to-Finish.
	✔️ Allows manual adjustment of dependency relationships

- - Planner Premium:
	✔️ Supports task dependencies: Finish-to-Start, Start-to-Start, Finish-to-Finish, Start-to-Finish
	✔️ Dependencies are updated automatically across the project when changes occur

- Project:
	✔️ Allows creation of **recurring tasks** with complex patterns (e.g., every Monday, every 2nd Wednesday).
- Planner Premium:
	❌ No support for recurring tasks
#### Resource and Workload Management

- Project :
	✔️ Allows assigning resources (e.g., people, materials) to tasks.
	✔️ Provides detailed resource costing and utilization reports.
	❌ No real-time tracking of resource availability across projects unless using Project Online.

- Planner Premium:
	✔️ Allows assigning team members to tasks.
	✔️ Provides visibility into workload through the People view.
	✔️ Updates resource allocation in real time as tasks are reassigned.
	✔️ Resource Leveling

- Project Professional:
	✔️ Allows manual and automatic leveling of resource conflicts.

- Planner Premium:
	❌ No direct resource leveling, but workload balancing can be adjusted manually using the People view.
#### Collaboration and Communication

 - Project
	❌ Project Professional has no built-in collaboration
	❌ The project file is not shared in real time; updates must be distributed manually.

- Planner Premium:
	✔️ Fully integrated with Microsoft Teams for real-time collaboration.
	✔️ Team members can comment on tasks and tag others.
	✔️ Notifications for task assignments and status changes are automated.
	✔️ File Sharing
#### Storage

- Project Professional:
	❌ Project plans are stored as separate (`.mpp`) files in folders 
- Planner Basic
	❌ Plans are managed within Planner's app storage
- Planner Premium
	✔️ plans are stored in Microsoft [[Dataverse]], part of Azure
### Reporting and Analytics

#### Progress Tracking and Dashboards

- Project Professional:
	✔️ Provides detailed progress reports and earned value analysis.
	✔️ Supports creating custom charts and graphs.

- Planner Premium:
	✔️ Provides visual dashboards for progress tracking.
	✔️ Real-time updates to charts and task completion data.
	✔️ Lacks the granular control over financial reporting available in Project Professional.
	✔️ Burndown and Velocity Tracking
#### Burndown charts

- Project Professional:
	✔️ Provides burndown charts and velocity tracking through custom reports.

- Planner Premium:
	✔️ Includes built-in burndown charts and velocity tracking for sprints.
#### Automation and AI

- Project Professional:
	❌ No built-in automation unless combined with Power Automate or VBA scripting.

- Planner Premium:
	✔️ Direct integration with Power Automate for automating task creation, notifications, and more.
	✔️ Copilot for generating tasks, setting goals, and adjusting schedules dynamically based on progress
### User Experience and Accessibility

#### User Interface

- Project Professional:
	❌ Complex interface tailored for experienced project managers.
	❌ Steep learning curve due to the number of options and configurations.

- Planner Premium:
	✔️ Simple, intuitive interface designed for quick adoption by teams.
	✔️ Accessible via browser, Microsoft Teams, and mobile apps.
	✔️ Platform Support

### Security and Permissions

- Project Professional:
	❌ Local file-level permissions only.
	❌ No role-based access unless using Project Server or Online.

- Planner Premium:
	✔️ Role-based access with Owners, Members, and Guests
	✔️ Supports Microsoft 365 sensitivity labels and compliance policies
## Why Move to Planner Premium

1. Real-time collaboration – Teams can communicate, adjust schedules, and track progress in real time.

2. Accessibility – Cross-platform support with a modern, web-based interface.

3. Integrated environment – Planner Premium fits naturally into the Microsoft 365 ecosystem, enhancing teamwork and productivity.

4. Automation and AI – Copilot and Power Automate reduce manual work and improve decision-making.
## Conclusion

For project managers currently using Project Professional as a standalone tool, transitioning to - Planner Premium will provide them with real-time collaboration, simplified task management, and automation. 
## References

1. [When to use Microsoft Project, Planner, To Do, or the Tasks app in Teams](https://support.microsoft.com/en-us/office/when-to-use-microsoft-project-planner-to-do-or-the-tasks-app-in-teams-8f950d32-d5f4-40db-a8b7-4d1b82b55e17) - Microsoft
2. [Microsoft Planner Datasheet](https://cdn-dynmedia-1.microsoft.com/is/content/microsoftcorp/microsoft/final/en-us/microsoft-brand/documents/MSFT-Planner-Infographic-Final.pdf) - Microsoft
3. [Planner Blog](https://techcommunity.microsoft.com/category/planner/blog/plannerblog) - Microsoft's Tech Community, ["planner premium" query](https://techcommunity.microsoft.com/search?q=planner+premium&location=category%3AMicrosoftLearn)
4. [Microsoft Planner AMA](https://aka.ms/NewPlanner/AMA), Microsoft, 2024-04-04
5. [Introducing the Project Accelerator](https://techcommunity.microsoft.com/blog/projectblog/introducing-the-project-accelerator/2201000), Microsoft, 2021 - ==I would avoid this at all costs==
6. [Microsoft Project for the web service description](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description) - learn.microsoft.com
7. [Project for the web and Project Online](https://support.microsoft.com/en-us/office/project-for-the-web-and-project-online-6569170c-5c8e-474e-a7f0-642872f62f8a) - Microsoft Support 