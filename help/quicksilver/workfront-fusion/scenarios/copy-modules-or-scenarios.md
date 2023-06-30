---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copy modules or scenarios in [!DNL Adobe Workfront Fusion]
description: Copy modules or scenarios in [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
---
# Copy modules or scenarios in [!DNL Adobe Workfront Fusion]

You can copy modules, groups of modules, or entire scenarios in [!DNL Adobe Workfront Fusion]. This ability allows you to reuse scenarios or parts of scenarios without having to build them again

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

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisites

You must add modules to a scenario before you can copy them.

## Copy a module or a group of modules

When you copy a module, the copy retains all of the field values and settings of the original module.

You can paste the module or modules into another area of the same scenario, or into a different scenario.

Consider the following when pasting modules into a different scenario.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Any field values that pull information from another module that you did not copy can no longer access that information. You must set these fields to pull information from the new scenario.
* If you paste the modules into a scenario owned by another team or organization, all connections must be updated to connections owned by the group or organization that owns the new scenario.

### Copy modules

Copying a group of modules is similar to copying a single module.

1. Right-click on the module that you want to copy.

   >[!NOTE]
   >
   >You can select more than one module by holding [!UICONTROL shift] and clicking on the modules that you want to copy. Copying a group of modules also copies any connecting lines, filters, or routing logic between them.

1. Select **[!UICONTROL Copy module]**.
1. Move the cursor to the area of the scenario where you want the copy of the scenario.
1. Right click, and select **[!UICONTROL Paste]**.
1. Connect the pasted modules to the scenario by dragging them to the appropriate location in the scenario.

   You can also use keyboard shortcuts to copy and paste.

## Copy a scenario by cloning

Cloning a scenario creates a copy of the scenario, which you can then edit.

1. Open the scenario detail page:

   1. Click the **[!UICONTROL Scenario]** tab in the left panel, then click a scenario you would like details on.

      Or

      If you are working on the scenario in the [The scenario editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), click the left arrow ![](assets/exit-editing-arrow.png) near the upper-left corner of the window.

1. Right click **[!UICONTROL Options]** at the upper-right of the page.
1. Select **[!UICONTROL Clone]**.
1. (Optional) Enter a name for the new scenario.
1. (Optional) Enable **[!UICONTROL Keep the states of any new modules the same as those being duplicated]** to ensure that the copied scenario also includes information about the most recent records processed by the original scenario.
1. Click **[!UICONTROL Save]** to create the scenario.

## Copy a scenario by using blueprints

Scenario blueprints represent the arrangement, mapping, and field values of a given scenario at a given point in time. You can export a scenario blueprint into a JSON file on your computer, then import it when creating a new scenario. Scenarios imported from a scenario blueprint can be edited.

A scenario blueprint represents the entire scenario. If you want to copy only certain modules from a scenario, see [Copy a module or a group of modules](#copy-a-module-or-a-group-of-modules) in this article.

>[!NOTE]
>
>For information on blueprints in the context of [!DNL Adobe Workfront], see [Blueprints overview](../../administration-and-setup/blueprints/blueprints-overview.md).

### Export a scenario blueprint

1. In the scenario, click the **[!UICONTROL More]** menu in the scenario settings area.
1. Click **[!UICONTROL Export Blueprint]**.

   A JSON file is created and downloads to your computer. You can locate this file in your [!DNL Downloads] folder.

### Import a blueprint

>[!IMPORTANT]
>
>If you import a blueprint to an existing scenario, the scenario blueprint replaces the existing scenario. You cannot append a blueprint onto an existing scenario.

1. Begin creating a new scenario.
1. In the scenario, click the **[!UICONTROL More]** menu in the scenario settings area.
1. Click **[!UICONTROL Import Blueprint]**.
1. In the dialog that appears, click **[!UICONTROL Browse]**
1. Navigate to the blueprint you want to import, and click **[!UICONTROL Open]**.
1. Click **[!UICONTROL Save]**.

   A JSON file is created and downloads to your computer. You can locate this file in your [!UICONTROL Downloads] folder.

## Copy and reuse scenarios by using templates

You can create templates as a starting point for your [!DNL Workfront Fusion] scenarios. When you create a scenario from a template, you can modify the scenario without modifying the template. Field values are not saved in templates.

For more information on creating and using templates, see [Scenario Templates](../../workfront-fusion/scenarios/templates/fusion-templates.md).
