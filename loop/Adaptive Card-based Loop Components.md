---
tags:
  - video
url: https://build.microsoft.com/en-US/sessions/0d175daf-5ccf-43dd-8ce9-8710245a8768?source=sessions
people: 
organizations: 
date: 2023-05-24
duration: 43:02
---

# Adaptive Card-based Loop Components

[post](https://build.microsoft.com/en-US/sessions/0d175daf-5ccf-43dd-8ce9-8710245a8768?source=sessions) starts at 04:27

HBR: a typical information worker toggles 1,200 times between different apps in a day, spending about 9% of their time in their work context switching

[[MS365]] Extensibility Platform

Continue in flow of work to discover, create, share, and act on external application content.

07:29

[[Jagdesh Goddhumuri]]
Product Manager, [[Zoho]]
https://www.linkedin.com/in/jagadeeshgoddumuri

- Atomic units of productivity
- They built them for [[Zoho Project]] and Service Express Cloud
- ServiceDesk Plus Cloud
	- ITSM tickets interactive in Outlook Mail and Teams

---

## SAP

14:30

[[Ullas Holla]]
Development Architect
https://www.linkedin.com/in/ullas-holla

- credit checks are a team sport
- approve and reject scenario to make a decision
- used [[Microsoft Teams Toolkit]] with Message Extension Template
	- a [[Message Extension]] is:
		- a Web server that the [[Bot Framework]] on Azure talks to using the Bot Protocol
	- use the Bot Framework SDK
	- The toolkit does the following for you:
		- creates the run configs
		- makes sure user is logged into their M365 account
		- makes sure the tenant has side-loading enabled
		- starts the tunnel
		- packages your app
		- registers your app on Azure
		- uploads your app package to Teams
		- starts your server
		- connects your tunnel to the server
		- creates good defaults to provision and deploy your Message Extension on Azure
- [[Microsoft Adaptive Card]]
- To surface a [[Microsoft Loop Component|Loop Component]] in the [[Microsoft Teams|Teams]] chat is via link confirming
	- user pastes a URL into Teams chat and this code is called

![[TeamsAppBasedLinkQuery.png]]

- List of domains goes into the app manifest
- uses principal propagation from Azure AD to SAP IAAS so the right people with the right authorization see the right data
---

## Priority Metrix

19:53

Pablo Diaz-Gutierrez
co-creator, co-Founder
@appfluence

- Adaptive Cards with LEAP properties - live, embeddable, and portable
- Guidelines to honor these properties
- an email and project management solution

![[Loop LEAP properties.png]]

- Visually compose your card using https://adaptivecards.io/designer

![[Dynamic Card Generation.png]]

- can toggle fields to make them visible or not but if need more space can let user get a full-view of the element in a pop-up from within the "hub"

- advice:
	- start with something minimally useful and iterate
	- get creative with UI elements: Emojis, ASCII art
	- test all variants (hub, OS, form factor)
	- embrace the review process, think of it as a bonus QA step
		- trust their UX recommendations


---

[[Luan Nguyen]], Principal Engineer, [[Microsoft]], @dotnetjunky

[[Sid Vinnakote]], Principal Engineer, [[Microsoft]], @SVinnakote

- they are adding graphs
- https://adaptivecards.io/roadmap
- mostly built by 3rd parties
- can it be integrated with Dyanmics 365 workflow? renaming to Viva Sales and yes they are working on adaptive cards