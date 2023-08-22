---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Create new templates in [!DNL Adobe Workfront Fusion]
description: You can create new scenario templates in [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
---
# Create new templates in [!DNL Adobe Workfront Fusion]

You can create new scenario templates in [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Before creating a new template, you can check the [!UICONTROL Public templates] tab to ensure that the template you want to create is not already available.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
  <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Create a new template

You can build a template in a process similar to building a scenario. Fusion administrators can also create templates from existing scenarios.

* [Build a template](#build-a-template)
* [Create a template from a scenario](#create-a-template-from-a-scenario)

### Build a template

1. Click **[!UICONTROL Templates]** ![](assets/fusion-template-icon.png) in the left navigation panel.
1. Click **[!UICONTROL Create a new template]** in the upper-right corner.
1. (Optional) Rename the template by replacing the default **[!UICONTROL New template name]** in the upper-left corner.
1. (Optional) To change the language of your template, click **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) and select the language from the Language drop-down.

   >[!IMPORTANT]
   >
   >The Languages selection corresponds to the languages available in the system settings and concerns only the name of the public template and its description. You can't change a template language once the template has been saved.

1. (Optional) To enter a description of the template, click **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) and enter the description.
1. Add apps, modules, and tools in the same way as you would do when creating a standard scenario.

   To add contextual help to the modules, see [Set up [!UICONTROL Wizard] functionality](#set-up-wizard-functionality) in this article.

   For more information on building a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >If your template includes modules that require adding the connection, credentials, or other privacy-sensitive information, this information is not shared with the template users.

1. (Optional) Click **[!UICONTROL Run once]** to test your template.
1. Click the **[!UICONTROL Save]** icon ![](assets/save-icon.png).

>[!NOTE]
>
>By saving your template you make it visible for all your team members. If you want your template to be accessible outside of your team you must submit a request to have it approved and published. The request comes to Adobe Workfront for approval and once it is approved the template is accessible by others outside of your team.

### Create a template from a scenario

>[!NOTE]
>
>You must be a Fusion administrator to create a template from a scenario. 

1. Open the scenario details page for the scenario that you want to create a scenario from.
1. Click the **Admin** drop down near the upper-right corner of the page.
1. Select **Clone as template**.
   
   The scenario is copied into a New template page.
1. (Optional) Rename the template by replacing the default **[!UICONTROL New template name]** in the upper-left corner.
1. (Optional) To change the language of your template, click **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) and select the language from the Language drop-down.

   >[!IMPORTANT]
   >
   >The Languages selection corresponds to the languages available in the system settings and concerns only the name of the public template and its description. You can't change a template language once the template has been saved.

1. (Optional) To enter a description of the template, click **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) and enter the description.
1. Edit apps, modules, and tools in the same way as you would do when editing a standard scenario.

   To add contextual help to the modules, see [Set up [!UICONTROL Wizard] functionality](#set-up-wizard-functionality) in this article.

   >[!NOTE]
   >
   >If your template includes modules that require adding the connection, credentials, or other privacy-sensitive information, this information is not shared with the template users.

1. (Optional) Click **[!UICONTROL Run once]** to test your template.
1. Click the **[!UICONTROL Save]** icon ![](assets/save-icon.png).

## Set up [!UICONTROL Wizard] functionality {#set-up-wizard-functionality}

The [!DNL Workfront Fusion template] [!UICONTROL Wizard] allows you to provide future users of your template with instructions or information related to the specific fields used in modules.

1. Click the module added to the template to see the module's fields.
1. Locate the field where you want to add [!UICONTROL Wizard] information, and enable **[!UICONTROL Use in Wizard]** for that field.
1. Enter the information you want to make visible for users into the [!UICONTROL Help] field.
1. (Optional) To allow users to see this text when using the template, enable **[!UICONTROL Use as default value]**.
1. Repeat steps 2-4 for each field that you want to provide information for.
1. Click **[!UICONTROL OK]** to save changes and close the module.
