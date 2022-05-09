---
filename: Get thmbnl-doc
content-type: api
navigation-topic: documents-webhooks-api
title: Get a thumbnail for a document
description: Returns the raw thumbnail bytes for a document.
---

# Get a thumbnail for a document

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

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

**Example:**:&nbsp;https://www.acme.com/api/thumbnail?id=123456
