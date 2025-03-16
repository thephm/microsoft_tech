---
tags: [article]
url: null
date: null
slug: null
read: no
service: null # where posted
products: [sharepoint]
duration: null
---

# SharePoint Add-Ins

![rw-book-cover](https://learn.microsoft.com/en-us/media/logos/logo-ms-social.png)

## Metadata
- Author: [[Vesa Juvonen]]
- URL: https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/sharepoint-add-ins

## Highlights
- two basic kinds of SharePoint Add-ins: SharePoint-hosted and provider-hosted
- A device app, such as mobile app, isn't really a "SharePoint Add-in" even when it accesses SharePoint. The same is true of a web application that is launched from outside of SharePoint. If you want to develop any of these kinds of apps, see [Access SharePoint from mobile and native device apps](https://msdn.microsoft.com/library/42014171-5ee5-421d-9cde-413efc3aecef%28Office.15%29.aspx)
- **A SharePoint Add-in is a self-contained piece of functionality** that extends the capabilities of SharePoint websites to solve a well-defined business problem.
- **Add-ins don't have custom code that runs on SharePoint servers**. Instead, all custom logic moves "up" to the cloud, or "down" to client computers, or "over" to an on-premises server that is outside the SharePoint farm or SharePoint Online subscription. Keeping custom code off SharePoint servers provides reassurance to SharePoint administrators that the add-in can't harm their servers or reduce the performance of their SharePoint Online websites.
- **Business logic in a SharePoint Add-in can access SharePoint data through one of the several client APIs included in SharePoint**. Which API you use for your add-in depends on certain other design decisions you make.
- **Almost all major types of SharePoint components can be part of a SharePoint Add-in**, including pages, lists, workflows, custom content types, list templates, web parts, and more.
- **The SharePoint websites where SharePoint Add-ins are installed, and from which users launch them, are called host webs.** The SharePoint components, however, are generally in a special child web of the host web called the add-in web. (M
- **SharePoint Add-ins can fit into a SharePoint website in several ways**:

  : **As an immersive full-page experience** that can have the look and feel of a SharePoint page.

  : **As part of a webpage, using a special kind of control called an add-in part**, to surface an iframe element that contains the add-in.

  : **As UI commands that extend ribbons and menus** for lists, documents, and more.
- **All SharePoint Add-ins that users install get a tile on the Site Contents page of the SharePoint website.** Clicking the tile runs the add-in.
- **A SharePoint Add-in is configured using an *add-in manifest***—an XML file that declares the add-in's basic properties, where it runs, and what SharePoint should do when the add-in starts. Among other things, the manifest can specify what languages the add-in supports, what SharePoint services and functionality it depends on, and the permissions to the host web that the add-in needs. (SharePoint Add-ins have full control of their own add-in web.)
