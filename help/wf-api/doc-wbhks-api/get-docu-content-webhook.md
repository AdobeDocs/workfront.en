---
filename: get-docu-content-webhook
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Get document content via Webhooks {#get-document-content-via-webhooks}

Returns the raw bytes for a document


## URL {#url}

GET /download


## Query Parameters {#query-parameters}


<table style="height: 20px;width: 325.5px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
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
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>id</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">&nbsp;The document ID.</td> 
  </tr> 
 </tbody> 
</table>



## Response {#response}

The raw bytes of the document.


` `**Example: **``:&nbsp; [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
