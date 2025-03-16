---
tags:
  - course
  - azure
date: 2024-10-12
---

# Intro to Azure

- [[Jim Cheshire]]
- https://www.linkedin.com/learning/getting-started-with-microsoft-azure

## Benefits of cloud computing

![[Intro to Azure - Cloud Services - 2024-10-12.jpg]]

![[Intro to Azure - Cloud Types - 2024-10-12.jpg]]

## Microsoft Azure under the hood

![[Intro to Azure - Regions - 2024-10-12.jpg]]

![[Intro to Azure - Data center - 2024-10-12.jpg]]

![[Intro to Azure - ARM - 2024-10-12.jpg]]

### ARM templates

![[Intro to Azure - VM templates - 2024-10-12.jpg]]

## Interacting with Azure

![[Intro to Azure - Portal - 2024-10-12.jpg]]


![[Intro to Azure - Services - 2024-10-12.jpg]]

### Azure Power Shell

![[Intro to Azure - PowerShell - 2024-10-12.jpg]]


![[Intro to Azure - Power Shell Example - 2024-10-12.jpg]]

### Azure CLI

![[Intro to Azure - CLI - 2024-10-12 1.jpg]]


![[Intro to Azure - CLI example - 2024-10-12.jpg]]

![[Intro to Azure - az interactive - 2024-10-12.jpg]]

### Azure Cloud Shell

![[Intro to Azure - Cloud Shell - 2024-10-12.jpg]]


![[Azure - Cloud Shell quiz - 2024-10-12.jpg]]

# Azure Virtual Machines


![[Intro to Azure - VMs - 2024-10-12.jpg]]

## Create a resource
![[Intro to Azure - Create a resource - 2024-10-12.jpg]]


![[Intro to Azure - Create a VM - 2024-10-12.jpg]]

- A Resource Group is a container of Azure Resources

## Azure Virtual Networks
![[Intro to Azure - Virtual Networks - 2024-10-12.jpg]]

### Network settings 

![[Intro to Azure - Networking - 2024-10-12.jpg]]


![[Intro to Azure - Networking - Subnets - 2024-10-12.jpg]]

## Add disks to a VM

![[Intro to Azure - Disks - 2024-10-12.jpg]]


![[Intro to Azure - Disks example - 2024-10-12.jpg]]

## Resize a VM

![[Intro to Azure - Resize a VM - 2024-10-12.jpg]]

![[Resize a VM.png]]

### Remote access

![[Azure - Remote Access.png]]

#### Bastion

- Click Connect on the left under `Settings` - takes about 10 minutes to setup

![[Azure - Bastian.png]]

## [[Azure App Service]]

### Create a Web App

![[Azure - Overview of App Service.png]]

![[Azure - Create a Web app.png]]

- Creates it in a VM running in Azure

![[Azure - Create Web App.png|500]]

![[Azure - Your web app is running.png]]

## Scale "elasticity"

- resizing VM is vertical scaling
	- Scale up - increase resources
	- Scale down - reduce resources
- horizontal is increasing number of VMs - all VMs are ==exactly the same== including size, apps
	- Scale in - reducing # of VMs
	- Scale out - increasing # of VMs

![[Azure - Overview of Scaling.png]]

![[Azure - Scale-up and down menu.png]]

![[Azure Scale out.png]]
### Auto scaling

- e.g. add instances (VMs)

![[Azure - Autoscaling.png]]

## Web Apps and Authentication 

![[Web Apps and Authentication.png]]

![[Azure - add an identity provider.png]]

![[Azure - add an identity provider - request API permissions.png]]

![[Azure - permissions requested dialog.png|350]]

### Configure backups for your Web app

- Automatic backups every hour (depending on pricing plan)

![[Azure - Web App Backups.png]]

- Can add a storage account on the fly

![[Azure - Configure custom backups.png]]

### Add a custom domain

![[Azure - Add a Custom Domain.png]]

- add the `domain.xyz` and then add `www.domain.xyz` (subdomain)

![[Azure - Custom domains.png]]

### Configure networking for Web apps

![[Azure - Networking and Web Apps - Overview.png]]

![[Azure - Networking.png]]

### Add hybrid connection

- Hybrid connections use `Hybrid Connection Manager` app you install on a server on the network (not all machines)

> the networking features and apps service allow you to connect your Web Apps to other Azure services, and to even connect your Web App to resources that are on other networks, such as on-premises resources, or maybe even resources that are in other clouds. 
> 
> There are a couple of key features in Web Apps that enable this functionality. VNet integration makes it easy to connect your Web Apps to an Azure virtual network, and Hybrid Connections allow you to connect your Web Apps to other networks. Hybrid Connections can be a bit more complicated, because you have to deal with multiple networks and networking across the internet, in most cases. VNet integration is a bit easier. 
> 
> to access the features for networking with your Web App, after you've opened your Web App in the **Azure portal**, in the **settings** menu, you just simply click on networking. Now, there are a lot of things here. 
> 
> **Inbound traffic** allows you to control what addresses are able to access your Web App from outside. 
>
> We're going to look at **outbound traffic**, because what we're talking about here is allowing our Web App to connect outbound to something else
> 
> set up **VNet integration** to integrate our Web App with the virtual network we created earlier. But before I do that, I want to show you ==Hybrid Connections== ... which allow you to connect your Web App to something on another network, let's say maybe a server that's located on premises, and it **does this using a little utility that you install on that on-premises server called the Hybrid Connection Manager**, 
>
> You don't have to install it on all the machines, just a machine that connects to whatever resource you're trying to get to. So the first step here is you would need to add a Hybrid Connection, and then we'll create a new Hybrid Connection. 
> 
> a two step process in App Service. The first thing you do is you select a Hybrid Connection or create a new Hybrid Connection, and then you add that Hybrid Connection to your Web App. 
> 
> Now, the **endpoint host** is the host name for the server that's going to be running that service that you're trying to connect to... the name of that server on my network, and then also the **port** that you're going to use to connect to, which could be whatever port you've opened to do that connection, 
>
> Now we need a Service Bus namespace. **Service Bus** is a feature in Azure, it's a service in Azure, and Hybrid Connections use Service Bus, or specifically, what's called a ==Service Bus relay==, just a technical term for that functionality that allows you to take that connection on your Web App in this case, and relay it into an on-premises server. 

![[Azure - Add Hybrid connection.png]]
### VNet integration

- Establish connectivity from Web app outbound to a VNet in Azure

![[{ABC36E8C-1427-4DB2-A48F-B02AB9878902}.png]]

## Azure Storage

![[Azure Storage overview.png]]

> Azure Storage offers many different services for storage. Azure Blob Storage is for storing unstructured files, files like images, documents, videos

- organize files in containers, like a file folder on your hard drive
- binary large object (blob)
- 3 tiers to control costs:
	- Hot - need to access often
	- Cool 
	- Archive

- Fixed amount for storage, lower (archive) to higher (hot)
- Variable price to access, more (archive) or less (hot)

### SaaS Tokens

> can use shared access signature, or SaaS tokens, to give someone else access to your blobs or your containers

- an SaaS token is just a URL, and it specifies the level of access and an expiration date
- anyone with that SaaS token can access your Azure storage with the level of access you specify
- when that expiration date gets reached, it stops working

### Azure Storage Explorer

![[Azure Storage Explorer.png]]

- `Hot tier` is the default tier, can use `Change access tier` for a specific file
	- have to leave something in cool tier (~ 30 days) to not incur additional charges -- early removal fee
- `Archive tier` is for backups, to access first have to move it to `hot` or `cool` tier - called **hydration**

![[{F39F21B8-FB7B-4109-9C50-DE163BDC4B1C}.png]]

### Give access

- Shared access signature

![[Azure Storage - Shared Access.png|400]]

![[Shared Access Signature.png|400]]

## Artificial Intelligence
### Overview of Artificial Intelligence

![[Azure Cognitive Services.png]]

- There are two different types of AI. 
	- weak AI
		- sometimes called narrow AI
	- strong AI
		- artificial general intelligence (AGI)
		- exceeds the capabilities of humans and is able to learn and evolve on its own without human intervention

			> When I first started teaching people about AI a few years ago, we believed that strong AI was likely decades away, and there were many who believed we would never achieve it, and it's amazing how times have changed because there are now experts who believe we'll have strong AI within the next five years. 

 > AI uses neural networks to perform work, and you can think of a neural network as something like a virtual representation of the way our brains work. Neural networks excel in being able to recognize patterns in data and the complex relationships between huge sets of data, and without these neural networks, the AI tools that people use today, like [[ChatGPT]], wouldn't be possible. 
 > 
 > Now, there's a field of AI called machine learning, or ML, that focuses on AI learning from enormous amounts of data and then making decisions based on that data. ML uses what are called [[ML models]], and those are just **complicated mathematical algorithms**. It uses those to make decisions and then to improve the accuracy of the model itself, and they train these models on absolutely enormous amounts of data. 
 > 
 > We now have natural language processing using some of our generative AI products, like ChatGPT for a conversational AI and then Midjourney and DALL-E for image creation using AI, and these new models use **prompts** that the user provides to learn what they need to do, and they're advancing rapidly, I mean, very rapidly. In fact, we're now seeing enormous advancements in weeks rather than years, and I think we can expect that to continue. 
 
 ### Machine Learning

![[Azure Machine Learning.png]]

### OpenAI

![[Azure - OpenAI.png]]