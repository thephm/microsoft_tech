---
tags:
  - post
url: https://planner-ms.ghost.io/dependencies-in-microsoft-planner/
date: 2025-05-11
people: otto
service: ghost
---
# Tracking Dependencies in Microsoft Planner Premium

> Master dependencies in Microsoft Planner Premium and take control of your project timelines.

Welcome back to another episode in [my series](https://planner-ms.ghost.io/hello-world/) of posts on Microsoft Planner Professional a.k.a. Project for the web. This week, I had a huge influx of no – zero, nadda, nul, nilch – new subscribers. The overwhelming volume of interest has me verklempt and inspires me to continue with my favorite topic: dependencies.

Un-managed dependencies kill projects especially those outside of your span of control. I've seen this happen many times in my career. Often, these killer dependencies were a result of some assumption that was made but not flushed out nor verified.

A boss many years ago explained to me what you need to define a dependency: **on who, for what, by when**. If you're missing one of those, you don't have a fully qualified dependency. It's stuck with me to this day.

Managing dependencies is a key aspect of Microsoft Planner Premium that many users struggle with. When tasks depend on each other, your project timeline can quickly become complicated. In Planner Premium, you can create and track dependencies directly within your schedules, giving you greater understanding over how the work flows.

In this post, I’ll show you how to add task dependencies in Planner Premium and explain a few use cases to help you take full advantage of this powerful feature.

## What are task dependencies?

It depends. Just kidding! A **task dependency** means that one task depends on the completion of another task before it can start or finish. This helps you:

- Sequence work logically
- Avoid scheduling conflicts
- Spot bottlenecks before they become issues

Here are a few simple examples of dependencies:

- **Marketing Campaigns**: “Design assets” must be completed before we “Launch social ads”.
- **Software Development**: “Complete backend API endpoint” must start for a month before we “Start frontend integration”
- **Event Planning**: We need to “Secure the venue” before we “Send out invitations”

In project management and in Project Professional, the terms predecessor and successor are often used. With Planner Premium, the terminology is different:

- **Depends on** are tasks that occur before this task.
- **Dependents (after)** are tasks that occur after this task.

We've talked about the basics of dependencies and things get a little harrier when intricacies within the work exist which is almost always the case on non-trivial projects!

### Refining the Dependencies

Planner Premium offers four ways to categorize a dependency; they call this **Dependency type**:

- **`Finish to Start`**: The most common, where Task B can't start until Task A finishes
- **`Start to Start`**: Task B can't start until Task A starts
- **`Finish to Finish`**: Task B can't finish until Task A finishes
- **`Start to Finish`**: Task B can't finish until Task A starts which is rare

That's enough to get started now let's create a dependency. Before you get started, you’ll need a **Project Plan** created in **Planner Premium** (Plan 3 license). If you're not sure which version of Planner you have, check with your IT department because this feature does not exist in Planner Basic (Plan 1 license).

## Adding a dependency between Tasks

Just like every other tool Microsoft creates, there are multiple ways to accomplish the same thing. That can be both frustrating and handy. I'll first show you how to create dependencies from within the task details and then how you'll likely end up doing it most often from Grid view. The pain before the pleasure.

### Adding a dependency within Task Details

1. **Open your plan** in [Microsoft Planner Premium](https://project.microsoft.com/?ref=planner-ms.ghost.io).
2. If not already in the Grid view, click the **Grid** tab.
3. Click the **`"i"`** icon to display the task details on the task which has a dependency.
4. Click **`Add dependency`** button under **Depends on**
5. Type the name or select the task you want to make the successor.
6. **Save** your changes.

![](https://planner-ms.ghost.io/content/images/2025/05/image-2.png)

Add dependency in task details

OK, here's where we get even more flexibility when creating dependencies. Hold on because this next part is also very important.

### Specifying delay

We skipped over one important feature. Once you click the **`Add dependency`** button, a few fields are displayed including **Dependency type** which was described above:

![](https://planner-ms.ghost.io/content/images/2025/05/image-5.png)

Depends on settings

The additional option of **Delay type** gives you more control rather than just hard start and finish dependencies. You can specify an additional constraint to allow things like "Task B depends on Task A starting but a week later" using **`Lag by`** or "Task B depends on Task A finishing but a week before" using **`Lead by`**. Choose one of those options and then specify how many days in the **`Span`** field.

Clicking `Add dependency` from within a task's details was one way to add dependencies. Another way, which I use most, is from the Grid view. It's a lot faster and you don't have to display each task.

### Adding dependencies within Grid view

Surprisingly, by default the dependency columns are not visible in the Grid view, so first you need to add them. To do that use **+ Add column** and choose **`Depends on`** and **`Dependents (after)`.**

![](https://planner-ms.ghost.io/content/images/2025/05/image-4.png)

Add dependency columns in Grid view

The two columns are added to the grid and then you can drag and drop them wherever you prefer. To add a dependency, double-click on the corresponding **Depends on** cell for the task and Planner will suggest some potential dependency tasks.

![](https://planner-ms.ghost.io/content/images/2025/05/image-6.png)

Adding a dependency in Grid view

Alternately, you can start typing the name of the task and it will show you the matching tasks with the Task Name that you typed.

🤯

To impress your co-workers, there's a faster way to add a dependency! In the ****Depends on**** field, type `3FF` and press `<Enter>` and that creates a dependency on task `3` with a `Finish to Finish (FF)` type.

### Lead and lag time

This part is tricky to see, but the little button "**`| >`**" to the right of the suggested task displays this dialog.

![](https://planner-ms.ghost.io/content/images/2025/05/image-7.png)

Dependency type in Task details

This dialog is handy if you're learning about the types of dependencies because it shows you a visualization and provides a little explanation. In the screenshot above you'll see how `Task 4` depends on `Task 3` and just below the image it says "Task 4 can only start once task 3 finishes" because the `Finish to Start FS` option is selected.

If you choose **Delay type** and set a **Span** value, the image and text tip changes, that's pretty cool!

![](https://planner-ms.ghost.io/content/images/2025/05/image-8.png)

Lag by and Lead by values

### One last way to add a dependency

Lastly, in **Timeline view**, you can click and drag a line from one task’s end to the start of another. This is a fun way to create dependencies, but I don't think I'll use it that often.

![](https://planner-ms.ghost.io/content/images/2025/05/image-10.png)

Planner Premium automatically reflects dependencies in the **Timeline View** but on **Task cards** there's no visual indicator to show a task has dependencies or dependents. You have to click on the Task and look at the “Depends on” section to see any linked tasks. This is a `#fail`.

Now that you know how to create dependencies in Planner Premium, a few things to keep an eye out for.

## Troubleshooting common dependency issues

There are many issues that you may run into when managing dependencies including hidden or circular dependencies, done but not done tasks, too many dependencies, or stale dependencies.

Here are some of the potential challenges and ideas on how to solve or avoid them in the first place.

### Hidden Dependencies

**Problem**: Team members are surprised by dependencies they didn't know existed. That never happens! 😂

**Solution**: Implement a dependency review as part of your regular team meetings. Have each team member verbally confirm they understand their task dependencies. Ask them "What do you need to finish your work?" then follow-up with "From whom?" and "By when?".

### Uncommitted Dependencies

**Problem**: Task B depends on Task A which ends up delayed because the owner of Task A never truly committed to delivering it by the date that you put in your schedule.

**Solution**: As soon as the dependency is identified, work hard to get the right owner of the Task and obtain their commitment to deliver on a specific date. This is very, very hard. Ask them for their confidence level as time progresses. Ask if they depend on anything or anyone else! Then, once you have their commitment, follow-up regularly on their progress and periodically re-confirm their commitment to the due date.

### Incomplete Dependencies

**Problem**: Task B depends on Task A which ends up finishing but it Task A didn't deliver what was really needed.

**Solution**: As soon as the dependency is identified, define what is needed and discuss it with the person delivering Task A. Agree on what it means to be complete a.k.a the Definition of Done: fully tested with automated tests all passing in dedicated production-like test environment, well documented, etc. If Task A is delivering a significant piece of work, specify the acceptance criteria so it's clear that the dependent person/Task B owner gets what they really need. You will be glad you spent the time up front.

### Circular Dependencies

**Problem**: Task C depends on Task B, which depends on Task A, which depends on Task C. These are lethal.

**Solution**: Identify circular dependencies through mapping exercises. Break the circle by determining which task truly needs to come first or by breaking a task into smaller components.

### Too many dependencies

**Problem**: Over-dependence creates bottlenecks where everyone is waiting on everyone else.

**Solution**: Challenge each dependency. Ask "Is this a true dependency or just a preference?" Consider whether tasks can be partially completed or run in parallel. Find creative ways to emulate something that is being created in parallel until it's ready to be integrated.

### Out of date Dependencies

**Problem**: As projects evolve, documented dependencies become outdated.

**Solution**: Schedule regular "dependency cleanup" sessions to review all of dependency relationships and update or remove them as needed. For big dependencies, track a separate risk in your Risk Log so it gets the attention it deserves. Talk about dependencies often, you won't regret it.

## Advanced techniques

Here are a few ideas to pique your interest in additional ways to manage and track dependencies in Planner Premium. I'd love to hear other tips and tricks that you use.

### Labels , buckets and filters

- Combine dependencies with **task** [**labels**](https://planner-ms.ghost.io/using-labels-in-microsoft-planner/), **priorities**, and [**buckets**](https://planner-ms.ghost.io/buckets-tasks-and-subtasks/) to fine-tune your workflow.
- Use **filters** to view high priority tasks that are blocking others or are currently blocked by using a "blocked" label. You can also filter on `Critical Path` Tasks in many views.
- Consider using **milestones** alongside dependencies for higher-level planning. Milestones are zero-duration (start and finish on the same day) Tasks in your schedule.

### Critical Path analysis

Even with the basic critical path feature in Microsoft Planner Premium, you can identify the sequence of the key dependent tasks which determine your project's minimum possible duration. Here's where you can enable that in the **Timeline** view.

![](https://planner-ms.ghost.io/content/images/2025/05/image-9.png)

Show Critical Path in Filter Tasks

### Dependency buffers

Build buffer time into your schedules by first identifying the high-risk dependency relationships. Add buffer time between the expected completion of predecessor tasks and the scheduled start of successor tasks by explicitly adding buffer tasks. Use this buffer time for quality checks and handoffs. Some leaders won't like seeing explicit buffer tasks but don't let that stop you.

## Final thoughts

Task dependencies bring **structure and foresight** to your project timelines. While simple in concept, they’re incredibly effective for aligning teams and preventing delays. With Planner Premium, you can manage and track dependencies without needing to leave the Microsoft 365 or using legacy tools like Project Professional (aka Project Desktop).

**Until next time, keep planning and keep smiling!**

_p.s. this post was written by me, myself and AI_