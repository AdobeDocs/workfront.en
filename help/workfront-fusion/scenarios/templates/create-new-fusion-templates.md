---
filename: create-new-fusion-templates
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
---



# Create new templates in *`Adobe Workfront Fusion`* {#create-new-templates-in-adobe-workfront-fusion}

You can create new scenario templates in *`Adobe Workfront Fusion`*.


>[!TIP] {type="tip"}
>
>Before creating a new template, you can check the Public templates tab to ensure that the template you want to create is not already available.




## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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


## Create a new template {#create-a-new-template}




1.  Click `Templates` ![](assets/fusion-template-icon.png) in the left navigation panel.
1.  Click `Create a new template` in the top-right corner.
1.  (Optional) Rename the template by replacing the default `New template name` in the top-left corner.
1.  (Optional) To change the language of your template, click Set up a template ![](assets/fusion-scenario-settings-icon.png) and select the language from the Language drop-down. 


   >[!IMPORTANT] {type="important"}
   >
   >The Languages selection corresponds to the languages available in the system settings and concerns only the name of the public template and its description. You can't change a template language once the template has been saved.



1.  (Optional) To enter a description of the template, click Set up a template ![](assets/fusion-scenario-settings-icon.png) and enter the description.
1.  Add apps, modules, and tools in the same way as you would do when creating a standard scenario. 


   To add contextual help to the modules, see [Set up Wizard functionality](#wizard) in this article.


   For more information on building a scenario, see [Create a scenario](create-a-scenario.md).


   >[!NOTE]
   >
   >If your template includes modules that require adding the connection, credentials, or other privacy-sensitive information, this information is not shared with the template users.



1.  (Optional) Click `Run once` to test your template.
1.  Click the `Save` icon ![](assets/save-icon.png).




>[!NOTE]
>
>By saving your template you make it visible for all your team members. If you want your template to be accessible outside of your team you need to publish it and then use a shared link, or ask your administrator to approve and publish the template.




## Set up Wizard functionality {#set-up-wizard-functionality}

The *`Workfront Fusion`* template wizard allows you to provide future users of your template with instructions or information related to the specific fields used in modules. 



1.  Click the module added to the template to see the module's fields.
1.  Locate the field where you want to add Wizard information, and enable `Use in Wizard` for that field.
1.  Enter the information you want to make visible for users into the Help field.
1.  (Optional) To allow users to see this text when using the template, enable `Use as default value`.
1.  Repeat steps 2-4 for each field that you want to provide information for.
1.  Click `OK` to save changes and close the module.


