---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Send a Document with the enhanced connector
description: You can send documents from Workfront to Experience Manager Assets. Documents uploaded and sent from Workfront to Experience Manager Assets still count against your overall document storage. Assets linked from Experience Manager Assets don't count towards overall storage.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
---
# Send a Document with the enhanced connector

You can send documents from Workfront to Experience Manager Assets. Documents uploaded and sent from Workfront to Experience Manager Assets still count against your overall document storage. Assets linked from Experience Manager Assets don't count towards overall storage.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
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
   <td> <p>View access or higher on Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must

* Install the Workfront for Experience Manager enhanced connector.

## Send a Document to Experience Manager Assets

When a user sends a document from Workfront to Experience Manager Assets, mapped metadata transfers along the document. If configured, the metadata syncs continuously each time a change is made.

To send a document:

1. Go to the **Documents** area in Workfront, and select the document you want to send.
1. Click **Send to**, then choose the Experience Manager Assets integration your administrator set up.

   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention Experience Manager Assets.

   ![Send to](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Choose where you want the asset to go, then click **Select Folder**.
1. When you find your desired destination, click **Save**.

## Send a new version to Experience Manager Assets

You can add a new version to a document you have previously uploaded to Workfront. For more information, see [Upload a new version of a document](../../../documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to Experience Manager Assets. If a mapped field in Workfront has changed, the new version updates the metadata in Experience Manager Assets when it sends.

To send the most recent version:

1. Go to the **Documents** area in Workfront, and locate the document.
1. Click **Send to**, then choose the Experience Manager Assets integration your administrator set up.

   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention Experience Manager Assets.

   ![Send to](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Click **Save**. The new version saves in the same location as the previous version.
