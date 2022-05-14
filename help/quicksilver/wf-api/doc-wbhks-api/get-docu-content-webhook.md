---
filename: get-docu-content-webhook
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Get document content via Webhooks
description: Returns the raw bytes for a document
---

# Get document content via Webhooks

Returns the raw bytes for a document

## URL

GET /download

## Query Parameters

<table> 
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

**Example:**:&nbsp; [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
