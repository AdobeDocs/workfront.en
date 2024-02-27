---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Get document content via Webhooks
description: Returns the raw bytes for a document
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
---
# Get document content via Webhooks

Returns the raw bytes for a document

## URL

GET /download

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
   <td> <p>id</p> </td> 
   <td>&nbsp;The document ID.</td> 
  </tr> 
 </tbody> 
</table>

## Response

The raw bytes of the document.

**Example**:&nbsp; `https://www.acme.com/api/download?id=123456`
