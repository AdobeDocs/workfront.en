---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Link assets and folders with Content Advisor powered by Experience Manager Assets
description: You can link an asset or folder from Experience Manager Assets or Assets Essentials to any Adobe Workfront object that supports documents. Assets sent from Assets Essentials don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
---
# Link assets and folders with Experience Manager Assets' Content Advisor

Content Advisor brings intelligent, context-aware discovery directly into Workfront, helping you quickly find relevant, approved content based on context. With features such as smart suggestions, Dynamic Media renditions, and detailed asset metadata, it enables you to efficiently evaluate and reuse content without leaving Workfront, accelerating content creation while maintaining brand consistency.

You can use Content Advisor to link assets and folders from Experience Manager Assets or Assets Essentials to Workfront. Once linked, you can view and manage the asset in Workfront, and any changes made to the asset in Experience Manager Assets or Assets Essentials will be reflected in Workfront.


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

* Your Workfront Administrator must configure an Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) or [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

* To use Smart suggestions or Campaign Briefs, you must sign a GenAI Rider. For more information, see [Use Content Advisor to access AEM content in Adobe applications](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).



## Link an asset from Experience Manager Assets with Content Advisor

You can now use Content Advisor to link assets from Experience Manager Assets directly within Workfront. Content Advisor is not available for Assets Essentials.

>[!IMPORTANT]
>
>If your organization declines to sign the GenAI Rider agreement, you still use Content Advisor to choose assets and folders in Experience Manager Assets, but you will not have access to AI-powered features such as AI Search, smart suggestions, or analyzing campaign briefs.



To link an asset:

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Experience Manager Assets.

1. With Content Advisor, you can:


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Search for assets using AI Search.</strong> Use AI-powered search that understands meaning and intent behind queries, supporting multiple languages, typos, and synonyms.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">AI Search for smarter asset discovery</a>.</td>
      </tr>
      <tr>
         <td><strong>View smart suggestions based on context and intent.</strong> Discover assets that align with your content needs using context-aware recommendations from the host Adobe application.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Smart suggestions based on context and intent</a>.</td>
      </tr>
      <tr>
         <td><strong>Upload a campaign brief to discover relevant assets.</strong> Upload a PDF, DOCX, or TXT campaign brief document so Content Advisor can analyze it and recommend relevant assets.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Campaign briefs to discover relevant assets</a>.</td>
      </tr>
      <tr>
         <td><strong>View and select Dynamic Media asset renditions.</strong> Browse channel-optimized renditions including image presets, Smart Crops, and format types, and apply Dynamic Media modifiers to preview adjustments in real time.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Dynamic Media asset renditions available for use</a>.</td>
      </tr>
      <tr>
         <td><strong>Apply Dynamic Media modifiers to renditions.</strong> Add modifiers to transform asset renditions in real time and preview the results before selecting a rendition for your host application.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Dynamic Media asset renditions available for use</a>.</td>
      </tr>
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      <tr>
         <td><strong>Access asset metadata.</strong> Review asset properties such as title, description, format, size, and other metadata tabs (Product, Campaign, Tags) consistent with the Assets view.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Access asset metadata consistent with Assets view</a>.</td>
      </tr>
      <tr>
         <td><strong>Filter assets using predefined filters.</strong> Refine asset results using filters such as File Type, File Format, Asset Status, File Size, Image Width, Image Height, Modified Date, and Created Date.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Access filters consistent with Assets view</a>.</td>
      </tr>
      <tr>
         <td><strong>Save and reuse searches.</strong> Create saved searches by specifying a search term and filter options, then reuse them across Experience Manager Assets and other Adobe applications.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Access and reuse recent and saved searches</a>.</td>
      </tr>
      <tr>
         <td><strong>Search for assets across and within collections.</strong> Search for assets or collections across all collections, or limit your search to a specific collection.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Search for assets across and within collections</a>.</td>
      </tr>
   </tbody>
   </table>


### Link a new version from Experience Manager Assets with Content Advisor

You can pull a new asset over from Experience Manager Assets or Assets Essentials and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets or Assets Essentials, the new version appears automatically in Workfront.

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder. 
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link:

   * Select the Assets tab to browse assets, folders, or collections in Experience Manager Assets or Assets Essentials.

      ![Content advisor](assets/content-advisor-full.png)

   * Content fragments do not support versions. If you select a content fragment, the new version will replace the existing content fragment instead of creating a new version.

1. Click **Select**.

## Link an asset from Experience Manager Assets Essentials

Experience Manager Assets Essentials allows you to link assets directly to Workfront. Content Advisor is not available for Assets Essentials.

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Assets or Assets Essentials.

1. Select the assets you want.

   ![Select an asset](assets/select-an-asset.png)

1. Click **Select**.

## Link a folder from Experience Manager Assets or Assets Essentials

Permissions to view individual assets inside of a folder rely on Experience Manager Assets or Assets Essentials permissions.

1. Go to the **Documents** area in Workfront where you want the folder.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Assets or Assets Essentials.

1. Select the folders you want.

   ![Select a folder](assets/select-a-folder.png)

1. Click **Select**.

## Link a folder from Experience Manager Assets or Assets Essentials

Permissions to view individual assets inside of a folder rely on Experience Manager Assets or Assets Essentials permissions.

1. Go to the **Documents** area in Workfront where you want the folder.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Assets or Assets Essentials.

1. Click Assets > Files & Folders. 

1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.

1. Select the folder you want to link. 

1. Click **Select**.


## Considerations

* Content Advisor functionality is not available for objects using Adobe Enterprise Storage. If your organization uses Adobe Enterprise Storage, you can still link assets and folders from Experience Manager Assets or Assets Essentials, but you won't have access to Content Advisor features such as AI Search, smart suggestions, or Dynamic Media renditions. For more information, see [Use the Adobe Experience Manager with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Content Advisor functionality is not available for Assets Essentials.

* Assets sent from Assets Essentials don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.

* Metadata fields are first mapped when you send an asset from Workfront to Experience Manager Assets or Assets Essentials. If your Workfront administrator has enabled object metadata sync, fields remain up to date if they are changed in either application.
