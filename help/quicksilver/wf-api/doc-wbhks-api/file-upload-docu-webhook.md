---
filename: file-upload-docu-webhook
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: File upload via Document Webhooks
description: Uploading a file to a document storage provider is a two-step process that requires two separate API endpoints. Adobe Workfront begins the upload process by calling /uploadInit . This endpoint returns a document ID which is then passed to /upload when uploading the document bytes. Depending on the underlying document storage system, it might be necessary to create a zero-length document, then update the contents of the document later.
---

# File upload via Document Webhooks

Uploading a file to a document storage provider is a two-step process that requires two separate API endpoints. Adobe Workfront begins the upload process by calling /uploadInit . This endpoint returns a document ID which is then passed to /upload when uploading the document bytes. Depending on the underlying document storage system, it might be necessary to create a zero-length document, then update the contents of the document later.

Added to version 1.1 of this spec, the document ID and document version ID can be used to retrieve extra information from Workfront.

**Example:** If the document management system wants extra information about the document, the webhook implementation code could use the document ID to retrieve that information using Workfront’s RESTful API. As a good practice, this information could come from custom data fields on the document and it’s containing task, issue, or project.

## Part 1

## URL

POST /uploadInit

## Query Parameters

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name&nbsp;</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId&nbsp;</td> 
   <td>The parent folder ID, as referenced by the webhook provider.</td> 
  </tr> 
  <tr> 
   <td>filename&nbsp;</td> 
   <td>The name of the document</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>The Workfront document ID (added in version 1.1)</p> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId&nbsp;</td> 
   <td>The Workfront document version ID (added in version 1.1)&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

## Response

The metadata for the file, as defined by the /metadata endpoint.

**Example:** https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b

response

[file_metadata] ­ includes the new document ID used by the document provider.

## Part 2

Uploads the bytes of a document to the webhook provider.

## URL

PUT /upload

## Query Parameters

| Name&nbsp; |Description |
|---|---|
| id&nbsp; |&nbsp;The document ID, which was just created. |

**Request Body**

The raw content bytes for the document.

**Response** 
<pre>{<br>result: “success”<br>}<br>or<br>{<br>result: “fail”<br>}</pre><pre>https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]</pre>response
<pre>{<br>result:"success"<br>}</pre>