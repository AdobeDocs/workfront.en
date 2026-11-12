---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Create a Folder with Document Webhooks
description: Create a Folder with Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
TQID: 'https://experienceleague.adobe.com/nneISzqXTIVje77d8QU29YPr6mOVplcwgzf48TEi-0A'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
---
# Create a Folder with Document Webhooks

Creates a folder in a given directory.

## URL

POST /createFolder

## Query Parameters

| **Name** |**Description** |
|---|---|
| parentId&nbsp; |The folder ID in which the folder should be created |
| name&nbsp; |The name of the new folder |




**Response**

The metadata for the newly created folder, as defined by the /metadata endpoint.

## Example

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

returns

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
