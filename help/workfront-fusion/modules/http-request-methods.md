---
filename: http-request-methods
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
---



# HTTP request methods {#http-request-methods}

When you are configuring an API call in a module, you need to fill in the field for the HTTP request method.


## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## HTTP methods {#http-methods}

Use one of the following HTTP methods.



* `GET`: Retrieves data from a web server based on your parameters. GET requests a representation of the specified resource, and receives a 200 OK response message with the requested content if successful.
* `POST`: Sends data to a web server based on your parameters. POST requests include actions like uploading a file. Multiple POSTs may result in a different outcome than a single POST, so be cautious about unintentionally sending multiple POSTs. If a POST is successful, you receive a 200 OK response message.
* `PUT`: Sends data to a location in the web server based on your parameters. PUT requests include actions like uploading a file. The difference between a PUT and POST is that PUT is idempotent, meaning that the result of a single successful PUT is the same as many identical PUTs. If a PUT is successful, you receive a 200 response message (usually 201 or 204).
*  `PATCH`: (Not available for some API call modules) Applies partial modifications to a resource on a web server based on your parameters. PATCH is not idempotent, meaning that the result of multiple PATCH’s could have unintended consequences. If a PUT is successful, you will receive a 200 response message (usually 204).
* `DELETE`: Deletes the specified resource from the web server based on your parameters (if the resource exists). If a DELETE is successful, you receive a 200 OK response message.


