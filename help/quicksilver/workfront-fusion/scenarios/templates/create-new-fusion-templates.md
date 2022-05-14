---
filename: create-new-fusion-templates
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Create new templates in Adobe Workfront Fusion
description: You can create new scenario templates in Adobe Workfront Fusion.
---

# Create new templates in Adobe Workfront Fusion

You can create new scenario templates in Adobe Workfront Fusion.

>[!TIP]
>
>Before creating a new template, you can check the Public templates tab to ensure that the template you want to create is not already available.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Create a new template

1. Click **Templates** ![](assets/fusion-template-icon.png) in the left navigation panel.
1. Click **Create a new template** in the top-right corner.
1. (Optional) Rename the template by replacing the default **New template name** in the top-left corner.
1. (Optional) To change the language of your template, click **Set up a template** ![](assets/fusion-scenario-settings-icon.png) and select the language from the Language drop-down.

   >[!IMPORTANT]
   >
   >The Languages selection corresponds to the languages available in the system settings and concerns only the name of the public template and its description. You can't change a template language once the template has been saved.

1. (Optional) To enter a description of the template, click **Set up a template** ![](assets/fusion-scenario-settings-icon.png) and enter the description.
1. Add apps, modules, and tools in the same way as you would do when creating a standard scenario.

   To add contextual help to the modules, see [Set up Wizard functionality](#set-up-wizard-functionality) in this article.

   For more information on building a scenario, see [Create a scenario in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >If your template includes modules that require adding the connection, credentials, or other privacy-sensitive information, this information is not shared with the template users.

1. (Optional) Click **Run once** to test your template.
1. Click the **Save** icon ![](assets/save-icon.png).

>[!NOTE]
>
>By saving your template you make it visible for all your team members. If you want your template to be accessible outside of your team you need to publish it and then use a shared link, or ask your administrator to approve and publish the template.

## Set up Wizard functionality {#set-up-wizard-functionality}

The Workfront Fusion template wizard allows you to provide future users of your template with instructions or information related to the specific fields used in modules.

1. Click the module added to the template to see the module's fields.
1. Locate the field where you want to add Wizard information, and enable **Use in Wizard** for that field.
1. Enter the information you want to make visible for users into the Help field.
1. (Optional) To allow users to see this text when using the template, enable **Use as default value**.
1. Repeat steps 2-4 for each field that you want to provide information for.
1. Click **OK** to save changes and close the module.

