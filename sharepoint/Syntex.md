---
tags:
  - app
slug: syntex
organizations: [microsoft]
url: https://adoption.microsoft.com/en-us/syntex/
github_id: 
integrations: 
stack: 
---

# Syntex

## Summary

## Quotes

> Take all the power of [@SharePoint](https://twitter.com/SharePoint) and [@Office](https://twitter.com/Office) an inject it straight into your custom applications! - Zach Rosenfield
## People

- [Zach Rosenfield](https://devblogs.microsoft.com/microsoft365dev/author/zachros) Partner Group Product Manager, Collaboration Platform & [[Microsoft]] Syntex

## References

1. [Introducing Syntex repository services: Microsoft 365 superpowers for your app](https://devblogs.microsoft.com/microsoft365dev/introducing-syntex-repository-services-microsoft-365-superpowers-for-your-app/)
2. [podcast](https://www.podbean.com/media/share/pb-smsdn-1438a5d?utm_campaign=embed_player_share&utm_medium=dlink&utm_source=embed_player) - Reid Carlberg and Marc Windle about Syntex respository services

## Notes

- in private preview from 2023-06
- a faster way to build file and document focused apps
- Syntex repository services are powered by [[SharePoint]]
- no user experience layer (headless) and is fully API driven
- [[Microsoft Loop|Loop]] app is 100% powered by Syntex repository services, as are apps such as [[Edge Spaces]] and [[Designer]]
- accessible via the easy-to-use [[Microsoft Graph API]]
- make it easy to deliver rich collaboration experiences for Office document types as part of your application. This includes Word, Excel, and PowerPoint, and it supports apps built on the [[Fluid Framework]]
- can provide web access to all users, regardless of their Microsoft 365 subscription status

From [1]

> - Build inside the [[Microsoft 365]] tenant boundary for both enterprise and ISV apps
> - Extend advanced Microsoft 365 security and compliance to your app
> - Deliver Microsoft 365 collaboration to your customers, users, and guest users as part of your app
> - Embed Microsoft’s trusted content management capabilities in your app

![[MS Loop Stack.png]]

> innovation behind this new capability is a ==special type of partition in the Microsoft 365 storage layer that we call repository containers==.

> not accessible through regular Microsoft 365 UX
> completely controlled and managed by the app that creates them

> your app can do critical things like audit file level activity; run global e-discovery queries that work across all your repository containers in addition to SharePoint files, OneDrive files, emails and Teams chats; and query for specific user activity across all files as well. Customers can apply retention policies, harness data loss prevention policies (DLP), use sensitivity labels, enforce conditional access policies and a whole lot more.

> this keeps all the documents you need to manage within your Microsoft 365 tenant but still isolated from the rest of your Microsoft 365 user experience

### From [2]

**Reid Carlberg**

- a PaaS
- You get these things
	1. All the security and compliance part of MS365 and Purview 
	2. Collaboration and co-authoring capabilities part of Office 365 products
	3. Preview for files including PDF, images, video text, ...
	4. Content management: versioning, large file handling, custom thumbnails, search
- Within tenant boundary
	- configuration
	- shared services: MS365 Storage Services - you get a partition in this

**Marc Windle**

- unlike SharePoint, it's ==a metered service== 
	- separate from M365 entitlements
	- doesn't affect customers storage quotas
	- consumption based model, usage determines cost
- all APIs on Microsoft Graph to create/update containers in M365 Tenant
- get an ID and it's like a Drive
- preview endpoint on Microsoft Graph API - embed in iFrame or open in new tab
- Developers can get a separate scope from all the other organization's data which is better for governance and resource protection