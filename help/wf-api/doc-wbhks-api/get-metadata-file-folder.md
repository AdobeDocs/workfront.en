---
filename: get-metadata-file-folder
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Get metadata for a file or folder {#get-metadata-for-a-file-or-folder}



### Get metadata for file or folder {#get-metadata-for-file-or-folder}

Returns metadata for the specified file or folder.


## URL {#url}

GET /metadata?id=[document or folder ID]


## Query Parameters {#query-parameters}


<table style="height: 153px;width: 725px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 69px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Name&nbsp;</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">id</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The ID of file or folder, as referenced by the webhook provider. This is different than <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span>’s document ID. To get the metadata of the root directory, use the value ‘/’.</p> <p>Note: The maximum length for the ID is 255 characters.</p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

## Response {#response}



<table style="height: 238px;width: 621px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Name&nbsp;</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Type&nbsp;</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">title&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The name of the document or folder</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">kind&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Specifies if this item is a file or folder (‘file’ or ‘folder’)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">id</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The id of the file or folder.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">viewLink</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The URL path used by a user to view the document in a browser window. The URL can be hosted by either the document provider or the native external storage provider.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">downloadLink</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The URL path used by a user to download the document in a browser window. The URL can be hosted by either the document provider or the native external storage provider.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">mimeType</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The MIME type for the file. (optional)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">dateModified</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Last time this file was modified (formatted RFC 3339 timestamp)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">size</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Long</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;The size of the file in bytes. (optional)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">readOnly</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Boolean</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> Indicates if this file or folder is read-only to the authenticated user.(optional) </td> 
  </tr> 
 </tbody> 
</table>

` `**Example: **``https://www.acme.com/api/metadata?id=12345
`<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345”,<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"2014­06­05T17:39:45.251Z",<br>size: "32554694"<br>}</pre>` 

>[!NOTE]
>
>Error handling should be consistent across all API calls. See the “Error Handling” section below for details.


