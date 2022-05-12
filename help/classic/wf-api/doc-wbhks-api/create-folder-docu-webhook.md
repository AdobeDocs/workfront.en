---
filename: create-folder-docu-webhook
content-type: api
navigation-topic: documents-webhooks-api
title: Create a Folder with Document Webhooks
description: Creates a folder in a given directory.
---

# Create a Folder with Document Webhooks

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

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
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
