---
filename: receive-a-webhook-from-a-web-service
product: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
---



# Receive a webhook from a web service {#receive-a-webhook-from-a-web-service}

If a web service is not currently implemented as an app in *`Adobe Workfront Fusion`*, but it supports sending webhooks, you can add the service to a scenario using the Custom webhook module as an instant trigger.


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


## Receive a webhook {#receive-a-webhook}




1. Add the `Webhooks > Custom webhook` module to your scenario.
1. Click `Add`, type a `Webhook name` in the box that displays, then click `Save`. 

1. Click `Copy address to clipboard`, then click `OK`.

1. Log in to the web service and do the following there:
    
    
    1. In the Settings area for the web service, create a webhook.
    1. Paste the address you copied to your clipboard in step 3 .
    1. Select the event that will trigger the webhook.
    
    
1. In the *`Workfront Fusion`* scenario, specify the event or events that you want to trigger the Custom webhook module.
1.  Run the scenario.


   When the event or events occur, the Custom webhook module triggers and the scenario runs.



