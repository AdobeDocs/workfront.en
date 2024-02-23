---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Search via Document Webhooks
description: Search via Document Webhooks
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
---
# Search via Document Webhooks

Returns metadata for the files and folders returned from a search. This can be implemented as a full-text search or as a regular database query. Adobe Workfront calls the /search endpoint when the user performs a search from the external file browser.

## URL

GET /search

## Query Parameters

<table style="table-layout:auto"> 
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
   <td>&nbsp;The page offset, used in conjunction with 'max'.</td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

## Response

JSON containing a list of metadata for files and folders matching the query. What constitutes a "match" is determined by the webhook provider. Ideally, it should do a full-text search. Doing a filename-based search also works.

**Example:** 

Example:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
