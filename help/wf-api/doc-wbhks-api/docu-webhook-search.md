---
filename: docu-webhook-search
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Search via Document Webhooks {#search-via-document-webhooks}

Returns metadata for the files and folders returned from a search. This can be implemented as a full-text search or as a regular database query. *`Adobe Workfront`* calls the /search endpoint when the user performs a search from the external file browser.


## URL {#url}

GET /search


## Query Parameters {#query-parameters}


<table style="width: 607px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Name&nbsp;</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">query</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The search term or phrase.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">parentId</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>(optional) The folder ID from which the search executed. Note: This is a placeholder for a future feature in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. Currently, workfront does not pass this parameter.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">max</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The maximum number of items to return. Used for pagination.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">offset</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">&nbsp;The page offset, used in conjunction with ‘max’.</td> 
  </tr> 
 </tbody> 
</table>

&nbsp;


## Response {#response}

JSON containing a list of metadata for files and folders matching the query. What constitutes a “match” is determined by the webhook provider. Ideally, it should do a full-text search. Doing a filename-based search also works.


` `**Example: **``Example:  `https://www.acme.com/api/search?query=test-query`
`<pre>[<br> { File/Folder Metadata },<br> { File/Folder Metadata }<br> ]</pre>` 