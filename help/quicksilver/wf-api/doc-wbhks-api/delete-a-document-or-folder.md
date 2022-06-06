---
filename: delete-a-document-or-folder
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Delete a document or folder (Not yet implemented)
description: "Note: The release date for this feature is yet to be determined."
---

# Delete a document or folder (Not yet implemented)

>[!NOTE]
>
>The release date for this feature is yet to be determined.

Deletes a document or folder with the given ID in the external system. Deleting a folder also deletes the folder contents.

## URL

PUT /delete

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| documentId&nbsp; |The document ID to delete |
| folderId&nbsp; |&nbsp;The folder ID to delete |

{style="table-layout:auto"}

&nbsp;&nbsp;

Response A JSON string indicating success or failure, as specified in the Error Handling section below.

## Example

<pre>PUT https://www.acme.com/api/delete ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­ id=1234 ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­</pre>returns
<pre>{</pre><pre>status: “success” </pre><pre>}</pre>returns
<pre>{</pre><pre>status: “failure”, error: “File not found”</pre><pre>}</pre>