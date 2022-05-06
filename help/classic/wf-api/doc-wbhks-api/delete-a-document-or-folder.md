---
filename: delete-a-document-or-folder
content-type: api
navigation-topic: documents-webhooks-api
title: Delete a document or folder (Not yet implemented)
description: Note: The release date for this feature is yet to be determined.
---

# Delete a document or folder (Not yet implemented)

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

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

&nbsp;&nbsp;

Response A JSON string indicating success or failure, as specified in the Error Handling section below.

## Example

<pre>PUT https://www.acme.com/api/delete ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­ id=1234 ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­</pre>returns
<pre>{</pre><pre>status: “success” </pre><pre>}</pre>returns
<pre>{</pre><pre>status: “failure”, error: “File not found”</pre><pre>}</pre>