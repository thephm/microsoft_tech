# Azure Resource Manager
### Azure Resource Manager

Running your app on Azure likely involves working with multiple Azure services. These services follow the same life cycle and can be thought of as a logical unit. For example, a web app might use Web Apps, SQL Database, Storage, Azure Cache for Redis, and Azure Content Delivery Network services. [Azure Resource Manager](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/overview) lets you ==work with the resources in your application as a group. You can deploy, update, or delete all the resources in a single, coordinated operation==.

Along with logically grouping and managing related resources, Azure Resource Manager includes ==deployment capabilities that let you customize the deployment and configuration of related resources==. For example, you can use Resource Manager deploy and configure an application. This application can consist of multiple virtual machines, a load balancer, and a database in Azure SQL Database as a single unit.

You develop these deployments with an easy to use infrastructure-as-code language called [[Bicep]]. If you prefer a less semantically rich approach, you can use an Azure Resource Manager template, which is a JSON-formatted document. Bicep files or templates let you define a deployment and manage your applications declaratively, rather than with scripts. Your templates can work for different environments, such as testing, staging, and production. For example, you can use templates to add a button to a GitHub repo that deploys the code in the repo to a set of Azure services with a single click.

> **When to use**: Use Bicep or Resource Manager templates when you want a template-based deployment for your app that you can manage programmatically by using REST APIs, the Azure CLI, and Azure PowerShell.
> 
> **Get started**: To get started using Bicep, see [What is Bicep?](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/overview). To get started using templates, see [Authoring Azure Resource Manager templates](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/syntax).