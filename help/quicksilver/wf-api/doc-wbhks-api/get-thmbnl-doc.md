---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Get a thumbnail for a document
description: Get a thumbnail for a document
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
TQID: https://experienceleague.adobe.com/-LE1gxQ9aViRNuN0sI14HlZaIcLc6Mmm8XmS1zaRCFQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
---
# Get a thumbnail for a document

Returns the raw thumbnail bytes for a document.

**URL**

GET /thumbnail

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| id&nbsp; |The document ID. |
| size&nbsp; |&nbsp;The width of the thumbnail. |


## Response

The raw thumbnail bytes.

**Example:**:&nbsp;https://www.acme.com/api/thumbnail?id=123456
