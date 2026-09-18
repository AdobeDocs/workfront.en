---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Rename a document or folder (not yet implemented)
description: Rename a document or folder
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
---
# Rename a document or folder (not yet implemented)

Renames a document or folder with the given ID in the external system.

**URL**

PUT /rename

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| id |The document or folder ID to rename |
| name&nbsp; |The new name of the document or folder |


## Response

A JSON string indicating success or failure, as specified in the Error Handling section below.

**Example:** PUT&nbsp;https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

returns

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
