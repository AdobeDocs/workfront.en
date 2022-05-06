---
filename: rename-docu-or-folder
content-type: api
navigation-topic: documents-webhooks-api
title: Rename a document or folder (not yet implemented)
description: Renames a document or folder with the given ID in the external system.
---

# Rename a document or folder (not yet implemented)

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Renames a document or folder with the given ID in the external system.

## URL

PUT /rename

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| id |The document or folder ID to rename |
| name&nbsp; |The new name of the document or folder |

&nbsp;

## Response

A JSON string indicating success or failure, as specified in the Error Handling section below.

``` ```**Example: **``````PUT&nbsp;https://www.acme.com/api/rename

-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------

returns
<pre>{</pre><pre>status: “success”</pre><pre>}</pre>returns
<pre>{</pre><pre>status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”</pre><pre>}</pre>