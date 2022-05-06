---
filename: docu-webhook-search
content-type: api
navigation-topic: documents-webhooks-api
title: Search via Document Webhooks
description: Returns metadata for the files and folders returned from a search. This can be implemented as a full-text search or as a regular database query. Adobe Workfront calls the /search endpoint when the user performs a search from the external file browser.
---

# Search via Document Webhooks

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Returns metadata for the files and folders returned from a search. This can be implemented as a full-text search or as a regular database query. Adobe Workfront calls the /search endpoint when the user performs a search from the external file browser.

## URL

GET /search

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
   <td>query</td> 
   <td>The search term or phrase.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(optional) The folder ID from which the search executed. Note: This is a placeholder for a future feature in Workfront. Currently, workfront does not pass this parameter.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>The maximum number of items to return. Used for pagination.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td>&nbsp;The page offset, used in conjunction with ‘max’.</td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

## Response

JSON containing a list of metadata for files and folders matching the query. What constitutes a “match” is determined by the webhook provider. Ideally, it should do a full-text search. Doing a filename-based search also works.

``` ```**Example: **``````Example:  ```https://www.acme.com/api/search?query=test-query```
<pre>[<br> 
{ File/Folder Metadata },<br> 
{ File/Folder Metadata }<br> 
]</pre>