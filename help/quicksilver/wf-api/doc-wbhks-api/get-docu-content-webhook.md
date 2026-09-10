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
TQID: https://experienceleague.adobe.com/AIN65ofKDJA95iMpvNwoe3oQapmyxzDC16dpf5ehwH0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
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
