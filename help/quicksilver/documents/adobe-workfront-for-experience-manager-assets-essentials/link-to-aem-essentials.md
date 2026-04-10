---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Link assets and folders from Experience Manager Assets Essentials
description: You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents. Assets sent from Assets Essentials don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 
---
# Link assets and folders from Experience Manager Assets Essentials

You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents.

To link assets and folders from Experience Manager Assets using Content Advisor, see [Link assets and folders with Content Advisor powered by Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).


## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses</td> 
   <td> 
   <p>Contributor or higher</p> 
   <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Additional products</td> 
   <td>You must have Experience Manager as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager Permissions</td> 
    <td>You must have write access to the folder.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you begin:

* Your Workfront Administrator must configure an Experience Manager integration. For more information, see [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Link an asset from Experience Manager Assets Essentials

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Experience Manager Assets Essentials.

1. Select the assets you want.

   ![Select an asset](assets/select-an-asset.png)

1. Click **Select**.

## Link a new version from Experience Manager Assets Essentials

You can pull a new asset over from Experience Manager Assets Essentials and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets Essentials, the new version appears automatically in Workfront.

To link a new version:

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets Essentials.

1. Select the asset you want to link.

1. Click **Select**.

## Link a folder from Experience Manager Assets Essentials

Permissions to view individual assets inside of a folder rely on Experience Manager Assets Essentials permissions.

1. Go to the **Documents** area in Workfront where you want the folder.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets Essentials.

1. Select the folders you want.

   ![Select a folder](assets/select-a-folder.png)

1. Click **Select**.

## Considerations

* Content Advisor functionality is not available for Assets Essentials. To link assets and folders using Content Advisor, see [Link assets and folders with Content Advisor powered by Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* Assets sent from Assets Essentials don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.

* Metadata fields are first mapped when you send an asset from Workfront to Experience Manager Assets Essentials. If your Workfront administrator has enabled object metadata sync, fields remain up to date if they are changed in either application.
