---
tags:
  - app
aliases:
  - Lists
slug: ms-list
organizations:
  - microsoft
url: 
email: 
blog: 
help: 
support_url: 
forums: 
integrations: 
stack:
---

# SharePoint Lists

## References

1. [How to create Microsoft - SharePoint lists with integrated Approval Workflows](https://youtu.be/zceFuXw5D7w) #to-do 
2. [Fastest Way to edit large SharePoint lists](https://www.youtube.com/watch?v=MPJ51O9Oj-w)
3. [[Listbusters]]
4. [[Listbusters in the lab with Microsoft Lists’ Miceile]]
5. [Lazyadmin](https://lazyadmin.nl/office-365/sharepoint-lists/#sharepoint-list-permissions)
6. [Understanding Permission Levels](https://learn.microsoft.com/en-US/sharepoint/understanding-permission-levels)
7. [Hacking low-level security](https://sharepoint.stackexchange.com/questions/304174/sharepoint-list-how-to-limit-items-in-list-with-formula/304176#304176)
8. [Creating custom lost templates](https://learn.microsoft.com/en-us/sharepoint/lists-custom-template) Microsoft
9. [Disable list templates at the org level](https://learn.microsoft.com/en-us/sharepoint/control-lists?source=recommendations)
10. [Package lists and flows in a template oh my!](https://learn.microsoft.com/en-us/sharepoint/package-biz-apps-org-list-template?source=recommendations)p
1. [Working with lists and liste items with REST](https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/working-with-lists-and-list-items-with-rest) - Microsoft [[Sharepoint REST]]
2. [Introduction to lists](https://support.microsoft.com/en-us/office/introduction-to-lists-0a1c3ace-def0-44af-b225-cfa8d92c52d7)
3. 

    > you can create a packaged SharePoint list template that contains in-built custom flows. The objective is to assemble and register a packaged file that contains the site script actions needed to create the list and the flows, and a Dataverse solution archive (zip) that contains the flow definitions.

## Notes

From [5]

- Calculated Columns
- Interesting types #to-do look into these

Colum Type | Description 
---|---
Managed metadata | Allows you to select managed metadata
Lookup | Allows users to select a reference/row from another SharePoint List. Creates a direct link to it.
External Data | Can be used in combination with Business Connectivity Services
Task Outcome | Used in combination with Workflows

**Creating List Views**

All SharePoint Lists have one default view that will show all the columns. In some cases, you want to create distinct views, that only show a couple of the columns, or the items that match a certain condition. To create an extra view for your SharePoint Lists:

1. Open `Settings` and select `List Settings`
2. Scroll down to `Views` and click on `Create View` (all the way the bottom of the list settings page)
3. Give your view a name
4. Scroll down to `Filter`
5. Select `Show items only when the following is true`
6. Select the column, `Order` new, set it to `is Equal to` and as `value` use `Yes`

> Sharepoint List Permissions
Permissions are the last part of the SharePoint lists that we are going to look at. A SharePoint list has in basis the same permission structure as an document library. So if you want to make the list read only, then you can use the SharePoint permissions for that. I have written an article about SharePoint Permissions, which you can find here.

It’s also possible require approval before new items can be added to the list. This way members of the SharePoint site can add new items to the list, but only owners can approve the new list items. To do this we will need to configure the Versioning Settings in the List Settings:

1. Click on `Settings` and select List Settings
2. Open the `Versioning Settings`
3. Set `Require content approval for submitted items` to Yes
4. (optional) Change the draft Item security so that only owners can see draft items
5. When a new item is added to the list, the approval status will be set to `Pending`. List owners can approve items by selecting the list item, click on `More Options` and choose `Approval`/`Reject`.
