---
filename: perform-custom-action
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Perform a custom action (not yet implemented) {#perform-a-custom-action-not-yet-implemented}

This endpoint allows an *`Adobe Workfront`* user (or an automated workflow event) to perform an action in the external system. The /customAction endpoint accepts a “name” parameter, which allows the webhook provider to implement multiple custom operations.


The webhook provider registers custom actions with *`Workfront`* by including the actions in the /serviceInfo response under customActions. *`Workfront`* loads this list when setting up or refreshing the webhook provider under Setup > Documents > Custom Integrations.


Users can trigger the custom action by selecting the section under “Document Actions”


## URL {#url}

GET /customAction


## Query Parameters {#query-parameters}


<table style="height: 72px;width: 697px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
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
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>name</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The identifier specifying the type of action to be performed. This value corresponds to one of the customAction values listed returned by the /serviceInfo endpoint.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">documentId&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The workfront document ID for which the action is being performed.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">documentVersionId&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">&nbsp;The workfront document version ID for which the action is being performed.</td> 
  </tr> 
 </tbody> 
</table>

&nbsp;


## Response {#response}

A JSON string indicating success or failure, as specified in the Error Handling section below. On failure (i.e. status = “failure”), *`Workfront`* will display the provided error message to the user.


` `**Example: **``https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3


response
`<pre>{</pre>``<pre>status: “success”</pre>``<pre>}</pre>`  