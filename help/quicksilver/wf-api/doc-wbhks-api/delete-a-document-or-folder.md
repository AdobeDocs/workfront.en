---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Delete a document or folder
description: Delete a document or folder
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
TQID: https://experienceleague.adobe.com/7-f8Z3qQQ2z7ZHHfSrGgJqIQCKdeqEoL96XlfCGzYSo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
---
# Delete a document or folder (not yet implemented)

Deletes a document or folder with the given ID in the external system. Deleting a folder also deletes the folder contents.

## URL

PUT /delete

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| documentId&nbsp; |The document ID to delete |
| folderId&nbsp; |&nbsp;The folder ID to delete |



## Response 

A JSON string indicating success or failure, as specified in the Error Handling section below.

### Example

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
