---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Templates administration
description: If you are an administrator, you have permission to view, modify, rename, publish, approve, and delete templates created by others. You can perform these actions from the [!UICONTROL Templates] page in the [!DNL Adobe Workfront Fusion Administration] area.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
---
# Adobe Workfront Fusion Templates administration

If you are an administrator, you have permission to view, modify, rename, publish, approve, and delete templates created by others. You can perform these actions from the [!UICONTROL Templates] page in the [!DNL Adobe Workfront Fusion Administration] area.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>Workfront Fusion for Work Automation </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront Fusion administrator for your organization.</p> </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## View [!DNL Workfront Fusion] templates as an administrator

To view a table of all created templates and their statuses:

1. Click **[!UICONTROL Administration]** in the left navigation panel to open the [!UICONTROL Administration] area.
1. Click **[!UICONTROL Templates]** in the left navigation panel.

There are three columns related to the templates publication status. A checkmark in a column indicates the following:

* **Published**: These templates are currently visible in the [!UICONTROL Team templates] tab in the user interface.
* **Requested approval**: These templates are waiting for your approval. They are currently visible in the [!UICONTROL Team templates] tab in the user interface.
* **[!UICONTROL Approved]**: These templates have been approved. They are currently visible in the [!UICONTROL Public templates] tab in the standard user interface.

>[!NOTE]
>
>Templates with the checkmark in both the [!UICONTROL Requested approval] column and in the [!UICONTROL Approved] column have been already approved and made public, but there is a newer version of them waiting for your approval.

## Edit [!DNL Workfront Fusion] templates as an administrator

1. Click **[!UICONTROL Administration]** in the left navigation panel to open the [!UICONTROL Administration] area.
1. Click **[!UICONTROL Templates]** in the left navigation panel.
1. Click **[!UICONTROL Detail]** to the right of the template you want to edit.

You can now edit the template, similar to editing a template as a non-admin user. However, in the Options in the top-right corner, there is one additional option - the SVG diagram that provides you with the SVG code. Also, the publishing process is the same as in the case of a standard user, refer to the [!UICONTROL Publishing and sharing templates] section for more details.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To view the SVG code of the template, click Options in the upper-right corner and select SVG.</p>
-->

For information about specific template options that you can edit, see [Create new templates in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

For information about publishing templates, see [Publish and share Adobe Workfront Fusion templates](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approve or disapprove [!DNL Workfront Fusion] templates

Approving a template makes it visible in the [!UICONTROL Public templates] tab and available to all users. Disapproving a template removes it from the [!UICONTROL Public templates] tab and makes it available only to the team that created it.

1. Click **[!UICONTROL Administration]** in the left navigation panel to open the [!UICONTROL Administration] area.
1. Click **[!UICONTROL Templates]** in the left navigation panel.
1. If you want to approve a template, click **[!UICONTROL Approve]** to the right of the template.
1. If you want to disapprove a template, click **[!UICONTROL Disapprove]** to the right of the template.

>[!NOTE]
>
>If you are approving the template that was previously approved and then edited, your second approval will overwrite the original template.

## Clone a scenario as a template

As an administrator, you have the ability to clone a scenario as a template.

For instructions on cloning a scenario as a template, see [Create new templates in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create)in [Create new templates in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
