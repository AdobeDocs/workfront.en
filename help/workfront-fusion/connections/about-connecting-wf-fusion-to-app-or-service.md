---
filename: about-connecting-wf-fusion-to-app-or-service
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
---



# About connecting *`Adobe Workfront Fusion`* to an app or service {#about-connecting-adobe-workfront-fusion-to-an-app-or-service}

For most apps, it is necessary to create a connection, through which *`Adobe Workfront Fusion`* can communicate with the given third-party service according to the settings of the specific scenario. 


For example, if you want to create a scenario that retrieves information from Google Sheets, you must grant access permission for *`Workfront Fusion`* to access your Google account.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Access rights {#access-rights}

For every connection, *`Workfront Fusion`* requires only those access rights that are necessary to successfully complete a given scenario. For example, if you create a scenario to list documents from Google Docs, *`Workfront Fusion`* does not ask for permission to get the content of the documents.


Unfortunately, not all services allow you to limit access to specific tasks. Therefore, *`Workfront Fusion`* must require full access rights. For more information on how to restrict *`Workfront Fusion`* access to your account registered to those services, see the application-specific documentation.


## About administering connections {#about-administering-connections}

You can administer all connections from one place in the Connections section. Here you can:



*   See which permissions were given to *`Workfront Fusion`* for each connection
*  Rename connections 
*  Reauthorize existing connections
*  Delete existing connections
*  Verify that the connection to the service was established successfully




## Renew a connection {#renew-a-connection}

*`Workfront Fusion`* usually obtains access rights to a given service for an unlimited period of time. However, this is not always the case. With some services, the access permission must be renewed after a certain period of time. In these cases, *`Workfront Fusion`* notifies you via email shortly before its access rights expire. 


To renew a connection:



1. Click the `Reauthorize` button in the `Connections` section.



