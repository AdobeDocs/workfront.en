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

## Request an approval on a document

You can add a document approval in Workfront to any document you uploaded from Photoshop, Illustrator, or InDesign, or from Adobe Cloud Drive, the same as any other document. For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--
need to verify
Creating an approval on a Creative Cloud document also creates a new version of the document. For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md#view-the-current-file-during-an-approval).
-->