---
tags:
  - post
url: https://planner-ms.ghost.io/assignments-who-what-when/
date: 2025-07-12
people:
  - otto
service: ghost
---
# Use Assignments in Planner to see who's on what, when

*Discover the assignments feature in Microsoft Planner which can be used to allocate effort per person per task and view that by day, week, month, or year.*

*![[Pasted image 20250712140351.png]]*
*Photo by [Justin Lim](https://unsplash.com/@justinlim?utm_source=ghost&utm_medium=referral&utm_campaign=api-credit) / [Unsplash](https://unsplash.com/?utm_source=ghost&utm_medium=referral&utm_campaign=api-credit)*

Welcome to episode #15 of [my adventure](https://planner-ms.ghost.io/hello-world/) to learn about Microsoft Planner and share some pragmatic project management tips. This episode takes us to the dark corner of the tool but before we go to that dark place, a note of thanks.

💡*Welcome ***Mark*** from Illinois and thanks for joining the club!*

Before describing the assignments feature, I want to look back a bit and then share some personal information.
### Looking back

Reflection is often good, so here's what I've learned and shared so far about Microsoft Planner premium plans:

- The basics including [buckets, tasks, and subtasks](https://planner-ms.ghost.io/buckets-tasks-and-subtasks/)
- [Labels](https://planner-ms.ghost.io/using-labels-in-microsoft-planner/) as another way to categorize work, easy to use
- Tracking [dependencies](https://planner-ms.ghost.io/dependencies-in-microsoft-planner/) within plans was a bit more complicated
- Simpler features like [sharing](https://planner-ms.ghost.io/planner-plans-to-share-or-not-to-share-that-is-the-question/), [filtering](https://planner-ms.ghost.io/microsoft-planner-filters/), and [task history](https://planner-ms.ghost.io/microsoft-planner-task-history/)
- How to track [goals](https://planner-ms.ghost.io/goals-in-microsoft-planner/) was something I likely should've started with 😂
- How to manage [sprints](https://planner-ms.ghost.io/sprints-in-microsoft-planner/), important for Scrum folk
- Assigning single [task owners](https://planner-ms.ghost.io/microsoft-planner-one-or-multiple-task-owners/) instead of multiple
- Using [conditional coloring](https://planner-ms.ghost.io/use-highlights-to-colorr-code-your-microsoft-planner-plan/) because who doesn't like coloring?!
- Tracking [custom information](https://planner-ms.ghost.io/microsoft-planner-custom-fields-of-dreams/) in your plans for your needs

That's a pretty comprehensive list of feature summaries if I do say so and covers a lot of the functionality of the tool. One feature not mentioned so far is the _Assignments_ tab but before getting into that feature, I need to share something.
### People, not Resources

As I get older, I end up with more pet peeves and buttons that can be pushed. These are little annoying things, nothing that I get upset about, just annoying 😂. Here are some of them:

|Peeve|Instead|Why?|
|---|---|---|
|Best Practices|Proven Practices|Best means they can't be improved|
|Periods at the end of bullets.|No periods|If they aren't full sentences, no period.|
|Meetings without agendas|Agendas|So I know what we'll talk about|
|Long email threads|Talk to each other|Resolves issues faster|
|Resources|People|We're people not things|

That last peeve is one that I've had for a long time: calling people "resources" on projects. Why? I find it dehumanizing and I try to avoid using the term, instead using "people". In this post I you'll see the term "Resources" because Microsoft uses the word in the user interface.

OK, now that I've done some reflection and risked telling you some of my buttons, let's head into the main topic.
### Balancing the work

Once you have a lot of tasks defined in your plan and they're assigned to people, you'll find yourself wanting to balance the workload across the team or teams. It's an almost impossible exercise.

Sometimes this activity is referred to as "Resource Balancing". In Microsoft Project Professional a.k.a. Microsoft Project, the feature was called "resource leveling" and the leveling can be manual or automatic.

What I found with Microsoft Project's automatic leveling was the schedule would go completely out of whack because the tool moves tasks around based on a person's other assignments. So, I'd disable automated leveling and modify the dates on tasks manually 🤦‍♂️.

This was madness and I avoided using the automated leveling feature. In Project, you could specify what percentage a person works on a task which helped a bit – Planner doesn't support that.

The balancing activity is always a challenge especially in environments where there's unplanned work in the form of operational issues, executive requests, or new regulations.

On projects that have a lot of standard work with strict Service Level Agreements (SLAs) between groups and tasks with well known durations, "resource" balancing may work. For information work, the task durations are often variable and unpredictable.

💡*Always check with the person, their team lead, or manager directly to confirm they're reserved and commit to doing the work.*

People won't be available when you need them just because your plan says so, make sure to confirm/check.

How does the Assignments feature work in Planner?
### Assignments

You get the Assignments feature in Microsoft Planner premium plans – those with a Plan 3 or above license – and here's where to find it:

1. Click "`Assignments`" tab
2. You'll see "`Group by Resource`"
3. The person's name is bolded on the left under the "`Assigned to`" column

![[MS Planner - Assignments - Group by Resource.png]]
*Assignments view showing Group by Resource and resulting table*

### Entering effort

To the right of the "`Effort`" column you'll see additional columns for each Day, Week, Month, Year where you can enter values.

In this example, I changed the "`Free Krabby Patty Slider to the first 10 customers`" task to require 3 hours on April 25, 2025.

![[MS Planner - Assignments - set value.png]]

*Assignments view with 3 typed in a cell*

If you're at the week, month, or year level and enter a value, Planner will equally distribute the effort across all of the days within the time period, i.e. between the "`Start`" and "`Finish`" dates.

### Zoom in and out

With the Assignments view you can get a good overview of what people are assigned to by zooming out to the weekly, monthly, or yearly level. To do that click the "`Daily`" button and change it:

![[MS Planner - Assignments - timeframe menu.png]]
*Assignments view showing the timeframe menu displayed*

In any of those timeframe settings you can edit the allocations for each person at the task level by clicking in the day/week/month/year cell and entering a value.

Planner only lets you enter values in the cells that are between the "`Start` " and "`Finish`" boundaries which makes sense. It took me a minute to figure that out because there's no warning in the user interface.

### Other features

In the Assignments view, you can move around in time or change the view to group by task.

**Time travelling**

In case you don't see it, these two arrows allow you to move back and forward in time:

![[MS Planner - Assignments navigation.png]]
*Assignments navigation: arrows left and right*

**Group by Task**

To change the view by Task click here and set it to "`Group by Task`":

![[MS Planner - Assignments - Group by Task.png]]
*Assignments view showing Group by Task*

### Why dark side?

I used the term dark side at the top of this post because the Assignments feature in Planner seems to be half-baked:

1. The "`Filter by keyword`" search doesn't seem to filter anything
2. There's no way to edit a task in this view
3. You can't resize the column widths
4. You can't sort by any of the columns
5. The "`Group by Task`" option is not very useful (to me)

### Not to leave on a bad note

One final note about how this feature fits in Planner. There's a correlation between the _Assignments_ tab and the _People_ tabs – they're two sides of the same coin, showing Task assignments from different perspectives.

The _Assignments view_ shows tasks by resource or assignment which is useful to see _who is working on what._

The _People view_ shows people and their assigned tasks which is useful for _managing current individual workloads._

### Nothing here, move on!

I've described the Assignments feature in Planner premium plans, those requiring a Plan 3 or above license. It will be useful if you're looking at forwarding on how people are allocated to work tasks. You can set effort on a task-level at either the daily, weekly, monthly or yearly level.

I hope this post has helped you. Your assignments, shall you accept them:

![[MS Planner - Assignments - Your assignments.png]]
*your assignments: have a great week ahead and try the Assignments feature!*

I don't mind making mistakes so you can help validate my learning by letting me know of any errors or major omissions.

Thanks,

Otto.

p.s. please forward to someone or "like" my posts on [BlueSky](https://otto-ms.bsky.social/?ref=planner-ms.ghost.io) or [Reddit](https://www.reddit.com/r/plannerpremium/?ref=planner-ms.ghost.io)