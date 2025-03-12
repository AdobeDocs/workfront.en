---
title: Link assets and folders with the enhanced connector
description: You can link an asset or folder from Experience Manager Assets to any Workfront object that supports documents.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
---

# Link assets and folders with the enhanced connector

You can link an asset or folder from Experience Manager Assets to any Workfront object that supports documents. Assets sent from Experience Manager Assets don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Experience Manager Assets do count towards overall storage.


>[!NOTE]
>
>Excel files linked through the enhanced connector cannot be previewed in Workfront. You must download the file in order to access it.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current: Request or higher</p> 
   or
   <p>New: Contributor or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher on a Document</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.
+++

## Prerequisites

Before you begin, you must

* Install the Workfront for Experience Manager enhanced connector

## Link an asset from Experience Manager Assets

You can link an asset from Experience Manager Assets to Workfront. Once the asset is linked you can

* [Proof a linked asset for Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md) 
* [Upload a new version of a document](../../../documents/managing-documents/upload-new-document-version.md)

To link an asset to Experience Manager Assets:

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Click **Add new**, then choose the Experience Manager Assets integration your administrator set up.

   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention Experience Manager Assets.

1. Select the assets you want.

   ![Select an asset](assets/select-an-asset.png)

1. Click **Link**.

## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder to Experience Manager Assets:

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Click **Add new**, then choose the Experience Manager Assets integration your administrator set up.

   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention Experience Manager Assets.

1. Select the folders you want.

   ![Select a folder](assets/select-a-folder.png)

1. Click **Link**.

## Link a new version from Experience Manager Assets

You can pull a new asset over from Experience Manager Assets and add it to an existing asset as a new version in Workfront. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

>[!TIP]
>
>You can view all versions of an asset if you go to **Document Details** > **Versions**.

To link a new version from Experience Manager Assets:

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder. 
1. Click **Add new**, then choose the Experience Manager Assets integration your administrator set up.

   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention Experience Manager Assets.

1. Select the asset you want.

   ![Select an asset](assets/select-an-asset.png)

1. Click **Link**.
