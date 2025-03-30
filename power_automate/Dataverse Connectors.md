---
tags:
  - term
source: chatGPT
---
[[Dataverse]] Connectors are integrations that allow applications to connect to **Microsoft Dataverse**, enabling seamless data exchange between Dataverse and external services. They are primarily used in **[[Power Platform]] ([[Power Automate]], [[Power Apps]], [[Power BI]])** and other [[Microsoft 365]] services to interact with Dataverse data.
### Types of Dataverse Connectors**

1. **Standard Dataverse Connector**
    
    - Used in [[Power Apps]], [[Power Automate]], and [[Power BI]].
    - Provides access to tables (formerly entities) in Dataverse.
    - Supports CRUD (Create, Read, Update, Delete) operations.
        
2. **Premium Dataverse Connector**
    
    - Offers advanced capabilities like direct SQL queries and choice fields.
    - Required for more complex workflows and enterprise integrations.
        
3. **Custom Connectors**
    
    - Allows integration with external APIs using [[OpenAPI]] definitions.
    - Used when a required service doesn’t have a built-in connector.
### Key Features

✔️ **No-code/low-code integration** – Ideal for Power Apps and Power Automate.  
✔️ **Data security & governance** – Leverages Dataverse’s role-based security model.  
✔️ **Supports real-time & scheduled automation** – Automate tasks with Power Automate.  
✔️ **Deep integration with Microsoft 365** – Connects with Teams, Outlook, and SharePoint.

### Common Use Cases

- Syncing Dataverse data with [[SharePoint]] or Excel.
- Automating email notifications based on Dataverse data changes.
- Creating [[Power BI]] reports using Dataverse tables.
- Integrating external CRM or ERP systems with Dataverse.