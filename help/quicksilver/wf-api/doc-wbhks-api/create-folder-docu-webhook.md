---
filename: create-folder-docu-webhook
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Create a Folder with Document Webhooks
description: Creates a folder in a given directory.
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

&nbsp;

**Response**

The metadata for the newly created folder, as defined by the /metadata endpoint.

## Example

<pre>POST https://www.acme.com/api/createFolder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­<br>-------------------------------<br>parentId=1234<br>name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­<br>-------------------------------</pre>returns
<pre>{title:"New Folder",br /> kind:"folder"<br> id":"5678",<br> viewLink:"”,<br> downloadLink:"",<br> mimeType:"",<br> dateModified:"2014­06­05T17:39:45.251Z"<br> size: ""<br> }</pre>