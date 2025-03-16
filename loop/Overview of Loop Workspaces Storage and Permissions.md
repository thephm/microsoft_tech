# Overview of Loop Workspaces Storage and Permissions

- Author: [[MikePlumleyMSFT]]
- URL: https://learn.microsoft.com/en-us/microsoft-365/loop/loop-workspaces-storage-permission?view=o365-worldwide

- Microsoft [Syntex repository services](https://devblogs.microsoft.com/microsoft365dev/introducing-syntex-repository-services-microsoft-365-superpowers-for-your-app/) powered by SharePoint platform stores all Loop app content. All Loop workspaces, pages, and components created in the Loop app are stored in a container in the [[Syntex repository service]], which is designated for that specific workspace.
- Loop components created outside of the Loop app in other Microsoft 365 apps (such as [Teams](https://support.microsoft.com/office/first-things-to-know-about-loop-components-in-microsoft-teams-ee2a584b-5785-4dd6-8a2d-956131a29c81), [Outlook](https://support.microsoft.com/office/use-loop-components-in-outlook-9b47c279-011d-4042-bd7f-8bbfca0cb136), [Whiteboard](https://support.microsoft.com/office/loop-components-in-whiteboard-c5f08f54-995e-473e-be6e-7f92555da347), [Word for the web](https://support.microsoft.com/office/use-loop-components-in-word-for-the-web-645cc20d-5c98-4bdb-b559-380c5a27c5e5)) are stored in the creator's OneDrive.
- Loop workspaces and pages count against your tenant's storage quota ([View Highlight](https://read.readwise.io/read/01hfz963atnaqckx6mnxr8f8yg))
- Sharing the workspace in Loop adds the user to the workspace roster. All workspace roster members have access and "*editing*" permissions to all the Loop pages in that workspace.
- There's a distinction between sharing a specific Loop page with a user versus inviting them to a Workspace.
- When you invite a user to a workspace, that user has access to all the pages in that workspace. Loop only supports inviting users to a workspace via this Workspace roster management flow, which enables access and sends an email invite to the invited users.
- When you share only a Loop page, you're giving users access to that specific page exclusively (not the whole workspace). The user can choose to use a company share link or people-specific share link; unless their tenant admin has disabled some of the share link types. When sharing a page, you can choose to grant the user "*edit*" or "*read only*" access.
## Loop workspaces and Microsoft 365 groups

- Loop workspaces don't use Microsoft 365 groups for access management, instead they create a roster for access management.
- Personal workspaces are also backed by a roster, but there's only one person in them by design. When a user leaves a company, their personal workspaces become "ownerless".
- Loop components created outside of the Loop are stored in the OneDrive of the person who created the component. Therefore, if that user leaves the organization, the standard OneDrive IT policy is applied.