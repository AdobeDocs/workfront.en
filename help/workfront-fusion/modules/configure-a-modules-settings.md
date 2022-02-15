---
filename: configure-a-modules-settings
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
---



# Configure a module's settings {#configure-a-modules-settings}

You must configure settings for every module you create. 


For example, the [Dropbox modules](dropbox-modules.md) modules require you to specify the target folder where you want to upload files. For the [Email modules](email-modules.md) modules, you need to enter the email address where emails should be sent. 


>[!NOTE]
>
>Besides the module settings, you can also adjust settings for a scenario. You can rename your scenario, change its schedule, and specify additional settings, just to name a few of the possibilities.




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


## Configure a module's settings {#configure-a-modules-settings-1}




1.  Add a new module to a scenario.


   Or


   Click the icon of the module in the scenario editor, as described in [Create a scenario](create-a-scenario.md).

1.  If required for the module, create a `Connection` to your registered user account for that given service, as described in [About connecting Adobe Workfront Fusion to an app or service](about-connecting-wf-fusion-to-app-or-service.md).
1.  In each field, type the appropriate text.


   Or


   Click `Map` if it appears to the right of the field, then map an item from another module in your scenario.


   Bolded parameters are required.


   For information about the different item data types *`Workfront Fusion`* can recognize (such as date, number, and text), see [Item data types](item-data-types.md).

1. (Conditional) If the module has advanced options you want to display and use, select `Show advanced settings`.


