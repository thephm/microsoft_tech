# Complete Basic Operations Using SharePoint REST Endpoints

![rw-book-cover](https://learn.microsoft.com/en-us/media/open-graph-image.png)
- Author: [[VesaJuvonen]]
- Summary: The document explains how to complete basic operations using SharePoint REST endpoints. It details how to make HTTP requests to retrieve or update SharePoint entities like webs, lists, and list items through appropriate endpoints. The REST service supports CRUD operations with HTTP requests corresponding to different operations. It also discusses how to read data, write data, and handle properties that aren't returned with the resource. Additionally, it addresses authentication methods, including OAuth and request digests, essential for creating, updating, and deleting SharePoint entities.
- URL: https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/complete-basic-operations-using-sharepoint-rest-endpoints

- One advantage of using REST is that you don't have to add references to any SharePoint libraries or client assemblies. Instead, you make HTTP requests to the appropriate endpoints to retrieve or update SharePoint entities, such as webs, lists, and list items.
- To read information from a REST endpoint, you must know both the URL of the endpoint and the OData representation of the SharePoint entity that is exposed at that endpoint. For example, to retrieve all the lists in a specific SharePoint site, you would make a **GET** request to `http://<site url>/_api/web/lists`.
- For more information about how you can obtain an access token, see [Context Token OAuth flow for SharePoint Add-ins](https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/context-token-oauth-flow-for-sharepoint-add-ins) and [Authorization Code OAuth flow for SharePoint Add-ins](https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/authorization-code-oauth-flow-for-sharepoint-add-ins).
  ```
HttpWebRequest endpointRequest =(HttpWebRequest)HttpWebRequest.Create("http://<site url>/_api/web/lists");
     endpointRequest.Method = "GET";
  endpointRequest.Accept = "application/json;odata=verbose";endpointRequest.Headers.Add("Authorization",
  "Bearer " + accessToken);
  HttpWebResponse endpointResponse  = (HttpWebResponse)endpointRequest.GetResponse();
  ```
  
- Another important consideration when creating, updating, and deleting SharePoint entities is that if you aren't using OAuth to authorize your requests, these operations require the server's request form digest value as the value of the **X-RequestDigest** header. You can retrieve this value by making a **POST** request with an empty body to `http://<site url>/_api/contextinfo` and extracting the value of the `d:FormDigestValue` node in the XML that the **contextinfo** endpoint returns. 