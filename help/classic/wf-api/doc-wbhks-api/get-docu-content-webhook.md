---
filename: get-docu-content-webhook
content-type: api
navigation-topic: documents-webhooks-api
title: Get document content via Webhooks
description: Returns the raw bytes for a document
---

# Get document content via Webhooks

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Returns the raw bytes for a document

## URL

GET /download

## Query Parameters

<table cellspacing="15"> 
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
   <td> <p>id</p> </td> 
   <td>&nbsp;The document ID.</td> 
  </tr> 
 </tbody> 
</table>

## Response

The raw bytes of the document.

``` ```**Example: **``````:&nbsp; [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
