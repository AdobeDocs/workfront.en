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
