---
tags:
  - post
url: https://planner-ms.ghost.io/use-highlights-to-colorr-code-your-microsoft-planner-plan/
date: 2025-06-28
people:
  - otto
service: ghost
---

# Conditional coloring in Microsoft Planner

Discover how conditional coloring in Microsoft Planner helps you visualize and manage your tasks more effectively.

![[Photo by Josh Maddocks.png]]

Photo by [Josh Maddocks](https://unsplash.com/@joshmaddocks?utm_source=ghost&utm_medium=referral&utm_campaign=api-credit) / [Unsplash](https://unsplash.com/?utm_source=ghost&utm_medium=referral&utm_campaign=api-credit)

Welcome back to another insight into Microsoft Planner as I [find my way](https://planner-ms.ghost.io/hello-world/) through this relatively new tool. I'm taking the easy way out this week and looking at a relatively simple feature. First off some news.

💡Welcome ****Erich**** and ****Catherine**** from Canada and ****Lana**** from Australia! Just when I thought there were only 11 people interested, you three subscribed. Thank you!

With Tuesday being a national holiday here, I took Friday and Monday off to make it a mini staycation. There are a few things that I must do around the house, I need to win games of Rummy 500 with my wife, and I want to work on my other hobbies. "Archie the Archivist" wants to work on the [Signal SQLite to Markdown](https://github.com/thephm/signal_sqlite_md?ref=planner-ms.ghost.io) tool and "[Mr. Tee](https://www.mrtee.ca/?ref=planner-ms.ghost.io)" wants to create some new t-shirts – especially one inspired by a badge I saw on a backpack this week: "Whisky Tango Foxtrot".

Enough pre-amble and onto the focus of this post: conditional coloring in Planner.

**DISCLAIMER**: For the purposes of this post I use the spelling "color" but the real spelling is "colour" for many Canadians.
## Highlights

To highlight certain aspects of your Microsoft Planner plan, go into the Grid view and click on "Conditional coloring" in the top right.

![[MS Planner - Conditional coloring dialog.png]]
*Image: Conditional coloring dialog*

This feature works very much like Excel's Conditional Formatting feature. You first pick an attribute ("`Field`") that you want to highlight, then set some conditions ("`Operator`") that will cause Planner to color the cells matching those conditions ("`Value`").

### Pick a field, not any field

Once the above dialog is displayed, choose which field (column) that you want to highlight.

![[MS Planner - Conditional coloring - Field list.png]]
*Image: Conditional coloring field list*

The order of the fields in the list seems to be based on the order of the columns in the grid which is a nice touch. It does not include custom fields, maybe they will add that later.

### If this

Once you've picked a field, you need to define the conditions that are used to color the field's background in the Grid. To do that, click the "`Operator`" menu and select one of the menu items: they are fairly logical.

![[MS Planner - Conditional coloring - Operator menu.png]]
*Image: Conditional coloring - Operator menu*

You're almost done.

### Then that

Once you've picked the field and the operator, set a `Value` or a range of values depending on the `Operator` that you chose, and then pick a color. In this example I entered "`5`" for five days.

![[MS Planner - Conditional coloring - Set value to 5 days.png]]
*Image: Set value to 5 days and pick a color with the color chooser*

The `Value` field is pretty forgiving. I entered "`5`" and it set the value to "`5 days`" but you could also start typing "`5 mo`" and it will suggest "`5 months`". Nice work Microsoft.

The result looked like this when I used the blue color.

![[MS Planner - Conditional coloring - blue highlight on Duration.png]]

### Multiple conditions

You can have multiple conditions. For example, if you want to have 1 to 2 week task durations in blue and those between 11 and 50 days in pink. To do this, use the "`+ Add Color`" button.

![[MS Planner - Conditional coloring - Add Color.png]]
*Image: Add another condition using Add Color*

Which results in something like this:

![[MS Planner - Conditional coloring - Grid view with two colors.png]]
*Image: Grid view showing tasks between 5 and 10 days in blue, between 11 and 50 days red*

One use case I thought of for this feature is to color code teams within a project plan, but it doesn't really work. Let me show you why.

### Color coded assignees

I set a condition with tasks assigned to SpongeBob and Patrick to be highlighted yellow like this:

![[MS Planner - Conditional coloring - Assignees.png]]
*Image: Conditional coloring dialog with assigned to equal to SpongeBob and Patrick*

It seemed to work OK, but Planner included tasks assigned to Eugen Krab (EK) which was not what I was expecting but logically it makes sense.

![[MS Planner - Conditional coloring - Assignee Eugen Krabs.png]]

*Image: Grid view showing tasks assigned to SpongeBob and Patrick in yellow background*

So, I added another condition: color tasks assigned to Eugen Krab with the color Blue like by doing this:

![[MS Planner - Conditional coloring - Multiple conditions.png]]
*Image: Conditional coloring adding assigned to Eugen Krabs condition*

To my surprise it overrode the yellow coloring of those tasks assigned to SpongeBob (SS) and Patrick (PS) to now be blue. I guess Eugen is the boss, but I don't think that's why Microsoft Planner did that 😂.

![[MS Planner - Conditional colors - Grid view showing all tasks with Eugen in blue background.png]]
*Image: Grid view showing all tasks with Eugen in blue background*

It seems that I have more to learn about this feature.

### Wrapping up

If you want to shine a light on certain aspects of your Planner plan, try out the conditional coloring feature. You can use it to highlight issues, visualize long duration tasks, or easily see a key person's tasks in your plan.

I can see using this feature temporarily to find anomalies or look at my plans in ways that the filters don't support. But then, I'd likely remove the conditions. You may find other, more permanent, ways to use this feature so please let me know if you do and how you use it!

That's it for this week.

Have a colorful week ahead and **Happy Canada Day!** to fellow Canadians.

Otto.

p.s. sharing is caring so please forward this post to a colleague or a link to [otto-ms.bsky.social](https://bsky.app/profile/otto-ms.bsky.social?ref=planner-ms.ghost.io) or [r/plannerpremium](https://www.reddit.com/r/plannerpremium?ref=planner-ms.ghost.io) so this blog can get to 15 followers.

p.p.s. My Planner Plan 3 trial license expires this week, so I'll need to decide if I pay the $30 monthly to keep the current subscription🤔.

![a red and white Canadian flag on a flagpole](https://images.unsplash.com/photo-1663602533161-b246e5f77e3a?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wxMTc3M3wwfDF8c2VhcmNofDd8fGNhbmFkaWFuJTIwZmxhZ3xlbnwwfHx8fDE3NTExMTc4NjR8MA&ixlib=rb-4.1.0&q=80&w=2000)