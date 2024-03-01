---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Perform a custom action
description: Perform a custom action
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
---

# Perform a custom action (not yet implemented)

This endpoint allows an Adobe Workfront user (or an automated workflow event) to perform an action in the external system. The /customAction endpoint accepts a "name" parameter, which allows the webhook provider to implement multiple custom operations.

The webhook provider registers custom actions with Workfront by including the actions in the /serviceInfo response under customActions. Workfront loads this list when setting up or refreshing the webhook provider under Setup > Documents > Custom Integrations.

Users can trigger the custom action by selecting the section under "Document Actions"

**URL**

GET /customAction

## Query Parameters

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name&nbsp;</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>name</p> </td> 
   <td> <p>The identifier specifying the type of action to be performed. This value corresponds to one of the customAction values listed returned by the /serviceInfo endpoint.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId&nbsp;</td> 
   <td>The workfront document ID for which the action is being performed.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId&nbsp;</td> 
   <td>&nbsp;The workfront document version ID for which the action is being performed.</td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

## Response

A JSON string indicating success or failure, as specified in the Error Handling section below. On failure (i.e. status = "failure"), Workfront will display the provided error message to the user.

**Example:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

response

```
{
status: "success"
}
```
