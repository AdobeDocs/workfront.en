---
filename: get-metadata-file-folder
content-type: api
navigation-topic: documents-webhooks-api
title: Get metadata for a file or folder
description: Returns metadata for the specified file or folder.
---

# Get metadata for a file or folder

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Get metadata for file or folder

Returns metadata for the specified file or folder.

## URL

GET /metadata?id=[document or folder ID]

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
   <td>id</td> 
   <td> <p>The ID of file or folder, as referenced by the webhook provider. This is different than Adobe Workfront’s document ID. To get the metadata of the root directory, use the value ‘/’.</p> <p>Note: The maximum length for the ID is 255 characters.</p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

## Response

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name&nbsp;</th> 
   <th>Type&nbsp;</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title&nbsp;</td> 
   <td>String&nbsp;</td> 
   <td>The name of the document or folder</td> 
  </tr> 
  <tr> 
   <td>kind&nbsp;</td> 
   <td>String&nbsp;</td> 
   <td>Specifies if this item is a file or folder (‘file’ or ‘folder’)</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String&nbsp;</td> 
   <td>The id of the file or folder.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String&nbsp;</td> 
   <td> <p>The URL path used by a user to view the document in a browser window. The URL can be hosted by either the document provider or the native external storage provider.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String&nbsp;</td> 
   <td> <p>The URL path used by a user to download the document in a browser window. The URL can be hosted by either the document provider or the native external storage provider.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String&nbsp;</td> 
   <td>The MIME type for the file. (optional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String&nbsp;</td> 
   <td>Last time this file was modified (formatted RFC 3339 timestamp)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Long</td> 
   <td>&nbsp;The size of the file in bytes. (optional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolean</td> 
   <td> Indicates if this file or folder is read-only to the authenticated user.(optional) </td> 
  </tr> 
 </tbody> 
</table>

**Example:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345”,<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"2014­06­05T17:39:45.251Z",<br>size: "32554694"<br>}</pre>

>[!NOTE]
>
>Error handling should be consistent across all API calls. See the “Error Handling” section below for details.

