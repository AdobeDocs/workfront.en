---
filename: configure-a-modules-settings
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Configure a module's settings
description: You must configure settings for every module you create.
---

# Configure a module's settings

You must configure settings for every module you create.

For example, the [Dropbox modules](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) modules require you to specify the target folder where you want to upload files. For the [Email modules](../../workfront-fusion/apps-and-their-modules/email-modules.md) modules, you need to enter the email address where emails should be sent.

>[!NOTE]
>
>Besides the module settings, you can also adjust settings for a scenario. You can rename your scenario, change its schedule, and specify additional settings, just to name a few of the possibilities.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> <draft-comment>
     <p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p>
    </draft-comment><p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Configure a module's settings

1. Add a new module to a scenario.

   Or

   Click the icon of the module in the scenario editor, as described in [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

1. If required for the module, create a `Connection` to your registered user account for that given service, as described in [About connecting Adobe Workfront Fusion to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. In each field, type the appropriate text.

   Or

   Click `Map` if it appears to the right of the field, then map an item from another module in your scenario.

   Bolded parameters are required.

   For information about the different item data types *Workfront Fusion* can recognize (such as date, number, and text), see [Item data types](../../workfront-fusion/mapping/item-data-types.md).

1. (Conditional) If the module has advanced options you want to display and use, select `Show advanced settings`.

