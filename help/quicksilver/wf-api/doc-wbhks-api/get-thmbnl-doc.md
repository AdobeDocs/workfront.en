---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Get a thumbnail for a document
description: Returns the raw thumbnail bytes for a document.
author: John
feature: "Workfront API, Digital Content and Documents"
---

# Get a thumbnail for a document

Returns the raw thumbnail bytes for a document.

## URL

GET /thumbnail

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| id&nbsp; |The document ID. |
| size&nbsp; |&nbsp;The width of the thumbnail. |

{style="table-layout:auto"}

## Response

The raw thumbnail bytes.

**Example:**:&nbsp;https://www.acme.com/api/thumbnail?id=123456
