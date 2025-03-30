---
tags:
  - post
title: Dependencies in (the new!) Microsoft Planner | LinkedIn
author: ricardo-almeida
url: https://www.linkedin.com/pulse/dependencies-new-microsoft-planner-ricardo-almeida-1nrcf/
date: 2025-03-30
description:
---
# Dependencies in (the new!) Microsoft Planner | LinkedIn

by [Ricardo Almeida](https://www.linkedin.com/in/ricardoalmeida/)

When working on a project, identifying (and managing) the tasks that belong to the critical path of a project helps us evaluate the impact of any change in the overall project's delivery. This topic has been presented in my previous [post](https://www.linkedin.com/pulse/baselines-new-microsoft-planner-ricardo-almeida-8hsef/?trackingId=srD1cZ4%2BRpeSTurgpSAd3Q%3D%3D). This discussion highlights the importance of an accurate appliance of relationships between tasks to ensure realistic planning.

This post presents the definition of the project's dependencies and/or interlinking tasks that you can create in the new Microsoft Planner. Although some presented topics are common terms in project management terminology, they weren't available in the previous Microsoft Planner version. Therefore, I believe it makes sense to include it in this newsletter. With the new Microsoft Planner, you can establish advanced dependencies between your tasks, which will greatly help you create realistic plans tailored to your needs.
### Initial Context

The terminology used in this post is widely known to those who work with project management software. The greatest news is that the new Microsoft Planner also offers advanced task dependency features (like most software for project management), enabling realistic critical path calculations and better priority management! The major principle is that a correct definition of dependencies between tasks allows the automatic project delivery calculation, being always up-to-date on the overall time delivery.

In the new Microsoft Planner, you will find **four dependency types** (which will be described later in this post):

- *Finish-to-Start (FS)* - default
- *Finish-to-Finish (FF)*
- *Start-to-Start (SS)*
- *Start-to-Finish (SF)*

Also, three **delay types** are available to level up the accuracy of your dependencies (and to be applied for each of these four dependency types):

- *Immediate*: no delay or overlap is accepted between tasks;
- *Lead time*: the time you accept a task can start before its predecessor finishes, enabling overlapping;
- *Lag times*: the time which defines a delay between tasks.

The next subchapters present some use cases for these dependency and delay types. I will use the terms first and second tasks, referring to two sequential tasks.

### Finish-to-Start (FS)

Definition: The second task starts as soon as the first task finishes (default dependency type).

Example: In our [previous](https://www.linkedin.com/pulse/baselines-new-microsoft-planner-ricardo-almeida-8hsef/?trackingId=srD1cZ4%2BRpeSTurgpSAd3Q%3D%3D) exercise we have defined that we only receive confirmations after sending all the invitations. In this case, we should select an FS dependency type on the second task, as presented in the image below. Also, by default, the ***Immediate*** option is selected, meaning no delay or overlap is permitted and the second task must start as soon as the previous one finishes.

![[Planner Dependencies - Finish to Start - Immediate.png]]
*Finish-to-Start (FS) with Immediate delay type*

But, imagine you would like to start the second task one day before the first one finishes; in that case, you can define the ***Lead by*** for 1 day. In our example, this means we would accept starting receiving confirmations even without sending all the invitations. The image below presents this configuration and its impact on your Gantt chart.

![[Planner Dependencies - Finish to Start - Lead by.png]]
*Finish-to-Start (FS) with Lead by delay type*

Let's imagine that you send your invitations by mail. You will expect only to receive confirmations after 2 or 3 days of sending the letters. In that case, and for better project planning, you might want to consider that the second task should only start 2 days after the first task finishes; and you can use ***Lag by*** to do this! The image below presents this case and the impact on your Gantt chart.

![[Planner Dependencies - Finish to Start - Lag by.png]]
*Finish-to-Start (FS) with Lag by delay type*
### Finish-to-Finish (FF)

Definition: The second task finishes when the first task finishes.

Example: In our [previous](https://www.linkedin.com/pulse/baselines-new-microsoft-planner-ricardo-almeida-8hsef/?trackingId=i2OkHd86T1KGtZkfgM%2Fmmg%3D%3D) exercise, imagine that receiving the 3 quotations and checking for traffic restrictions can finished on the same date. You can define such a behavior by choosing an FF dependency as shown in the image below.

![[Planner Dependencies - Finish to Finish - Immediate.png]]
*Finish-to-Finish (FF) with Immediate delay type*

You can also use *Lead by* and *Lag by* delays with this dependency type. Just to give you a quick example, if you define *Lead by* for 1 day, it means you accept finishing the second task one day before the first task finishes, as presented in the image below. For the *Lag by* type, the principle is the same as presented before for the FS dependency type. I believe you got the picture;)

![[Planner Dependencies - Finish to Finish - Lead delay.png]]
*Finish-to-Finish (FF) with Lead by delay type*
### Start-to-Start (SS)

Definition: The second task starts when the first task starts.

Example: You can always use this dependency type if you believe two tasks should start on the same date, and this example is presented in the image below. As in the previous dependency types, you can also use *Lead by* and *Lag by* delays.

![[Planner Dependencies - Start-to-Start - SS - with Immediate delay type.png]]
*Start-to-Start (SS) with Immediate delay type*
### Start-to-Finish (SF)

Definition: The second task finishes once the first task has started.

Example: This is not a very common dependency type but let's imagine that you have the following two tasks:

- First task: New ERP system up-running.
- Second task: Shut down the old ERP system;

In this use case, we can only deactivate the old ERP system once the new ERP system is available for users. A graphical example is presented in the image below, although not for this use case; the idea is to share the visual impact on your Gantt chart. As in the previous dependency types, we can use *Lead by* and *Lag by* dlelays.

![[Planner Dependencies - Start-to-Finish - SF - with Immediate delay type.png]]

Start-to-Finish (SF) with Immediate delay type

### Final thoughts

Today, I focused on advanced task dependency for the new Microsoft Planner. As shown, Planner offers major dependency types to apply to your tasks and to help achieve a realistic delivery time for your project. I believe Microsoft Planner has assumed a new role as a truthful project management tool! I hope you are as excited as I am with these new features:)

It's time to update our features table:

![[Feature table - Outlook Tasks - To-Do - Teams - Planner - Planner Premium.png]]

Comparison between Outlook Tasks, Microsoft To-Do, app for Microsoft Teams, Microsoft Planner and Microsoft Planner Premium

Stay tuned!