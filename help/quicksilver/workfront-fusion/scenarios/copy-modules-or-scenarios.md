---
filename: copy-modules-or-scenarios
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copy modules or scenarios
description: 
---

# Copy modules or scenarios

You can copy modules, groups of modules, or entire scenarios in Adobe Workfront Fusion. This ability allows you to reuse scenarios or parts of scenarios without having to build them again

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
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

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

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
   >You can select more than one module by holding shift and clicking on the modules that you want to copy. Copying a group of modules also copies any connecting lines, filters, or routing logic between them.

1. Select **Copy module**.
1. Move the cursor to the area of the scenario where you want the copy of the scenario.
1. Right click, and select **Paste**.
1. Connect the pasted modules to the scenario by dragging them to the appropriate location in the scenario.

   You can also use keyboard shortcuts to copy and paste.

## Copy a scenario by cloning

Cloning a scenario creates a copy of the scenario, which you can then edit.

1. Open the scenario detail page:

  1. Click the **Scenario** tab in the left panel, then click a scenario you would like details on.

     Or

     If you are working on the scenario in the [Scenario editor](../../workfront-fusion/scenarios/scenario-editor.md), click the left arrow ![](assets/exit-editing-arrow.png) near the upper-left corner of the window.

1. Right click **Options** at the upper-right of the page.
1. Select **Clone**.
1. (Optional) Enter a name for the new scenario.
1. (Optional) Enable **Keep the states of any new modules the same as those being duplicated** to ensure that the copied scenario also includes information about the most recent records processed by the original scenario.
1. Click **Save** to create the scenario.

## Copy a scenario by using blueprints

Scenario blueprints represent the arrangement, mapping, and field values of a given scenario at a given point in time. You can export a scenario blueprint into a JSON file on your computer, then import it when creating a new scenario. Scenarios imported from a scenario blueprint can be edited.

A scenario blueprint represents the entire scenario. If you want to copy only certain modules from a scenario, see [Copy a module or a group of modules](#copy) in this article.

>[!NOTE]
>
>For information on blueprints in the context of Adobe Workfront, see [Blueprints overview](../../administration-and-setup/blueprints/blueprints-overview.md).

### Export a scenario blueprint

1. In the scenario, click the **More** menu in the scenario settings area.
1. Click Export Blueprint.

   A JSON file is created and downloads to your computer. You can locate this file in your Downloads folder.

### Import a blueprint

>[!IMPORTANT]
>
>If you import a blueprint to an existing scenario, the scenario blueprint replaces the existing scenario. You cannot append a blueprint onto an existing scenario.

1. Begin creating a new scenario.
1. In the scenario, click the **More** menu in the scenario settings area.
1. Click **Import Blueprint**.
1. In the dialog that appears, click **Browse**
1. Navigate to the blueprint you want to import, and click **Open**.
1. Click **Save**.

   A JSON file is created and downloads to your computer. You can locate this file in your Downloads folder.

## Copy and reuse scenarios by using templates

You can create templates as a starting point for your Workfront Fusion scenarios. When you create a scenario from a template, you can modify the scenario without modifying the template. Field values are not saved in templates.

For more information on creating and using templates, see [Scenario Templates](../../workfront-fusion/scenarios/templates/fusion-templates.md).
