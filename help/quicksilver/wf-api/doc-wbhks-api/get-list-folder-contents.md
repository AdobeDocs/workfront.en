---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Lists metadata for files or folders
description: Lists metadata for files or folders
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
---

# Get item list of folder contents

Lists metadata for the files and folders for a given folder.

**URL**

GET /files

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| parentId&nbsp; |The folder ID. To get the metadata of the root directory, use the value '/'. |
| max&nbsp; |The maximum number of items to return. Used for pagination. |
| offset&nbsp; |&nbsp;The page offset, used in conjunction with 'max'. |


## Response

JSON containing a list of files and folders. The metadata for each item is the same that returned by the /metadata endpoint.

**Example:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
