---
aliases: 
  - ADF
---
# Azure Data Factory

Azure Data Factory (ADF) is a cloud-based data integration service that allows you to create, schedule, and orchestrate data workflows. It is designed to help organizations gather, prepare, transform, and analyze vast amounts of data from various sources, both on-premises and in the cloud. Here are some of the key features of Azure Data Factory:​

- Data Integration: ADF provides a platform to efficiently integrate data from disparate sources. It supports copying data between a large variety of data stores in different formats, performing data transformations, and loading the processed data to a destination for analytics.​
    
- Managed Data Pipelines: You can create, schedule, and manage data-driven workflows (called pipelines) where each pipeline can ingest, move, transform, and process data as needed. ADF lets you create complex ETL processes without having to write code.​
    
- Data Flows: Data flows allow you to visually design data transformations in ADF without writing code. These transformations are then executed at scale across multiple computing environments, such as Azure Data Lake Analytics, Azure HDInsight, and even on-premises servers.​
    
- Integration Runtime: The integration runtime (IR) component in ADF is what executes the data flows as managed data pipeline activities. It supports data integration across network environments, facilitating data movement and dispatch between various network environments (public cloud, private cloud, and on-premises).​
    
- Connectivity: Azure Data Factory has built-in connectors for a wide range of data sources and sinks. This includes traditional databases, data warehouses, data lakes, and SaaS services, allowing seamless connectivity and integration.​
    
- Monitoring and Management: ADF provides robust monitoring features that help you track the health and activity of your pipelines. It also integrates with Azure Monitor and Azure Log Analytics for enterprise-grade monitoring and analytics.​
    
- CI/CD for Data Pipelines: ADF supports continuous integration and delivery (CI/CD) for data pipelines using Azure DevOps and GitHub, which enables automation of pipeline deployment and management across different environments.​
    
- Security and Compliance: Azure Data Factory is integrated with Azure Active Directory (Azure AD) for authentication and supports role-based access control (RBAC). Data stored and processed in ADF can be secured using Azure’s built-in security measures to ensure compliance with various standards and regulations.​
    
- Global Availability: Azure Data Factory is available globally, allowing deployment in multiple regions worldwide to meet local data residency requirements and to optimize for latency.​