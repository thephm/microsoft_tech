---
tags: [video]
url: https://www.youtube.com/watch?v=HvFEz_2OZB0
slug: daniel-anderson
organizations: [null]

date: 2023-04-04
duration: 11:34
---

# Tasks in Microsoft Loop

https://www.linkedin.com/posts/danielando_microsoft-loop-built-for-modern-task-management-activity-7056184699538313216-OOlt?utm_source=share&utm_medium=member_desktop

## References

1. [Microsoft Loop - Built for Modern Task Management](https://youtu.be/HvFEz_2OZB0) by [[Daniel Anderson]] 2023-04-04
2. [Microsoft Loop Tasks](https://youtu.be/YLpH9sGqlbg) - Where did they go?

## Tasks Loop Component

In this example, the Tasks are added into a Microsoft Loop workspace called `Meeting Notes`. 

> [!tip]
> The name of the workspace should be more descriptive. If we use `Meeting Notes`  it doesn't provide any context of which project it's on

### Add tasks to Loop

In a Loop workspace, create a Tasks list by doing the following

1. Use "`/`" to display the context menu
2. Under `Templates`  choose `Task list`
![[Microsoft Loop - Add Task list.png|300]]

Three columns are shown: `Task`, `Assinged to`, `Due date` which can be sorted, hidden, or expanded using these buttons:

![[Microsoft Loop - Tasks component options.png]]

### @ assign someone a task

People aren't notified if they're not in the Loop workspace, but you can grant them access (share) and notify

### Email notification

This is what the assignee sees in email notification:

![[Microsoft Loop - Task assigned email notification.png|500]]

## Where do the tasks live?

The Tasks are created as a new MS Planner Plan in a bucket called `Tasks`.

> [!question] Question
> What happens when I move a task to another bucket in Planner, how does it show up (or not) in Loop?

## See and edit tasks in Teams

The Tasks can be then be seen in [[Microsoft Teams]]. This screenshot assumes you pinned the `Tasks by Planner` in the Teams' sidebar / "rail" on the left.

1. Click `Tasks by Planner`
2. Click `Assigned to me`
3. You'll see the source `Meeting Notes` and `Microsoft Loop` for context on where it was created
4. Click the title e.g. "Gather resources" and the task is opened right inside teams. You can see the source "Meeting Notes" and context of where it came from "Microsoft Loop" 

![[Microsoft Loop Tasks in Teams.png]]

## Manipulate tasks

Right click on the task to add it to `My Day` or perform other functions. Tasks marked completed here show as ~~strikehtrough~~ done in MS Loop.

![[Microsoft Loop - Task menu.png]]

### Create a Loop Component from the Tasks List

Create a Loop component of the task list by

1. Clicking the Bento Menu (9 dots) just under `Tasks`
2. Click the copy icon
3. Click `Copy` button

![[Microsoft Loop - Create Task List Component.png]]

### Share the component in Teams

Paste the URL in a Teams Chat and a live instance of the task list is displayed with context "Meeting Notes Component"

![[Microsoft Loop - paste URL to Tasks component in Teams.png]]

> [!question] Question
> Why are the two `Assigned to` people red in this screen

### Share the component in Outlook

Paste the same URL it into MS Outlook email and it becomes a live task list in someone's email inbox.

![[Microsoft Loop - Paste URL to Tasks Component into Outlook.png]]

> [!question] Question
> Can I create a loop of Just Alex's tasks? 