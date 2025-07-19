---
tags:
  - post
url: https://planner-ms.ghost.io/microsoft-planner-know-your-limits-and-work-within-them/
date: 2025-07-19
people:
  - otto
service: ghost
---

# Microsoft Planner - know your limits and work within them

*Understand the limitations and missing features of Microsoft Planner's premium plans to set realistic expectations and avoid frustration!*

![[Toronto Signs.png]]
*Photo by [Hugo Coulbouée](https://unsplash.com/@hugoclb?utm_source=ghost&utm_medium=referral) / [Unsplash](https://unsplash.com/)*

Welcome to Episode # 16 in this latest [hobby of mine](https://planner-ms.ghost.io/hello-world/) to go deep on Microsoft Planner's premium plans. So far, I've been writing a lot about what you can do in Microsoft Planner and this week I'm going to summarize the things that you can't (yet?) do and some limits that you might run into.

Why? This way you and your teams won't get frustrated. As my dad always said:

> Frustration occurs when expectations don't meet reality.

But first let's start with something positive, a new subscriber!

> [!NOTE] Welcome
> Welcome ****Tad**** from Washington! You're officially Member #16 🕺

This post is all about setting – or re-setting if you've been using the app – expectations about Microsoft Planner so you and your user community don't become frustrated later.

I fully expect that I made mistakes and since Microsoft is investing in this tool right now, the limits and features will change. I used ChatGPT on this post to help find some of the limits as I got tired after adding 105 buckets 😄

Let's get into it!
### The TL;DR on Limits

If your time is limited, you may not want to read the entire post – I won't be offended, just sad 😂 – so I created this table to summarize the **limits on premium plans**.


> [!NOTE] 
> I've included notes where specific features are not supported in Planner basic plans, i.e. plans that come as part of Microsoft 365.

I include hyperlinks to my posts on the specific feature and elaborate more on basic vs. premium plans in another section below.

|Feature|Maximum|Per|Note|
|---|---|---|---|
|[Buckets](https://planner-ms.ghost.io/buckets-tasks-and-subtasks/)|Unlimited|Plan|Practically 100 to 200|
|[Tasks](https://planner-ms.ghost.io/buckets-tasks-and-subtasks/)|3,000|Plan||
|Checklists|20|Task||
|Attachments|10|Task||
|[Dependencies](https://planner-ms.ghost.io/dependencies-in-microsoft-planner/)|20|Task|Unsupported in Basic plans.|
|[Dependencies](https://planner-ms.ghost.io/dependencies-in-microsoft-planner/) - Types|4|Task|Finish to Start/Finish, Start to Finish/Start|
|[Labels](https://planner-ms.ghost.io/using-labels-in-microsoft-planner/)|25|Plan|Color coded|
|[Custom Fields](https://planner-ms.ghost.io/microsoft-planner-custom-fields-of-dreams/)|10|Plan|Unsupported in Basic plans.|
|Custom Fields - Text|4,000|Field|Free form up to this many characters|
|Custom Fields - Choice|25|Field|Menu items|
### The TL;DR on Features

For the missing features / wish list, I've summarized some of the ones that I know of and I suppose this list could be a lot longer and you have some key features you'd want.

Premium seems to strip away simple conveniences from the Basic experience, making some workflows slower or impossible.

These are not only the **Feature**s that I see as missing but also those gaps people are complaining about on forums. I include my personal emotion via emoji. Why? Because it's fun - for me.

| Feature                     |     | Notes                                                                       |
| --------------------------- | --- | --------------------------------------------------------------------------- |
| Comments                    | 🤬  | No comments with date/time, commentor, replies, resolve.                    |
| Recurring Tasks             | 😬  | Daily, weekly, monthly - biggest complaint from users.                      |
| Copy/move between plans     | 😮  | Tasks can't be copied from personal to Premium.                             |
| More Custom Field types     | 🙏  | Missing multi-select and person fields.                                     |
| Workflow                    | 😤  | No create/promote subtasks if hiding completed tasks.                       |
| Checklist/comments on cards | 🤦  | Only inside task. Basic supports this.                                      |
| Sort grid view              | 🤔  | Grid view sorting in Basic plans only.                                      |
| Automation                  | ⚙️  | Via Dataverse but Power Automate in basic.                                  |
| Simple status               | 🚦  | Basic plan has simple status but premium has % complete with enforced dates |
### Basic to Premium

Premium plans are missing simple conveniences that exist in Basic plans, making some workflows slower or impossible.

Planner users expect "more” by paying for advanced features in Plan 1 and above license tiers but many report a net loss on usability in areas like recurring tasks, automation, board readability, and basic task actions.

If your team heavily relies on recurring tasks, in-card comments/checklists, automation workflows, or needs basic status/status simplicity, then basic plans might offer a better experience. Premium plans add dependencies, timeline/Gantt, milestones, goals, subtasks, and custom fields but sacrifice familiar, usable features in Basic plans.

I recommend visiting Microsoft’s official [planner feedback channels](https://feedbackportal.microsoft.com/feedback/forum/a1a93b69-2f1c-ec11-b6e7-0022481f8472?ref=planner-ms.ghost.io) or [Tech Community](https://techcommunity.microsoft.com/category/Planner?ref=planner-ms.ghost.io) to upvote requests for restoring "lost functionality". As of this writing, there are 1,798 items posted in the feedback channel. In the Tech Community you can browse discussions, ask questions, share feedback, and follow updates from the Planner product team.

The following sections go into more detail on a few of the feature gaps. First up my favorite feature and gap, labels.

### 25 labels per plan

As I described in my [Read this before using labels in Planner](https://planner-ms.ghost.io/using-labels-in-microsoft-planner/) post, Planner only allows 25 labels per plan. I know, that's ridiculous and hopefully someone in the product team at Microsoft realizes how limiting that is. There are oodles of posts on Microsoft Community about it going back over 4 years!

- [unlimited labels](https://techcommunity.microsoft.com/discussions/planner/unlimited-labels/3262448?ref=planner-ms.ghost.io) - Mar 21, 2022
- [Need more labels](https://techcommunity.microsoft.com/discussions/planner/need-more-labels/3876342?ref=planner-ms.ghost.io) - Jul 17, 2023
- [maximum number of labels](https://techcommunity.microsoft.com/discussions/planner/maximum-number-of-labels/4049080?ref=planner-ms.ghost.io) - Feb 05, 2024
- [Planner - Add more than 25 Labels](https://techcommunity.microsoft.com/discussions/planner/planner---add-more-than-25-labels/4229166?ref=planner-ms.ghost.io) - Aug 26, 2024

**More labels please!**

Another feature sinkhole is commenting.

### No comment

In Planner premium plans, task **comments are not stored inside the Task** card itself like in basic plans. They have a little Note field and instead of a comments, there's a Conversation feature where you're redirected to a linked Microsoft Teams conversation thread and messages are stored in a dedicated channel conversation within the linked Teams team.

![[MS Planner - Add a note - Conversation.png]]

Each conversation is labeled with the task name e.g., `[Task] Launch campaign`. I haven't used the feature yet, but from what I've read this approach adds friction as you must go into Teams from Planner, tasks aren't in the same channel, and they're generally harder to follow.

```
<rant>
Likely Microsoft did this with an aim to standardize communications across M365 using Teams – maybe for compliance and auditability – and to centralize chat history in Teams/Outlook rather than in Planner. They keep pushing people towards Teams as a hub and that drives me nuts. Instead, they should have the comment function as a first-class citizen in Planner and then have it show up in Teams team.
</rant>
```

Next up and not a big limitation for me to-be-honest, attachments.

### **10 attachments per Task**

You're limited to 10 attachments per task and these include: file attachments from SharePoint/OneDrive or upload, hyperlinks (Links, URLs), and embedded files from Teams or other M365 services.

The limit applies to the _total number_ of attachments, not just files. Each file must also comply with SharePoint/OneDrive file size limits which is up to 250 GB as of now – that's pretty big unless you work with video files.

File attachments are stored in the connected Microsoft 365 Group’s SharePoint document library. I find it difficult to know where things are sometimes across all of the MS365 products. _Note to self: another post idea._

Here are a few workarounds to this limitation:

- Upload a folder with multiple documents to SharePoint and link the folder
- Link to an index file like a Loop or Excel file with list of files / links
- Use a document such as a Word or OneNote file with embedded content

That's it!

### The end of the beginning

In this post, I shared the limits of the features and listed many of the features that are "missing" from premium plans. Oddly, many of those missing functions already exist in the free "basic" plans that come with your Microsoft 365 license.

We're relatively at the beginning of the Microsoft Planner premium plan product variant and I expect – _hope?, pray?, **beg?!**_ – that Microsoft will close the big gaps between their products.

I will aim to keep this page updated and notify you of changes as I hear about them. My ask is that you do the same i.e. please let me know of errors, omissions i.e. other limitations, or notify me if Microsoft closes a gap and I didn't tell you.

Thanks for subscribing and may your week ahead be feature-full with no surprises on what's in and out of Planner premium.

Otto.

p.s. please forward to someone or "like" my posts on [BlueSky](https://otto-ms.bsky.social/?ref=planner-ms.ghost.io) or [Reddit](https://www.reddit.com/r/plannerpremium/?ref=planner-ms.ghost.io)