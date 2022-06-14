---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Rename a document or folder (not yet implemented)
description: Renames a document or folder with the given ID in the external system.
feature: "Workfront API, Digital Content and Documents"
---

# Rename a document or folder (not yet implemented)

Renames a document or folder with the given ID in the external system.

## URL

PUT /rename

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| id |The document or folder ID to rename |
| name&nbsp; |The new name of the document or folder |

{style="table-layout:auto"}

&nbsp;

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
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
