---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: The Documents area
description: In the Documents area, you can organize, manage, and view metadata for documents uploaded to Adobe Workfront. You can also see the proof decision.
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/IdrQfkprrzF-Jt-ZwlnVfvIO07B2ejvbOLhbAhPh8Lc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
---
# The Documents area

In the Documents area, you can organize, manage, and view metadata for documents uploaded to Adobe Workfront. You can also see the proof decision.

Workfront currently has two versions of the Documents area: the legacy documents area and the new Documents area. The version that your organization uses depends on whether your organization is on legacy Workfront storage or Adobe cloud storage. For more information about these storage types, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Legacy documents area

There are two types of Documents areas. Features and functionality are the same for both:

* **Documents area in a program, portfolio, template, project, task, or issue:** Lists all documents that you have access to for a particular project, task, or issue. To access this area, click **Documents** ![Documents icon](assets/document-icon-12x14.png) in the left panel while viewing a project, task, or issue.

* **Global Documents area:** Lists all documents that you have access to&nbsp;in Workfront. To access this area, click **Documents** ![Documents icon](assets/document-icon.png) in the Main Menu ![Main Menu icon](assets/main-menu-icon.png).

For information about uploading documents to Workfront, see [Add documents to Adobe Workfront from your file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).


The documents area records a count of the following items:

* Workfront folders
* Files uploaded from the file system
* Files added to Workfront from integrations
* Linked Experience Manager Assets

### Summary panel

When you select a document in the documents area, you can use the Summary on the right to view document details, manage document updates and approvals, view versions of the document, and add and edit Custom Forms for the document.

If proofing is set up for the document, the Details section includes information such as the proofing due date and current proofing progress.

You can click the Details heading to go to the full Document Details area when you need all of the information about a document.

![Documents area](assets/documents-area-v2-350x199.png)

For information about the Summary, see [Summary for documents overview](../../documents/managing-documents/summary-for-documents.md).

### Proof decision

Once a proof decision is made, it appears in the Document list.

![Proof decision in document list](assets/proof-decision---doc-list-350x168.png)

### Folders

You can set up folders to organize documents. For more information, see [Create document folders](../../documents/organizing-documents/create-documents-folder.md).

In the global Documents area, you can set up two types of folders to organize the documents you have access to:

* **Smart Folders:** Show only the documents that you want to see. For more information, see [Create and Manage Smart Folders](../../documents/organizing-documents/create-manage-smart-folders.md).

* **My Folders:**&nbsp;Organize documents the way you want them. For more information, see [Create document folders](../../documents/organizing-documents/create-documents-folder.md).

### Expanded Document Details

The Document Details page provides a more full-scale version of the Document Details in the Summary on the right.

## New Documents area

The new Documents area is only available for if your organization is on Adobe cloud storage. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Use the summary panel

When you select a document in the documents area, you can use the Summary panel on the right to view details about the document, add and edit attached custom forms, create and manage approval workflows, view versions of the document, and more. 

#### Review and approve with Frame.io

You can review and approve documents in the new Documents area using the Frame.io viewer.

For more information, see [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Manage versions

You can upload new versions of a document in the new Documents area. When you upload a new version, the previous version is retained and can be accessed from the Summary panel. Versions are automatically named with the date and time of the upload, but can be renamed as needed. 

You can also kick off a new approval workflow for a specific version of a document.

#### View document history

You can view a document's history in the new Documents area. The history includes the following types of information:

* When the document was uploaded
* When new versions were uploaded
* When approval workflows were kicked off for the document
* And more

### System-level folders for document permissions

Workfront automatically creates a system-level folder when the first document is uploaded to a task or issue. These folders inherit permissions from the task or issue and are visible in the project-level documents area. All documents uploaded to that task or issue are stored in that folder and inherit permissions from it. This is the primary way that permissions are managed for documents in the new Documents area. For more information, see [Object permissions and access level overview for the Adobe cloud storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Considerations

* The new Documents area is optimized for screens 1024 pixels wide or larger. If you have a smaller screen, you may may have issues accessing the Summary panel. 

* The global Documents area is not available in the new Documents area experience. You can only access documents from a programs, portfolios, projects, tasks, or issues.
