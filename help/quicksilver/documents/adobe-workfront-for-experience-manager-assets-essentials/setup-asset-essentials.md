---
filename: setup-asset-essentials
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configure the Experience Manager Assets Essentials integration
description: Connect your work with your content in Experience Manager Assets Essentials - EDIT ME.
---

# Configure the Experience Manager Assets Essentials integration

Connect your work with your content in Experience Manager Assets Essentials​:

* Push assets and metadata from Adobe Workfront to Experience Manager Assets Essentials​
* Link assets from Experience Manager Assets Essentials to your projects and tasks in Workfront​
* Facilitate versioning workflows for assets pushed to Experience Manager Assets Essentials

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have Experience Manager Assets Essentials.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Set up the integration

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).
1. Select ![](assets/document-icon.png) **Documents** in the left panel, then select **Experience Manager Integration**.
1. Select **Add Experience Manager Integration**.
1. Specify the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Enter the name you want users to see in the Add new button in the Documents area.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Navigation&nbsp;URL</td> 
      <td>The system automatically populates the Navigation URL. This URL is used to link to your organization's Assets Essentials instance from the Main Menu for quick access.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Experience Manager Assets repository</p> </td> 
      <td> <p>The system automatically populates the Experience Manager repository associated with your Organization ID. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Set up metadata mapping:

   Documents with the native or custom fields automatically map to the specified fields the first time an asset is sent to Experience Manager Assets Essentials:

   1. In the **Workfront Source Field** column, choose a native or custom Workfront field.
   1. In the **Experience Manager Target Field**, choose an Experience Manager Assets Essentials field. 
   1. Repeat steps a. and b. as needed.

      >[!NOTE]
      >
      >You can map metadata only in one direction: from Workfront to Assets Essentials. Metadata for documents linked to Workfront from Assets Essentials cannot be transferred to Workfront.

1. Select **Save**.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Adobe Experience Manager Assets as a Cloud Service </h2>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Set up asset metadata </h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Map Workfront object data to asset media fields in Experience Manager Assets. Metadata maps when an asset is pushed from Workfront fo the first time.</p>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Set up folder metadata - CS only</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">When you create a linked folder, the associated project, portfolio, and program data is mapped to folder metadata fields in Experience Manager Assets.</p>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Enable Project metadata sync - CS only</h2>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Enable linked folders - Cs only?</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

