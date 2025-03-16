# SharePoint Sites and Content API Overview

![rw-book-cover](https://learn.microsoft.com/en-us/media/logos/logo-ms-social.png)

- Author: [[MSGraphDocsvTeam]]
- URL: https://learn.microsoft.com/en-us/graph/sharepoint-concept-overview


- use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content
- Microsoft 365 groups, Microsoft Teams, and portals are all based on SharePoint
- Use the SharePoint API in Microsoft Graph to access:
  • Team sites that store the content that users collaborate on with their coworkers.
  • Communication sites and portals where users publish rich content pages to share across the organization.
- Unleash your data with SharePoint lists
  [Lists](https://learn.microsoft.com/en-us/graph/api/resources/list) are the foundation for data storage in SharePoint. [Create lists](https://learn.microsoft.com/en-us/graph/api/list-create) to store a variety of business data, from a simple customer contact list to a custom business application, fronted with Power Apps. When you use [columns](https://learn.microsoft.com/en-us/graph/api/resources/columndefinition) to define your schema, SharePoint can protect the integrity of your data as well as enable rich indexing, querying, and search capabilities.
- SharePoint stores files in a special [list type](https://learn.microsoft.com/en-us/graph/api/resources/listinfo) called a document library. You can use the [OneDrive API](https://learn.microsoft.com/en-us/graph/api/resources/onedrive) to work with a library as a [drive](https://learn.microsoft.com/en-us/graph/api/resources/drive), or the SharePoint API to work with it as a [list](https://learn.microsoft.com/en-us/graph/api/resources/list). Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.
- With Microsoft Graph, you can surface your users' most important data within your app. Keep things fresh by [querying](https://learn.microsoft.com/en-us/graph/api/listitem-get) the list that stores your users' data. [Create](https://learn.microsoft.com/en-us/graph/api/list-create) your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.
- The [SharePoint Framework](https://learn.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview) provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages
- [SharePoint Add-ins](https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/sharepoint-add-ins) are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server
- To learn about these models in more detail, visit the [SharePoint Dev Center](https://developer.microsoft.com/sharepoint) or the [SharePoint Developer Docs](https://learn.microsoft.com/en-us/sharepoint/dev/).
  API reference