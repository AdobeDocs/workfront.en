---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Get information about the service
description: Get information about the service
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
---

# Get information about the service (not yet implemented)

>[!NOTE]
>
>The release date for this feature is yet to be determined.

Returns information about the service, such as features and capabilities. Adobe Workfront will use this information to customize the user interface in Workfront. For example, if the webhook implementation contains some custom actions, the JSON should list those operations in the JSON. Users would then be able to invoke these actions from Workfront.

**URL**

GET /serviceInfo

## Query Parameters

None. In addition, calls to this endpoint should not require authentication.

## Response

JSON containing information about this service

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name</th> 
   <th>Type&nbsp;</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion&nbsp;</td> 
   <td>String&nbsp;</td> 
   <td>The webhook version implemented by this service. This is the version&nbsp;number listed at the top of this spec.</td> 
  </tr> 
  <tr> 
   <td>version&nbsp;</td> 
   <td>String&nbsp;</td> 
   <td>The internal version number for this service. This number is determined by the webhook service provider and is used for informational purposes only.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher&nbsp;</td> 
   <td>String&nbsp;</td> 
   <td>The name of the company providing the webhook implementation.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String&nbsp;</td> 
   <td>A list containing the API Endpoints implemented by this service. This may be used to ensure that the user interface in Workfront reflect the capabilities offered by the webhook provider. Each item in the list must include the name of the endpoint (such as "search").</td> 
  </tr> 
  <tr> 
   <td>customActions&nbsp;</td> 
   <td>String</td> 
   <td>&nbsp; <p>A list containing the custom operations implemented by this webhook. Each list item includes a name and display name. The display name will appear in the "Document Actions" dropdown in Workfront. Clicking on the item in the dropdown will invoke the action in the webhook by calling the /customAction endpoint.</p></td> 
  </tr> 
 </tbody> 
</table>

**Example:** `https://www.acme.com/api/serviceInfo`

returns

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```