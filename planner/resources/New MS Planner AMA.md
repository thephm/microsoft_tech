---
tags:
  - chat
people: 800
topic: New MS Planner AMA
date: 2024-04-04
url: https://aka.ms/NewPlanner/AMA
time: 13:00
service: youtube
---

# New MS Planner AMA

![|150](https://statics.retailservices.teams.cdn.office.net/ui/static/releases/uno/all/assets/planner2.8e27f89bc2da530d3b02.svg)

This is the [Recording](https://aka.ms/NewPlanner/AMA)

## Links

- [The new Planner in Teams is now in Public Preview](https://techcommunity.microsoft.com/t5/planner-blog/the-new-planner-in-teams-is-now-in-public-preview/ba-p/4072525)
- [Licensing](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description)
- [Feedback portal](https://aka.ms/plannerfeedback)
- [FAQ](https://aka.ms/newplannerfaq)
- [The new Microsoft Planner begins roll out to General Availability](https://techcommunity.microsoft.com/t5/planner-blog/the-new-microsoft-planner-begins-roll-out-to-general/ba-p/4101056) by Roberto Bojorquez
# From the call

> Users don't need to where the data is stored

- OMG that ^ made me LOL!

- Basic [plan] is managed in Planner. Premium in [[Dataverse]] and To do in To Do

- Better support for Sprints in hybrid project e.g. waterfall

- Power Automate for new Planner. Any plans 1, 3, or 5 can build apps without additional power automate license

- Templates? No, copy plan. With CoPilot can create it for you!

- Copilot: Create a plan, add goals, answer what's the status of the plan? What are the overdue tasks this week?

- Guests: added guest user at the tenant level then the plan, can edit plan, complete plan. They don't get timeline and gantt. 

- Premium features like baselining are being worked on and portfolios. Won't be in basic plans.

- Project for the web bringing into Planner in Teams. Will bring to the Web later

- Actively working on bringing Project online and Project desktop features to New Planner as premium features e.g. Baseline and portfolios

- MS notifies Admins ahead via "MC posts" 3 days ahead. Rollout through rings first internally, then technology programs (TAP), then private previews, then public previews 

- Can I delete a task or plan? There is a way, hard to find. My plans breadcrumb, click name of plan, plan details at the bottom is Delete option.

- Recover a plan? Not yet, it's in the backlog aka "Recycle bin"

- Roadmap feature for Project for the web: not much change in roadmaps? "Add roadmaps in Teams as a tab continues to work. In New Planner have not enabled roadmaps yet as we are actively  working to enhance the roadmap capability to make it a portfolio solution"

---

# From the questions

DISCLAIMER: I've captured most of the questions and answers here minus the questions not answered and minus some I didn't care much about. I also remove some of the pleasantries or @ mentions by the respondents.

## Accelerator questions

Colin Craig

> How does this impact project accelerator? We've needed to deploy accelerator for its functionality. However, it appears like baselines and portfolio management are part of the upcoming releases. Do I need to plan an accelerator rollback?

Brian Smith (CSS), Microsoft

> ==There will certainly be new features coming that could replace some of the capabilities currently delivered with the Accelerator==, and also for many customers and partners the Accelerator has just been a starting point. As the new features come along, I would suggest getting into the previews to understand how things might need to change if you have any custom solution applied - not just the Accelerator. New Planner doesn't impact anything here though.

---

Cody Olson

> Hey there! Does this new version of Planner incorporate the P4W Accelerator? It has been a headache needing to constantly copy over all the tasks/to do's into a second area. I like the idea of having project, planner, and to-do all connected, but I have found very little info regarding if this also covers the accelerator version of P4W. Looking forward to the meeting on April 4th!

[[Brian Smith]] (CSS), Microsoft
 
> It doesn't directly, but if you have the Accelerator also loaded in your default Dataverse environment then any plan tasks assigned will show up in new Planner. If you have the accelerator in named environments then this will be supported at a later date.

Colin Craig 
 
> I'm also curious about this! We've needed to deploy accelerator for its functionality. However, it appears like baselines and portfolio management are part of the upcoming releases. Do I need to plan an accelerator rollback?

Brian Smith (CSS), Microsoft
 
> You certainly may need to consider if some of the Accelerator capabilities are still needed once features like portfolio come along - but I feel it will be more of a trim back than roll back.

---

[[Yvonne Esch]]

> We're heavy users of the Microsoft PMO Accelerator with Project for the Web. 1) What are the plans for integrating the functionality of the PMO Accelerator and the Resource Scheduling app into the new Project/Planner app? 2) What will happen to customizations we've deployed as custom solutions layered onto the PMO Accelerator/Project for the Web?

---

## General

Laura Gariano

> The features users want the most are the same Planner improvements that have been requested for the past several years: ==At-mentioning in comments, Task dependencies, Reminder date/times (like ToDo offered), Notifications in the tool vs. email only, Checklist item assignments/due dates, Manager oversight to tasks for individuals==, Roles in Planner that diversify what various users can do in the Plan, recycle bin, etc. We see these questions in the posts below, but it feels like these core functionality items are being ignored in lieu of Copilot and Premium licenses.

Maureen Mullen

> Agreed. I've started a new job that only uses Microsoft products and we need a task/small projects manager. I was going to start using the Lists app because its functions are more what my team needs, even if it means I need to spend more time building it out on the front end. I was excited to see that Planner was getting an update and so I've been holding off on Lists and waiting to see if they'd be incorporating the Lists functions, but so far, I'm not seeing the draw to Planner. ==Seems like Lists is still the better option... (and it's still not exactly what I need, but given the Microsoft options)==

Alexis Green

> Totally agree with this! You honestly listed out the important BASIC functionalities needed for tech owners to suggest Planner OVER other tools. I'd also add the feature of sharing a plan with individuals without having to create an O365 group or simply adding "guests" to plans. The ability to work cross-functionally is critical to business use and we don't want to have to manage unnecessary O365 groups.

---

Brandon Sullivan 

> Apologies if this is already asked, but it seems like the change is really just: ==Basic Plan = Legacy Microsoft Planner== [and] ==Premium Plan = Project for the Web== renamed I don't see any features combined in them, for example, a Premium plan doesn't support recurring tasks, but a Basic plan does. So it's just a rebrand/name change and Teams app?

Stephen Thoms

> I'm worried about migrating all my [[Project for the Web|Project for Web]] plans over to Planner Premium. I hope MS is planning a migration strategy.

---

## Resource management and team tasks

Stephen Thoms

> I'd love to hear about the roadmaps to these products also. Robust Project and Portfolio planning tools are being pushed to the side as Microsoft focus on small time, agile tools like Loop and Planner. MS is neglecting advanced project management tools. ==Resource Management no longer part of Project, you need a technical resource to install a Power BI add-on and it seems more geared towards Dynamics (Project For Web seems to be an after thought)==. All this makes us wonder where our we should focus our energy next with new tools.

---

Mark Wonsil

> Will Managers be able to view the tasks of their team?

Ian Bruckner

>This is a big ask from my org. They want resource/line mangers to see the tasks their matrixed staff in projects have been assigned (alongside tasks they assign themselves as managers)... and further, they want to also see those tasks in context of the projects without having to be on every. single. team.

---

Mark Ellestad

How can I link work/tasks/projects to a portfolio, so that we can balance resources across teams, make enterprise reporting, stuff like that?

Stephen Thoms

> I have the same concerns, Resource Management appears to be a missing feature across [[Project for the Web]] and [[Microsoft Planner|Planner]] Premium.'

---

immrted1966

> I am really interested in Resource Management. I need a overall look at all production staff and what projects they are working on

Brian-Smith (CSS), Microsoft

> The deeper resource management capabilities of Project for the web aren't exposed in new Planner at this point
 
immrted1966

> [this article](https://learn.microsoft.com/en-us/project-for-the-web/overview-universal-resource-scheduling) will help you understand what is already available via the [[Power Apps]] interface 

---

Stephen Thoms

> What's the roadmap for Resource Management for [[Project for the Web]]/Planner Premium? I find it difficult to workload level across projects and understand how busy folks are going to be based on estimated budget hours. Also, need have better reporting on Actual burn rates vs original Forecasts

Brian Smith (CSS), Microsoft

> you may already be familiar with the universal resource sheduling capabilities detailed [here](https://learn.microsoft.com/en-us/project-for-the-web/overview-universal-resource-scheduling) but if there is more you need be sure to [give us feedback](https://feedbackportal.microsoft.com/feedback/forum/40792262-301c-ec11-b6e7-0022481f8472) 

---

Jeanne Darche
 
> Will there be functionality to see human resources occupancy rate? Like how much of employee 1's time is already booked in total? Overall, not just on one project. Right now: - We can only see occupancy for one project at a time - We can add time for a task and add it to an employee, but the total for the employee also includes done tasks! We have no way to filter down to eliminate done tasks for the total.

Brian Smith (CSS), Microsoft

> [[Project for the Web]] used in the [[Dataverse]] has resource management capabilities, but ==no immediate plans to expose this in new Planner==, although the tasks from those plans from the default environment will be in the resources 'My Tasks'.

---

Yannick Lamarre 
 
> Is it possible to have a global view of tasks by resource? Example, I have 8 active projects. In the morning, I want to be able to see which tasks resource A and resource B are working on and in which of my projects. I'm looking for a cross-sectional view of all tasks by resource or priority.

Courtney Svoboda 

> Yes, please make this happen, without having to create a Power BI dashboard. Should be native within the system.

---

## Notifications

Bruce Kraft Jr

> Nnoooo! Having to rely on teams for a notification queue is not the way to go!!! The teams notification is ALREADY cluttered Plus there are some companies who don’t want to and refuse to use teams Using teams to get a full list of tasks activity is not positioning planner as a stand alone solution! This decision will only drive more people towards clickup! Besides, planner having their own notification queue will help us stay organized when it pertains to TASKS AND COMMENT-RELATED TASKS-BASED NOTIFICATIONS ALONE… We SHOULD NOT BE FORCED TO USE TEAMS FOR A NOTIFICATION QUEUE!!

---

Bailey Souza

> When the Planner and Project integration happens, will Project tasks automatically be added to each users planner? Will the new Planner notify users when tasks are due and overdue? Lastly, will there be an option to add subtasks within an open task, or will it only be available through the Project "Grid" view?

Brian Smith (CSS), Microsoft

> Assignments from premium plans (Projects) in the default [[Dataverse]] will show up in the users My Tasks and My Day as appropriate Bailey. Notifications will also be unified across the plans. I like the idea of being able to add subtasks from the task itself, rather than having to use the grid (which you need to do today) - be sure to give us that feedback over at https://feedbackportal.microsoft.com/feedback/forum/a1a93b69-2f1c-ec11-b6e7-0022481f8472 too so others can vote on it. Copilot will also be able to 'indent tasks' and I think some of these types of commands, which seem trivial, will soon become a common way of interacting with the plan - as they can be used regardless of the view you are in.

---

Jerry Dolezal

> When having Tasks are setup with dependency will there be a notification to the assigned users once the FS dependency are completed? Or will we need to setup a power automate flow to make a notification?

Biatrice Ambrosa, Microsoft

> We do not currently have notifications for completed dependencies. Thank you for bringing this to our attention. I could see how they would be useful for both completion as well as slippage.

---

## email / Outlook integration

Jessica Perkins

> Any plan to support creating a planner card from email/Outlook, similar to create a task functionality? Or at minimum have the mail tasks visible in Planner, similar to To Do?

David Rhoads

> The ability to interact with email is important to our organization. Even as we move our workflow towards Teams, email will remain the way we interact with users outside our organization. With that in mind, I have 2 questions: 1. As Jessica Perkins writes above, will we have the capability to email tasks to a planner board? Currently, the only way to do this is to send an email to a Teams Channel and create the tasks manually from the channel 2. Is it possible to receive email notifications off a task? And if so, is it possible to specify who receives these notifications (as in can you @mention specific users or only send a comment to everyone assigned to the task). We are a "hybrid" organization in that we haven't fully transitioned to Microsoft 365, but the two factors above are pushing us towards licensing Trello. I'm hoping the new Planner can solve these natively, as the Teams-native functionality seems pretty great!

sastocky

> Yes! This is what is needed when receiving a task via email or sending a task via email. Then the ability to provide automatic follow-up based on a provided date or the completion date of the planner task/card.

---

Rich Lus

> Will the new Planner allow for the option to not create an email address when a new Planner is setup? If not, how do I remove the email addresses it sets up? My clients don't need email addresses for each project and worse the email addresses are flooding the address book and it can be annoying. Yes, I've tried not having them appear in the GAL but they end up reappearing anyway.

Laura Becker, Microsoft

> When a user shares a plan, it is either shared with an existing M365 group, or a new M365 group is created. The email addresses are for the group, and not for the plan. Thank you.

---

## Guest access

Mark Kashman, Microsoft

> [This is the Project guests article](https://techcommunity.microsoft.com/t5/project-blog/guest-access-now-av) Roberto mentioned, "Guest access now available in Project for the Web!"

---

Occasional Reader

> How will plans work across tenants? - if I have my work plan, my plan as a guest in client 1 tenant, plan as guest in client 3 tenant.

 Nancy Wang, Microsoft

> Users will have access to the functionality dictated by their license - for guests, you can see the full list of capabilities based on license [here](https://support.microsoft.com/en-us/office/let-guests-see-your-project-in-project-for-the-web-81e1c210-74b2-4711-98ab-dea58f1b566b).  For more info feel free to check our [service description](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description)

---

[Ellen Buwalda / Level Next](https://techcommunity.microsoft.com/t5/user/viewprofilepage/user-id/1508647)
 
> It is possible for guests/externals to collaborate in a Planner without being members of a Teams team

Charlie Tran, Microsoft

> A user must be part of the Teams team associated with the plan in order to access the plan - so yes any guests or external users would need to be a member of the Teams team.

Damon Pettitt

> what if the guest has a Project license in their own tenant? Do they get to see Gant charts, etc. from this host tenant? Or do they need to be "premium" licensed in the host tenant as well?

Nancy Wang, Microsoft

> Yes, if a guest has a Project license they can access premium functionality from the host tenant. See our documentation for more [details](https://support.microsoft.com/en-us/office/let-guests-see-your-project-in-project-for-the-web-81e1c210-74b2-4711-98ab-dea58f1b566b). 

---

Alan Lee

> If I subscrible to premium plan and create gantt chart and other related premium features, can I share the gantt chart or other content created under premium plan to colleagues or external users who doesn't have premium subscription?
 
> To clarify further, my colleagues and external users can edit and collaborate in my premium content (ie. gantt charts) that I create without all of them subscribing to a premium subscription? Thanks in advance for the clarification and I just want to make sure that premium subscription is needed for the project managers only who create the Gantt chart, but not the users, collobrator or contributors who access or edit gantt chart. It would be way too expensive if all people who see, touch, or edit gantt chart need a premium license.

Nancy Wang, Microsoft
 
> Sorry to be the bearer of bad news, it's actually not possible for users without premium licenses to access premium functionality ‌‌:( These users can access the same capabilities they have in basic plans, for example updating a task's title, start date, or priority. You can see the full set of capabilities offered by each license in our [service description](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description). 

---

Damon Pettit

> Can someone who's not in your tenant interact with tasks that you assign?

Tarkan Sevilmis, Microsoft

> You can add people from outside of your tenant and guest users and assign tasks to them. They will be able to work with the task as regular users. There is additional information [here](https://support.microsoft.com/en-us/office/guest-access-in-microsoft-planner-cc5d7f96-dced-4da4-ab62-08c72d9759c6)

---

Blake Daniels 

> Are there plans to implement read-only, edit, owner level permissions to plans / projects? Would improve the business use-case drastically.

Nancy Wang, Microsoft

> This is something we're looking into - do you have any examples of how you would use this sort of feature in your plans and projects? Thanks for your feedback Blake!'

---

Tanya Keyser

> Will there be the ability to lock a Plan or modify Permissions to View Only or Contribute only? What about a recycle bin or version control for task items?

Andreas Backlund

> Must have features. Especially for Front Line Workers. Everyone can edit and delete tasks or the whole Plan without possibility to restore. Really?

---

## Licensing

Biatrice Ambrosa, Microsoft

> [this page](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description) has more information on the capabilities available for each subscription

---

Priscila Marciano

> My company has E5 + P3 Plan. Do we still need to have the Premium license to have these updates?

Lauran Becker

> Yes. You will have access with your current P3 license automaticallly. https://aka.ms/newplannerfaq

---

Jaime Chavez
 
> When will we be able to migrate an existing Standard Plan to Premium Plan?

Brian-Smith

> Yes, that will be coming to new Planner. You can already do this from the existing Planner web tasks.office.com endpoint using the Copy Plan to Project option. The best part is the licensing for M365 users ensures they can carry on participating in the plan once it 'goes premium'.

---

Maxime Belanger
 
> I have access to [[Tasks by Planner]]and [[To Do]] in Teams. How do I know if my enterprise license has the new Planner, and which 'version' of Planner and will have, without having to ask the company?

Cindy Lewis

> When you add an app in Teams, see if you have "Planner". It actually gives you a nice introduction screen so you know it is the new Planner. [This](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/microsoft-planner-service-description) or [this](https://techcommunity.microsoft.com/t5/project-blog/enhanced-collaboration-in-project-for-the-web-with-your/ba-p/4076639) are good sources to learn about the enterprise plans. Welcome to Planner screen

---

Raul Silva Soares

> My question is what will be the users' perspective and the functionalities they currently have access to on the planner via Microsoft 365 in relation to premium plans and other plans, since we don't have that division today?

Robyn Guarriello, Microsoft
 
> with a Microsoft 365 license, you will have access to basic plans, which include all of the same functionalities you currently have access to with Planner! Premium plans require a Planner Plan 1, Project Plan 3, or Project Plan 5 license.

Nancy Wang, Microsoft

> Adding onto what Robyn shared, Microsoft 365 licensed users can also collaborate on premium plans. They can access the same capabilities they have in basic plans in premium plans, such as the ability to update task priority, task name, or task assignee. See our [documentation](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description) for more info.

---

Wyatt Mickelsen

> Do you only get to see the "Premium" plans after you have a project plan license?

Laura Becker

> Basic plans are available with an E3 or E5 Microsoft license. For Premium plans, you will need a paid license to experience the premium capabilities. You can share premium plans with those that do not have a premium license.

Howard Crow, Microsoft

> Just to be really clear - M365 users can see all plans (if they are given permissions) - but they will only see 'basic features' in premium plans. hope that helps.

Nancy Wang, Microsoft

> Just to be really *really* clear :D - here's the [service description](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description) that shows the capabilities available in premium plans based on your license. And like Howard said, basic plans are available to all Microsoft 365 licensed users not just E3 and E5.

---

Beth Purnell

> Will there be a Planner Premium plan (not Project)? Much like there is Teams Premium? Perhaps not all the bells & whistles of Project but some of the upgrades like sub-tasks

Brian Smith (CSS), Microsoft
 
> Project Plan 1 was renamed to Planner Plan 1 - and this would get you some of the bells and whistles - more with Project Plan 3 and 5. Does this help, or are you looking for something less than Plan 1?

---

Rich Lusk

> Is Planner Premium included in Microsoft 365 Business Premium

Nancy Wang, Microsoft

> No, you would need to separately purchase a Project Plan 1, 3 or 5 license in order to access Planner Premium: https://www.microsoft.com/en-us/microsoft-365/project/compare-microsoft-project-management-software. If you'd like to try Planner Premium before purchasing you can also start a trial by going to: aka.ms/tryprojectnow. Thanks for the question Rich and I hope this helps!

Biatrice Ambrosa, Microsoft
 
> It is not. Please check out feature capabilities available across subscriptions [here](https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-web-service-description).

---

## Power BI / reporting

 Nicole EFANDA

> I use Power Bi Dashboard with Project for the Web. Could we use new Planner data in Power BI?

Brian Smith (CSS), Microsoft 

> To be clear, the premium plan tasks are the only ones that can be easily seen in Power BI, as they sit in Dataverse. There are ways to sync Planner tasks to a different storage that is also directly available in Power BI, and several 3rd parties use this approach for their Planner Power BI solutions.

---

Alexandros Kanakaris 

> As we have implemented the use of Planner is various workflows, we would like to understand, how the Reporting capabilities, that are currently limited, will be affected by the new Planner.
> 
> It is promising that the new Planner will provide greater visibility on the organization level, rather than the limited reporting capabilities currently available.
>  
> We are already investigating third-party solutions, specifically for Reporting (FluentPro - Microsoft Power BI for Planner (fluentpro.com)) as we deem extended reporting capabilities, a must.
> 
> So, should we expect functional parity with this third-party product or should we still look into that?
> 
> Is there an option to be able to visualize or test these capabilities early on, prior to product release?

Brian Smith (CSS), Microsoft

> No change to how basic plan tasks can be accessed in Power BI. There are 3rd party options available, as you mention, and new Planner should not break these in any way. Premium plans are natively available to Power BI. I'd be surprised if the 3rd Parties don't also consolidate in their solution


## Status reports - no

[Amber Baines](https://techcommunity.microsoft.com/t5/user/viewprofilepage/user-id/2358482#profile) - sent her a message
 
> Will planner have the ability to produce project status reports?

Robyn Guarriello, Microsoft

> I would love to learn more about what you envision for a status report feature - what information do you see as most important for a status report generated for your plan, how do you expect to use these reports (would you send it out to your team weekly, use it to quickly catch up on a plan, or something else), or anything you can share to help us make this a great feature for you would be super helpful!

Amber Baines

> I would love to provide feedback! Status (stoplight reporting-red/yellow/green for Overall health/scope/schedule/resources/cost), percent complete, project start date, planned completion date, tasks recently completed/tasks planned for next period, highlight key milestones completed, current issues, risks, upcoming decisions, project changes. Ability to add (or have Copilot create with user edit capabilities) a concise executive summary and/or comments for each of the stoplight reporting areas. Ability to set the "period" for when the status report is run (daily, weekly, monthly, etc). Would be great to create different status report templates with the ability to choose what information is included for different audiences (ie: high level status for entire organization, detailed level for project team). Would like to be able to share these status reports on various SharePoint sites or download .docx/pdf copy. Report should have visual indicators as much as possible (ie: charts, colors, etc). Happy to chat further if needed!

---

## Teams for now, Web later

[Laura Becker](https://www.linkedin.com/in/laura-becker-6a534556) Microsoft, Marketing and GTM for Planner

> We are hoping to to release the web experiences later this summer/early Fall - but clearly with software development we cannot commit to a specific date. We will start private and then public preview earlier! Please sign up for notification so we can keep you posted: Sign up to get the latest updates on the new Planner [here](https://aka.ms/plannernewsletter)

---

Fabian Scmidt

> Can I use the new Planner without Teams? Given the changes to Teams license some organizations might want to use Planner without Teams.

Jacques Goupil
 
> As of April 2024, new Planner is only available in Teams. Per AMA response, the Microsoft development teams is looking pushing out the new Planner into the Planner standalone app. Additionally, you can launch the Planner App via teams into it's own window by right-clicking on the Planner app icon in Teams and selecting "Open in new window"

---

## But, not for private channels

Kim Kruthaup, Georgia Tech
 
> Will the new Planner be available in Private Channels?

Andrew Friedman, Microsoft

> we're tracking this on our backlog. Here is a link to an entry in the Feedback Portal in case you'd like to upvote this item: [Enable adding a planner tab to create task in private channels · Community (microsoft.com)](https://feedbackportal.microsoft.com/feedback/idea/cf9eaf96-3a1c-ee11-a81c-000d3ae5b6f4)

---

## Portfolio features

 Peter Laws

> When talking about enterprise needs and portfolio capabilities, looking e.g. to the Project for the web roadmap feature 187140, will it be extended PowerBI templates, an extended integration for Viva Goals or something new. What can i tell customers today ... beside to wait for the preview in june 2024.

Brian Smith (CSS), Microsoft
 
> Sharing what you are wanting and hoping for [here](https://feedbackportal.microsoft.com/feedback/forum/40792262-301c-ec11-b6e7-0022481f8472), would be a great start - and the team working on the portfolio features can engage with you there.

---

Jason Rhoades
 
> What can we expect from Portfolio Management, assuming we have used that feature within Project Online for years.

Jason Hughes

https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=Worldwide%20(Standard%20Multi-Tenant)&searchterms=187140

---

Donni Northey

> Will the features of the [[MS Project Online]] (not project for the web) be available? Are there features part of project online that won't be available? Specifically the project center views to see the full portfolio and we're also interested in program management within the portfolio as well.

Brian Smith (CSS), Microsoft
 
> The portfolio features coming later in the year may address some of your questions Donni, but don't expect a 1 to 1 match with what you see today in [[Project Online]] today. The general same capabilities will be delivered, but possibly in a different way - and some of the lesser used features may not have an equivalent. But then as Holly mentioned, Copilot is uniquely placed to help with some of those scenarios too.

---

sekelly222
 
> Can you explain how the new Planner will support PMOs track and report the progress of programmes and projects, what tools are available to do this, and when a user requires a licence please?

Brian Smith (CSS), Microsoft

> New Planner doesn't directly introduce anything here, but capabilities already exist in Project for the web, whose tasks will be exposed in new Planner. Also keep an eye on the Roadmap for ==Portfolio features coming later in the year==. The beauty of new Planner is allowing the assigned resources to see their tasks from the PMO as well as being able to manage other work they have, some of whom won't need any additional license but can be assigned tasks.

---

## Cross-project, no

DedraSimmons

> Can a task be co-linked to multiple cards or on multiple planners

Brian Smith (CSS)

> It can't, but certainly heard that request before. Make sure to vote for, or add the idea [here](https://feedbackportal.microsoft.com/feedback/search/a1a93b69-2f1c-ec11-b6e7-0022481f8472)

---

Diana Christian

> Is there going to be a way to view the total tasks assigned to a person across multiple projects? Will tasks assigned in project for the web flow over to Planner?

Brian-Smith (CSS), Microsoft
 
> For yourself you'd see these in My Tasks, but it sounds like you want to see other resources tasks? Keen to hear more on the scenario. Project for the web tasks from the default environment will flow into My Tasks too, in new Planner. Other environments coming later. (and even the default is still rolling out, so you might not see them yet).

Diana Christian

> exactly. I'm a project manager, so I create all the timelines in MS Project. I run multiple projects at the same time that utilize the same resources. I was thinking it could be an amazing tool if each resource could view all project tasks assigned to them in one central location, rather than clicking into each individual project. One of the pain points is constantly reminding people when things are upcoming or due.

---

## No shared views, still

Ian Bruckner
 
> Can you please make it like sharepoint, so that when I apply a filter, for example... it maintains that for me... and it updates the URL so I can share the URL with others so they can get to the same view I'm looking at? Best example of a use case... filtering out completed tasks from gridview. This is multi-step every single time you go back to the project/plan.

Brian Smith (CSS), Microsoft

> There is some persistance within a plan Ian, but we don't persist the view across plans, or across sessions, and don't have a shareable Url to encapsulate this. We have heard this feedback before though - and if it isn't in the feedback portal be sure to add - or vote if it is already there.

Ian Bruckner

> Which feedback portal to use? Seems like the P4W one seems to have been abandoned in terms of being responded to / labeled anything other than "open". Should this all go to "Planner" now? Most (all) of my questions would be related to what I think are now called "premium plans" which I think is the new name for "project for the web"?

Alex Henry

> Yes, the shared views is a huge pain point. Especially for new users

---

## Custom fields

 [[Serge Tremblay]]

> Are there any plans to allow to add custom Fields (columns) and Custom views to Planner?

 [Nancy Wang](https://www.linkedin.com/in/nancywangjhu), Microsoft 

> Custom fields/columns are currently offered as a capability in ==premium== plans and you can see more [here](https://support.microsoft.com/en-us/office/create-a-custom-field-in-project-839d206f-b314-48f5-aa06-79140db93b94). Could you share more on what sort of custom views you're looking for?

Brian Smith (CSS), Microsoft 
 
> For premium plans yes Serge, no plans for basic plans (but you can ==use labels== of course)

Mikko Sorsa

> The Enterprise Task Custom Fields would be excellent (like in Project Online). Many customers would like to have this task custom information to the Power BI Reports. Thank you.

---

Serge Tremblay

> Are there any plans to allow to add custom Fields (columns) and Custom views to Planner?

Nancy Wang, Microsoft

> Custom fields/columns are currently offered as a capability in premium plans and you can see more [here](https://support.microsoft.com/en-us/office/create-a-custom-field-in-project-839d206f-b314-48f5-aa06-79140db93b94). Could you share more on what sort of custom views you're looking for?

Brian Smith (CSS), Microsoft
 
> For premium plans yes Serge, no plans for basic plans (but you can use labels of course)

Mikko Sorsa
 
> The Enterprise Task Custom Fields would be excellent (like in Project Online). Many customers would like to have this task custom information to the Power BI Reports. Thank you.

Ian Bruckner

> It sure would be great to do these across projects, with some local extensibility... but definitely across projects for organization level reporting.

---

Elsa Blomster
 
> How do we add custom fields to tasks? How can tasks på accessed from dataverse? What are the license requirments for those features?

 Brian Smith (CSS), Microsoft

> Only tasks from premium plans are stored in Dataverse. They are available via various APIs and applications to people with the right level of access and license. There are some limitations on how they can be updated, and there is a schedule API for that purpose. Applications such as Power BI can report on those tasks. Additional fields can be added to premium plans, or if you use a PowerApp you could extend the schema for additional fields. Plan 3 and 5 give access for customization - see the Project Service Description - https://learn.microsoft.com/en-us/office365/servicedescriptions/project-online-service-description/project-online-service-description

---

Nathan Black

> My team’s API integrations into Project for the web have been limited by the unavailability of custom fields in the https://{orgName}.crm.dynamics.com/api/data/v9.0 namespace. We can access basic task information like Name, Start Date, and Finish Date, but not any custom fields our users might add. Will this deficiency be addressed in upcoming releases of the new Planner?

---

## Personal use

Eero Joukainen

> Hi! I'm currently using [[Microsoft Lists]] as my personal todo list at work. I'm planning to move to new Planner, but I'm missing few features. Are these on the roadmap?
> 
> Paste inline pictures to notes area. My use case is to paste screenshots. If not, what about inserting files from local drive? Now attachments in personal plans are need to be pasted as URL links and that's too slow.
> Rearranging, deleting and creating new labels?
> When creating new task there are only few fields available to fill. Most cases I need to input more informating such as labels, priority etc. and to do that I need three additional clicks to reopen the task in full view. It would be super handy if the task opens in full view in the first place when clicking "Add task".

David Hopkins, Microsoft

> Great idea for creating a new task! Is there any more you could share on how and why this would enhance your experience?

---

Sathyanarayanan Vasudevan

> I have questions related to personal plans in New planner. Hope you can throw some light in to these questions? 1. Does personal plan is enabled by default in the new planner? 2. Where is the data stored related to personal planner (in Azure? similar to planner in teams) 3. when is the personal plan gets deleted? (e.g when user leaves the organization or the creator of the plan deletes the plan)? 4. is it possible to share the personal plan to multiple users, if so how does the deletion process kicks off? 5. Does the personal planner supports ediscovery? 6. Is it possible to switch of the personal planner? Thank you!

Luke Humphrey, Microsoft
 
> 1) yes 2) if you created a list in our [[To Do]] apps, technically the storage will be To Do's storage (Exchange), if you created the plan in new Planner, storage is the same as all other Planner plans 3) user deletes, user leaves org 4) if you share a personal plan in new Planner (created in Planner) it becomes an M365 group-based plan. 5) not at this time but this is on our radar, keep an eye on our Planner blogs for new info 6) can you clarify what you mean? thanks for the questions!

Forrest Hoffman

> How does your #4 answer work if Admins have restricted who can create Groups? We have purposely limited who can create Groups to prevent users from creating Redundant / Duplicate Teams when originally rolled out Teams. As described in the MS Article here
> 
> Does the backend service workflow do this as a privileged task or does it assume the user Sharing the Personal Plan has the permission to create M365 groups? or does it simply ignore the restriction?
> 
> There has been a longstanding confusion on my part around the Personal Plans based on Rosters and users only being able to create them via Graph. It seems that earlier guidance was wrong. We have people creating Project Plans that are not mapped to groups and they no longer work here.  Management of orphaned plans is becoming overwhelming. This getting complicated for me to follow. I believe that the terms "Project Plans" versus "Planner Plans" is part of the issue, especially when many articles talk about merging features between them.

---

## Comments

 [Ellen Buwalda](https://www.linkedin.com/in/ellenbuwalda)

> Will it be possible to edit a comment after posting?

Brian Smith (CSS), Microsoft

> There is the comment capability still - but it needs a Group, so if you choose not to attach or create a group then you don't see comments (it is a personal plan). To Ellen's point you cannot edit as these are stored as an e-mail thread - and you can't go back and edit an e-mail you've sent (plenty of times I wished I could!)

---

 Serge Tremblay
 
> I missed the beginning, when are we going to be able to use @mention in the Tasks comments?

Andrew Friedman, Microsoft

> this feature is one of our top requests, and it's on our backlog. If you would like to upvote this item in the feedback portal, you can do so here: [Mention function in the comment box using "@" · Community (microsoft.com)](https://feedbackportal.microsoft.com/feedback/idea/56452e81-90a3-ed11-a81b-002248519701)

---

## Existing tools / the future

Scott Ledwon

> What is the future of the [[Microsoft To Do|ToDo]] application? Will it continue to see app updates or is it all moving under this new app in Teams?

Luke Humphrey, Microsoft

> Hi Scott - thanks for the question. We're ==ultimately trying to rationalize all Microsoft tasking experiences to enable a holistic M365 task ecosystem==. Are there scenarios in To Do that you don't see in the new Planner that you leverage today/care most about?

---

Jason Hughes

> Can you clarify what will eventually be depricated and what will continue to exist in the long term? I assume "Dataverse" based Planner, and Project Operations (D365) will all continue to exist going forward...is that correct?
> 
> - Does that mean Project Desktop, Project Server, and Project Online will eventually be deprecated?
> - Will Project Operations (D365) be affected by the roadmap at all? Will that also consolidate with Planner or will it remain a separate solution?
> - Will Azure DevOps be affected by the roadmap at all? Will that also consolidate with Planner or will it remain a separate solution?
> - Will there eventually be a Desktop app that connects to Planner?

Brian Smith (CSS), Microsoft

> As announced at Ignite, there is no end of life date for [[Project Online]]. Project Server and [[Project Desktop]] follow their own lifecycles.[[ Project Server]] Subscription Edition is an evergreen release following the modern lifecycle, and expect Project Desktop future releases to stay in line with Office as it has in the past. [[Project Operations]] isn't affected by the new Planner. No plans for connection to the desktop currently, and no effects on DevOps. We'd love to hear the scenarios behind your questions.

Erik van Hurck
 
> I was assuming that Project Operations uses the Project for the web schedule? Is that changing in any way?
 
Brian Smith (CSS), Microsoft

> Nothing changing in Project Operations Erik, they will still use the schedule. Of course some changes will be coming, and Project Operations already support configuration of Hours Per Day etc. features that will also get to new Planner premium plans at some point.
   
Jason Hughes

> It's still confusing as to why Microsoft wants to keep so many different project tools. Are there long-term plans to consolidate all the project tools into one? The presentation regarding "New Planner" says things like "...it will be scalable.", "...it can handle agile and waterfall use cases.", "...it can be used for software development projects.". If all of that is going to be true, then why doesn't Microsoft put together a long-term plan to consolidate into a single tool for task/project/program/portfolio management that is "scalable", "flexible" (agile/waterfall), and can handle any type of projects?

---

AlexJacquet

> Hi, What is going to happen to Project Online? Is Planner (on the web) going to replace Project Online? And so, would you be able to connect a Microsoft Project (mpp) file to Planner?

Brian Smith (CSS), Microsoft

I'm not sure exactly which Project version you are referring to but here is a link to our FAQs: https://aka.ms/newplannerfaq and answers to some of your questions: 

> With the rebranding of Project for the web to Planner, will Project be retired? 
> 
> No, Project is not being retired.
> 
> - [[Project for the Web]] capabilities are becoming part of the new Planner. 
> - [[Project desktop]], [[Project Online]], and Project Server will continue to be available and supported for both existing and new customers. I am a current Project Online customer. 
>  
> What does this mean for me? Current customers can continue to use Project Online. 
> 
> There is currently no end of service date for [[Project Online]]
> 
> You can also import mpp files as premium plans, but not all data will come across. It doesn't connect in the same way as Project connects and saves to Project Online today.

---

[Perla Scarlett Ramirez](https://techcommunity.microsoft.com/t5/user/viewprofilepage/user-id/2054116)

> Will there be any changes to To Do? We are heavy users of it and enjoy the features.

[Robyn Guarriello](https://techcommunity.microsoft.com/t5/user/viewprofilepage/user-id/1675513) Microsoft

> This announcement does not impact any existing user scenarios or functionality of To Do apps. Many To Do capabilities that you use and love today, such as My Day, My Tasks, Flagged Emails, and more, will be available to you in the new Planner app in Teams.

 > what are the To Do features you care most about that you don't see in the new Planner but would like to? Thanks for the question!
 
---
 
## Subtasks

Cody Wiseman

> A big challenge we have is no availability of subtasks. Is there a better way to do this or are you going to add that as a feature so we can have multiple people completing certain parts of the main task?

[Brian Smith](https://techcommunity.microsoft.com/t5/user/viewprofilepage/user-id/68#profile) (CSS), Microsoft

> This is available in premium plans Cody, checklists is one way in basic plans, but I appreciate these aren't assignable.

---

Laura Gariano 
 
> Will Planner (standard or Premium) have the ability to manage checklist items by assigning them to individuals and indicating a due date for each item? How about task dependencies?

Brian Smith (CSS), Microsoft
 
> This sounds a good fit for subtasks in premium projects, but please share the scenario so we can better understand why assigned checklist items are important to you.

---

Peter Szabo

> When a task card is created and sub task are defined (check list), will be possible to add responsible and deadline for the check list?

Anav Silverman
 
> One thing you could try, in the new Planner in Teams, you can create a premium plan, with the premium capability of creating sub-tasks. By creating sub-tasks you can assign them to owners and set finish dates. Thanks for the question and would be curious to know if this would meet your specific need based on your use case.

Robyn Guarriello

> we don't support assignment and due dates for checklist items, however in premium plans we support summary tasks, under which you can have sub tasks with all task fields available to set

---


## MS365 Groups

Christophe Humbert
 
> I heard Roberto Bojorquez say that Microsoft 365 groups are needed to support Planner plans (around 5-10 minutes into the call). As far as I know, you can also create roster plans not associated with any team or group. What am I missing? Is that feature going away?

Brian Smith (CSS), Microsoft

> you can have personal plans with no group, and you can create roster plans via API - and Loop also uses this concept. Groups are needed for some features such as comments - I'll review the context of Roberto's answer later and clarify if needed.

---

## Dependencies

Robyn Guarriello, Microsoft 
 
> Premium plans support task dependencies, which allow you to link tasks together just like you are describing. Then, the Planner scheduling engine will automatically update your plan's schedule anytime a predecessor task's dates are updated

---


## Limits

Mike Meall

> If I remember correctly, there was a limitation of 1,000 items in Project for the Web. Projects that our team manage can be 5,000 items or more. What are the expected capabilities of projects and the number of items within Teams?

Brian Smith (CSS), Microsoft

> Premium plans do still have this limit, but keep an eye on the public roadmap. For basic plans there are other, higher limits, but no scheduling, effort or dependencies.

---

Trish Gillham

> Are you going to eliminate the cap on number of tasks in a tenant and the number of tasks in the lifetime of a plan? These severely hamper our ability to use this product. We inject 2000-3000 tasks per month just for simple operation. That number adds up quickly with the current limitations.

Brian Smith (CSS), Microsoft

> There are some limits on numbers of tasks for basic plans and these are documented. https://learn.microsoft.com/en-us/office365/planner/planner-limits . There isn't a limit on the total number of tasks in a tenant, and the limits that do exist are designed to suit the anticipated ways Planner is used. If there are limits you feel are impacting your use then we'd love to know the scenarios. Premium plans also have task limits - keep an eye on the Roadmap for changes here.

---


## Templates

Anton Bauman

> Will there be a feature to create customized templates? And will there be a way to export plans like in MS Project (to for example print them out)?

David Hopkins, Microsoft

> We don't currently have a way to create custom templates, but there are two things you can do instead. One I've seen is to build the plan you want (name it Template) and then use Copy Plan to create copies of it when you need. And another exciting one is to use Copilot in Planner to effectively build a new plan for you based on a natural language prompt. And yes, premium plans can be exported to Excel (coming soon for basic plans too).

---

## Loop

John Hoover

> When [[Loop]] integration is added to OneNote, will that integration allow for embedding specific Planner plans right into OneNote? Currently facing a challenge of capturing meeting minutes in OneNote but then not having an easy way to move meeting minute action items from OneNote into Planner.

David Hopkins, Microsoft

> Yes, being able to show Planner plans in OneNote using the Planner Loop component is on our backlog to support (in addition to the rest of the surfaces that Loop components can be used in).

---

Karen Angerer

> What is required to be able to see loop tasks in the new planner? Currently we have tasks by planner, and we have loop, but we don’t see the loop tasks in tasks by planners, which I’m sure is a config thing since we do not allow users to create plans unless they are associated with a team channel. Is that fixed in the new planner or do you except we’ll see more issues if we don’t allow users to create plans outside of channels?

David Hopkins, Microsoft

> [[Loop]] tasks assigned to you will show in your 'Assigned to me' view in 'My Tasks' in the new Planner. We are also working on making Loop plans available to manage within the new Planner. The new Planner also allows you to work with all your plans that aren't

---

## Migrating

 Laurie Heer, D365Teams
 
> When will we be able to convert planners to premium projects? I love the due date tasks experience on planner tasks. Will task deadlines be available for premium project tasks?

Brian Smith (CSS), Microsoft

> Yes, you will and you can already see this in Planner web using the Copy Plan to Project option. There isn't a task deadline specifically, just a finish date - is that what you need? If not then [feedback](https://feedbackportal.microsoft.com/feedback/forum/a1a93b69-2f1c-ec11-b6e7-0022481f8472)

---

Erik van Hurck 

> I got 3 questions from a client: 1. How do you (Microsoft) plan for upgrading the old Project For the Web customer? For named org scenarios specifically? What is the task limit going to be? 2. Who is the target customer/user for the New Planner? 3. Will there be any restrictions when interacting with the Project API? Can we read, create etc.?

Brian Smith (CSS), Microsoft
 
> There isn't really any need for upgrade as such, all the tasks from To Do, Planner and Project for the web are still the same tasks. Today you'll only see the default environment tasks - named environments coming later. As was mentioned yesterday at Meet the Makers, there will likely be some architectural changes coming, but those changes should be somewhat transparent to our customers. Keep an eye on Roadmap for task limit increases, and no changes in the API for now.

---

## Power Automate

Anne Hodgskiss

> Will the new Planner have more triggers that we can use in Power Automate? I'd love to be able to create flows that use the tags field or trigger off what bucket I put the task in to.
 
Alexander Lahuerta, Microsoft

> We haven't changed the current Power Automate connector as part of the new Planner. We're focusing on delivering the converged user experience in the Teams app, and then shifting to the tools we give customers for customization and extensibility.

---

Abram Cardoza 

> Are there any new Power Automate Triggers and Actions available with the new Planner?

Brian Smith (CSS), Microsoft

> No new triggers or actions right away. Are there specific ones you think are missing or and which ones would add the most additional value?

---

John Johnson

> Will [[Project for the Web]] still be able to be embedded into PowerApps? Will developers need to update their PowerApps? Will it feature the same functionality as Planner? Currently 'Project for the web' is a slightly lighter version when its embedded in a PowerApp.

Alexander Lahuerta, Microsoft

>  Yes, we will continue to support managing ==premium plans (Project for the web)== within the Power Platform. We haven't made changes for how you can integrate these types of plans.

---

## Other Questions

Alex Henry

> I would like to teach my users how to protect their planner boards from staff deleting or modifying tasks they shouldn't be (#DLP)

Alexis Green

> Only option I've found is to not tell people Planner exists so they don't go there and do something they aren't supposed to

--- 

Scott Brant

> Appreciate this has likely been asked, but with Task Version Control in Planner Premium, is that coming soon or under the Project Plan 3 License, today?

Brian Smith (CSS), Microsoft

> - I'm not sure what you heard in terms of version control - there is task history to help you follow what changes have been made, and baselines coming to help you compare to a previous checkpoint - but not version control in the way I would think of it.

---

John Hoover

> Plans for better supporting the needs of engineering and construction consultant organizations that want to use new Planner (P4W)? - Better way of exporting Gantt charts to share with customers? Current .pdf export is fairly terrible - Being able to baseline project schedules to show schedule changes over project lifecycle - Adding in financial planning / budgeting features left out from legacy MS Project - Easily export Planner schedule as MS Project or P6 compatible file for Customers using those products

 Robert Ornelas

> This is crucial. We need more export options. Hopefully one day we can print a filtered view to a PDF, not the entire plan.

---

Peter Laws
 
> Are there plans for a backup feature for Planner plans and Project for the web? What is your recommendation for IT operation.

Ryan Helmer

> I know of only one backup solution for Planner (AvePoint; not sure if compatible with New Planner), but have no experience with it, particularly with restore. Much better would be versioning, but currently there is zero realistic recovery story provided, though this has been requested I think since at least 2018 in UserVoice. This is critical to the Integrity and Availability of the CIA triad, and therefore critical for serious business use.

---

Alicia Pichardo
 
> My other question just got lost, but my Tasks in New Planner in Teams only allows the update of Progress on a Task from Project for the web that has effort. To update Effort, you have to click on the Project for the web Project link to update Effort and Work Remaining in Project for the web? Is this intended behavior?

 Brian Smith (CSS), Microsoft

> That is the current intended behavior. If you open up the plan from My Plans you would be able to add the effort and remaining effort columsn to make such an update, but initially the columns available in My Tasks for premium plans are similar to those of basic plans

---

SholomG

> At what point does a project or task become a "plan" on a planner?

 Luke Humphrey, Microsoft
 
> In the new Planner you can create new plans or premium plans, the latter are technically "projects" if you are familiar with Project for the web. Tasks created outside of plans (e.g. in Private Tasks) can be moved into plans.

---

Alex Henry

> Will you be adding a proper "Activity Feed' that informs team members exactly what has changed, when it happened and who did it? The current solution (the pop-up banner) is as useless as a screen door on a submarine.

Brian Smith (CSS), Microsoft

> Premium plans do have task history, that shows the kind of information you are looking for. No plans to have this available for basic plans. (Love your screen door analogy Alex!)

---

Mikko Sorsa

> If there are hundreds of tasks in the project, the Show Outline Level feature could be very useful. Like in the MS Project and Project Web App. E.g. "Show Outline Level 1" could show the first hierarchy level tasks.

Brian Smith (CSS), Microsoft
 
> Great suggestion! This isn't such an option at general release, but I can see this being something we may get customer feedback on and would be as a useful addition.
