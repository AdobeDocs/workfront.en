---
filename: choose-where-trigger-module-starts
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Choose where a trigger module starts in Adobe Workfront Fusion
description: Some trigger modules allow you to select the first bundle from which you want the retrieving of bundles to start.
---

# Choose where a trigger module starts in Adobe Workfront Fusion

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Some trigger modules allow you to select the first bundle from which you want the retrieving of bundles to start.

You can also specify whether you want to retrieve all bundles or just the bundles from after a specific date.

For more information about trigger modules, see the section [Trigger modules](../../workfront-fusion/modules/module-types.md#triggers) in the article [Types of modules](../../workfront-fusion/modules/module-types.md).

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

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Choose where a trigger module starts

1. Save a trigger module.

   Or

   Change the trigger module's settings as described in [Configure a module's settings in Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Or

   Right-click the icon for the trigger module in the Scenario editor, as described in [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Select an option in the **Choose where to start** box that appears.

   ![](assets/choose-where-to-start-350x346.jpg)

   The options displayed depend on the possibilities of a given service. They may include the following:

   | From now on (default) |Retrieves all bundles added or updated (depending on settings) from now on |
   |---|---|
   | From after a specific date |Retrieves all bundles added or updated (depending on settings) after a specified date/time |
   | With ID greater than or equal to a specific value |Retrieves all bundles with an ID greater than or equal to a specified ID |
   | All bundles |Retrieves all available bundles |
   | Select the first bundle |Allows you to select the first bundle from which the retrieval of bundles is to start |

