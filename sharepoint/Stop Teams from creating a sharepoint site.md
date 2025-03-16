# Stop Teams from creating a sharepoint site

## References

1. [How do I stop Microsoft Teams from creating a SharePoint site?](https://answers.microsoft.com/en-us/msteams/forum/all/how-do-i-stop-microsoft-teams-from-creating-a/a6b92ecd-e923-42a7-9642-8f5c2500b62c) - 2023-02-14
2. [Manage site creation in SharePoint](https://learn.microsoft.com/en-us/sharepoint/manage-site-creation) - 2023-02-21
3. [Create a Microsoft Team from SharePoint](https://support.microsoft.com/en-us/office/create-a-microsoft-team-from-sharepoint-545973b6-c38f-426a-b2b6-16405a561628)
4. [Overview of Teams and SharePoint integration](https://learn.microsoft.com/en-us/SharePoint/teams-connected-sites) - 2023-02-21

> Each team is connected to a Microsoft 365 group in Azure AD where the team membership is stored. The files you see on the **Files** tab in a team are stored in a SharePoint site. All standard channels in a team share the same SharePoint site, but each private channel has its own site.
> - [4]

![[Teams and SharePoint.excalidraw]]

## When do Teams and SharePoint get connected?

> Teams and SharePoint are connected in the following scenarios:
> 
> -   When you create a new team from scratch, a new SharePoint site is created and connected to the team.
> -   When you create a new team from an existing Microsoft 365 group, the team is connected to the SharePoint site associated with the group.
> -   When you add Teams to an existing SharePoint site, that site is connected to the new team.
> -   When you create a new private or shared channel, a new SharePoint site is created and connected to that channel.
> 
> In Teams, the Files tab on each standard channel is connected to a folder in the parent site's default document library. The Files tab on each private and shared channel is connected to the default document library in the corresponding channel site. Whenever you add or update a file on the Files tab, you are accessing the SharePoint site.