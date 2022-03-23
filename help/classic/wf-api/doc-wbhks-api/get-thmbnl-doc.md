---
filename: Get thmbnl-doc
content-type: api
navigation-topic: documents-webhooks-api
title: Get a thumbnail for a document
description: Returns the raw thumbnail bytes for a document.
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

## Response

The raw thumbnail bytes.

``` ```**Example: **``````:&nbsp;https://www.acme.com/api/thumbnail?id=123456
