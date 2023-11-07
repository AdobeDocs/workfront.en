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
---

# Delete a document or folder (Not yet implemented)

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

PUT https://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234 ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­
* ­returns `status: "success"`

* returns `status: "failure", error: "File not found"`
