---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: Use Workfront documents in Creative Cloud apps
description: Open, edit, and save Workfront documents from Photoshop, Illustrator, and InDesign, and request approvals on them.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Use Workfront documents in Creative Cloud apps

After a Workfront project is available in the Creative Cloud Projects panel, you can work with its documents directly from Photoshop, Illustrator, or InDesign.

## Prerequisites

* Your organization must be on a version of Workfront that supports Adobe cloud storage.
* Workfront and Photoshop, Illustrator, or InDesign must be entitled in the same Adobe Identity Management System (IMS) organization.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront version</td> 
   <td>Workflow Ultimate, with Adobe cloud storage enabled</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>
      <p>View access to a project to see it in the Creative Cloud projects panel</p>
      <p>Edit access to a project to add, edit, or delete it</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Access a Workfront project

The Documents folder structure in a Workfront project is mirrored in the Projects panel. When you open a document from a project folder, edit it, and save, your changes appear in Workfront.

>[!NOTE]
>
>Legacy Workfront storage projects are not supported in the Projects panel—-only Adobe cloud storage projects.


To access a Workfront project in Photoshop, Illustrator, or InDesign:

1. Open Photoshop, Illustrator, or InDesign.
1. In the **Projects** panel on the left side of the app, select the Workfront project you want to open.

   ![Workfront projects listed in the Projects panel](assets/cc-projects.png)

1. Open a document in the project to edit it. Once you save your changes, they are automatically saved back to the Workfront project.


>[!TIP]
>
>To edit a file type that Photoshop, Illustrator, or InDesign can't open, such as a Word or Excel document, use Adobe Cloud Drive instead. For more information, see [Adobe Cloud Drive overview](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md).

## Save a new document to Workfront from a Creative Cloud App

You can save a new file to Workfront or you can save a new copy of an existing file to Workfront from Photoshop, Illustrator, or InDesign. 

To save a new document to Workfront: 

1. Open Photoshop, Illustrator, or InDesign, and create a new file.
1. If you are saving a new file, click **Save** in the top menu.
Or
If you are saving a new copy of an existing file, click **Save As** in the top menu.
1. In the **Save As** dialog, select **Save to cloud documents**, then choose the Workfront project you need. 

    >[!NOTE]
    >
    >When saving a document already in the Workfront project, the Save As dialog doesn't open. You can select a Workfront project, save to a different folder or choose a different Workfront project.


     ![save new document in workfront](assets/save-new-to-wf.png)

1. Choose a document folder, then click **Save**. If you don't choose a folder, the document is saved to the project root folder.

    ![choose folder to save new document in workfront](assets/save-to-folder.png)

## Request an approval on a document

You can add a document approval in Workfront to any document you uploaded from Photoshop, Illustrator, or InDesign, or from Adobe Cloud Drive, the same as any other document. For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).



## Manage versions of a document in Workfront from a Creative Cloud app

When you save a document from Photoshop, Illustrator, or InDesign to Workfront, the changes you save appear in the Current file on the Versions tab and are marked with a "New changes" badge.

You can request an approval on the Current file rather than uploading a new versionof the document. For more information, see [Request an approval on the Current file](#request-approval-on-the-current-file).

![current file with new changes badge](assets/current-file.png)

### Request approval on the Current file

To request an approval on the Current file of a document in Workfront:

1. Go to the project in Workfront that contains the document you want to request an approval on.
1. Open the document and go to the **Versions** tab.
1. On the Current file, click **More** menu, then click **Request Approval**.
1. In the **Request Approval** dialog, follow the steps in [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) to create the approval.

   ![request approval on current file](assets/request-update-on-current-file.png)

