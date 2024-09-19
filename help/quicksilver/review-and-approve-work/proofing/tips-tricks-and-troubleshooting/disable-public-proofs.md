---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Disable sharing proof via public URL or embed code
description: You can turn off the ability to share a proof with a public URL or embed code on a proof by proof basis or for individual users.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
---
# Disable sharing proof via public URL or embed code

You can turn off the ability to share a proof with a public URL or embed code on a proof by proof basis or for individual users.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Disable per Proof

You must be the proof owner or creator, or you must have the Author or Moderator proof role.

1. In the project that contains the proof, click **Documents** in the left panel.
1. Hover over the proof and select **Document Details** .
1. In the left panel, click **Proofing Viewer Settings**, then disable the **Allow sharing proof via public URL or embed code** checkbox.

   ![](assets/proofing-viewer-settings-350x200.png)

1. Click **Save**.

## Disable per user

You can disable the Public proof setting for individual users in your Workfront instance. You must have a Proof Permission Profile of administrator to make this change.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Proofing**.
1. Click **Account Settings** near the top-right corner.
1. Click the **Users** tab, then click on the name of a user.
1. In the **Default proof settings** section, disable the **Public Sharing** checkbox.

   ![](assets/default-proof-settings--public-sharing-350x210.png)
