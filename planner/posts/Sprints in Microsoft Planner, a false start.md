---
tags:
  - post
url: https://planner-ms.ghost.io/sprints-in-microsoft-planner/
date: 2025-06-14
people:
  - otto
service: ghost
---

# Sprints in Microsoft Planner, a false start

I delve into how Microsoft Planner supports Sprints. While it's not a first-class feature, it can still be useful for basic Scrum-style projects.

Another week goes by and another post gets crafted. This week I was stumped by how Microsoft Planner supports Sprints.

So far in my journey learning about Planner, I've covered the differences between [Project Professional and Planner](https://planner-ms.ghost.io/project-professional-vs-planner-premium/) premium plans, actually [twice](https://planner-ms.ghost.io/project-professional-vs-planner-premium/), moved onto the basics of [buckets, tasks, and subtasks](https://planner-ms.ghost.io/buckets-tasks-and-subtasks/), then [labels](https://planner-ms.ghost.io/using-labels-in-microsoft-planner/), [dependencies](https://planner-ms.ghost.io/dependencies-in-microsoft-planner/), [sharing](https://planner-ms.ghost.io/planner-plans-to-share-or-not-to-share-that-is-the-question/) plans, [filters](https://planner-ms.ghost.io/microsoft-planner-filters/), task [history](https://planner-ms.ghost.io/microsoft-planner-task-history/), and last week [goals](https://planner-ms.ghost.io/goals-in-microsoft-planner/)! Maybe I should've started with goals 🤣 That's a pretty good set of features that I've covered already.

In my last post I forgot to mention an [interesting message](https://www.reddit.com/r/plannerpremium/comments/1l48ueq/planner_is_making_me_miserable_does_it_get_better/?ref=planner-ms.ghost.io) posted in my [r/plannerpremium](https://www.reddit.com/r/plannerpremium/?ref=planner-ms.ghost.io) subreddit titled "Planner is making me miserable - does it get better?"! The user vented their frustration implementing Microsoft Planner for their new team. They're experienced with other tools like Asana and Jira but find Planner difficult and limiting — especially the lack of recurring tasks and bulk editing for assigning tasks or changing due dates. Despite trying to learn from resources online, they feel overwhelmed by Planner’s limitations and performance issues. They’re considering asking IT for permission to switch to a third-party tool.

In my response I tried to acknowledge the original poster's frustration and offer a different perspective. I don’t find recurring tasks necessary in project planning and suggested calendar events as a better fit for repeated work. Similarly, I prefer a "pull" model where team members assign tasks to themselves when ready, rather than command-and-control and bulk-assigning tasks far in advance. I don't think that helped the person but made me wonder how many people actually bulk assign tasks or create recurring tasks. Let me know if you do.

This week I'll cover Sprints; a time-boxing technique used heavily in Scrum-style projects and they can be equally useful in any project or parts of a project.

### Another hidden feature

Sprint features are not available in Planner basic plans so you need a Planner Plan 1 or above (or Project Plan 3/5) licenses. As a reminder that part of Microsoft’s consolidation, Project for the Web is being retired in August 2025, and its premium features including sprints are migrating into Planner premium plans.

I thought Sprints would be a first-class feature in Microsoft Planner. The first place I would've thought they'd appear was here in the main set of tabs at the top of all pages:

![[Microsoft Planner - Project tabs, no Sprints to be found.png]]

*Project tabs, no Sprints to be found*

But no, they're not there. To show sprints, you need to go into the Board view, click the "`Group by Bucket`" and change that to "`Sprint`".

![[Microsoft Planner - Group by Sprint.png]]

OK, now that you know where to find sprints, I can show you how to add a new one. At least that part is obvious.

### Add a Sprint

Once you're viewing sprints, use the big "`Add sprint`" button:

![[Microsoft Planner - Add Sprint.png]]
*Add sprint under Board view*

This little dialog appears where you can give the sprint a name and set the start and end dates.

![[Microsoft Planner - Add Sprint dialog.png]]
*Add sprint dialog with sprint name, Start, and Finish dates*

If you create an overlapping sprint, Planner still displays the sprint as well as a thin error message at the top of the page.

![[Microsoft Planner - Overlapping sprint.png]]

You'll need to correct the date on the newly added sprint because if you reload the page, it will be gone. It's not the best user experience but at least it doesn't let you create overlapping sprints.

### Delete or rename the Default Sprint

In the Board view you can rename or delete the Default Sprint. I didn't want it laying around.

1. To rename it, double-click the title and type a new name
2. To delete it, hover over the title, click "...", and then "`Delete`"

![[Microsoft Planner - Remove default sprint.png]]
*"..." menu on a Sprint with Rename and Delete options*

### Ordering of sprints in Board view

The only other small feature in the Board view related to sprints is the ability to order them from left-to-right or right-to-left. You can find that option here:

![[Microsoft Planner - View Options.png]]

You know how to find sprints, add a new one, and order them. Now I'll show you how to include the sprints in the Grid view.

### Showing Sprints in Grid view

To include the sprint in Grid view, use the "`+ Add column`" button the far right of the table view as shown here:

![[Microsoft Planner - Add Column Sprint in Grid view.png]]
*Add column - Sprint*

A new column will be added to the table and you can then assign tasks to sprints from within the table.

### Filtering by Sprint

Just like all of the other Planner features, you can filter your project Tasks by sprints in pretty much every view here:

![[Microsoft Planner - Filter by Sprint.png]]
*Filter Tasks by Sprint*

That's about it for sprints in Microsoft Planner.

### A minimal quasi-viable product

It looks like Microsoft is not ready to fully support Scrum-based projects given how hidden the sprint feature is. It feels like an afterthought.

I wish you could hide old sprints and I was very surprised that you can't associate a Sprint with a goal since setting sprint goals is very common in Scrum.

There is no sprint burn up or burn down charts or cumulative flow diagrams. I expect they will add support for epics/stories down the road and until then, sprint support is pretty basic.

I saw this [What's new in Microsoft Planner](https://techcommunity.microsoft.com/blog/plannerblog/whats-new-in-microsoft-planner---january-2025/4371460?utm_source=chatgpt.com) post from January mentioning other features. It may be that my subscription doesn't have them:

> Get started quickly with new out-of-box templates. We’ve added new premium templates—Goals & Objectives, Project Retrospective, Event Planning, Training Plan, and Sprint Retrospective—that can help you set goals, organize sprints, plan events, and more!

### The end

If you're using something like Jira today, you will be disappointed with the sprint support in Microsoft planner. If you're not running large Scrum projects and just need to setup basic sprints, then this feature could work for you. Try it out and let me know if I've missed anything. Knowing Microsoft and their strategy of embrace, extend, kill other products, this is an area to keep an eye. Jira is not cheap.

That's it, another post done. Have a great weekend ahead, rest up, and then sprint away this coming week!

Otto.

p.s. sharing is caring so please forward this post to a colleague or a link to [otto-ms.bsky.social](https://bsky.app/profile/otto-ms.bsky.social?ref=planner-ms.ghost.io) or [r/plannerpremium](https://www.reddit.com/r/plannerpremium?ref=planner-ms.ghost.io)