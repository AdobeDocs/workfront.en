---
filename: get-service-info-webhook
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Get information about the service (not yet implemented) {#get-information-about-the-service-not-yet-implemented}



>[!NOTE]
>
>The release date for this feature is yet to be determined.


Returns information about the service, such as features and capabilities. *`Adobe Workfront`* will use this information to customize the user interface in *`Workfront`*. For example, if the webhook implementation contains some custom actions, the JSON should list those operations in the JSON. Users would then be able to invoke these actions from *`Workfront`*.


## URL {#url}

GET /serviceInfo


## Query Parameters {#query-parameters}

None. In addition, calls to this endpoint should not require authentication.


## Response {#response}

JSON containing information about this service

<table style="height: 134px;width: 685px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Name</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Type&nbsp;</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">webhookVersion&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The webhook version implemented by this service. This is the version&nbsp;number listed at the top of this spec.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">version&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The internal version number for this service. This number is determined by the webhook service provider and is used for informational purposes only.<br><br></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">publisher&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The name of the company providing the webhook implementation.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">availableEndpoints</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">String&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">A list containing the API Endpoints implemented by this service. This may be used to ensure that the user interface in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> reflect the capabilities offered by the webhook provider. Each item in the list must include the name of the endpoint (such as “search”).</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">customActions&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">String</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">&nbsp; <p>A list containing the custom operations implemented by this webhook. Each list item includes a name and display name. The display name will appear in the “Document Actions” dropdown in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. Clicking on the item in the dropdown will invoke the action in the webhook by calling the /customAction endpoint.</p></td> 
  </tr> 
 </tbody> 
</table>

` `**Example: **`` `https://www.acme.com/api/serviceInfo` 


returns
`<pre>{<br>webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”<br>“thumbnail”, “uploadInit”, “upload” ], customActions [<br>{<br>name: “archive”, displayName: “Archive” }, {<br>name: “doSomethingElse”, displayName: “Do Something” }, ] }</pre>`  