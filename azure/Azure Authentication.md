# Azure Authentication

It's crucial to not only know who is using your applications, but also to prevent unauthorized access to your resources. Azure provides several ways to authenticate your app clients.

## [[Microsoft Entra ID]]

> The Microsoft multitenant, cloud-based identity and access management service. You can add single-sign on (SSO) to your applications by integrating with Microsoft Entra ID. You can access directory properties by using the Microsoft Graph API. You can integrate with Microsoft Entra ID support for the OAuth2.0 authorization framework and OpenID Connect by using native HTTP/REST endpoints and the multiplatform Microsoft Entra authentication libraries.
    
> **When to use**: When you want to provide an SSO experience, work with Graph-based data, or authenticate domain-based users.
> 
> **Get started**: To learn more, see the [Microsoft Entra developer's guide](https://learn.microsoft.com/en-us/azure/active-directory/develop/v2-overview).
    
## App Service Authentication

 When you choose App Service to host your app, you also get built-in authentication support for Microsoft Entra ID, along with social identity providers—including Facebook, Google, Microsoft, and Twitter/X.
    
> **When to use**: When you want to enable authentication in an App Service app by using Microsoft Entra ID, social identity providers, or both.
> 
> **Get started**: To learn more about authentication in App Service, see [Authentication and authorization in Azure App Service](https://learn.microsoft.com/en-us/azure/app-service/overview-authentication-authorization).

To learn more about security best practices in Azure, see [Azure security best practices and patterns](https://learn.microsoft.com/en-us/azure/security/fundamentals/best-practices-and-patterns).