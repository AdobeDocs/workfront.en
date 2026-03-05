---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: The Documents area
description: In the Documents area, you can organize, manage, and view metadata for documents uploaded to Adobe Workfront. You can also see the proof decision.
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
---
# The Documents area

In the Documents area, you can organize, manage, and view metadata for documents uploaded to Adobe Workfront. You can also see the proof decision.

Workfront currently has two versions of the Documents area: the legacy documents area and the new documents area. The version that your organization uses depends on whether your organization is on legacy Workfront storage or enterprise storage. For more information about these storage types, see [Enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Legacy documents area

There are two types of Documents areas. Features and functionality are the same for both:

* **Documents area in a program, portfolio, project, task, or issue:** Lists all documents that you have access to for a particular project, task, or issue. To access this area, click **Documents** ![Documents icon](assets/document-icon-12x14.png) in the left panel while viewing a project, task, or issue.

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

On a project, task, or issue where documents are uploaded, you can set up folders to organize the documents. For more information, see [Create document folders](../../documents/organizing-documents/create-documents-folder.md).

In the global Documents area, you can set up two types of folders to organize the documents you have access to:

* **Smart Folders:** Show only the documents that you want to see. For more information, see [Create and Manage Smart Folders](../../documents/organizing-documents/create-manage-smart-folders.md).

* **My Folders:**&nbsp;Organize documents the way you want them. For more information, see [Create document folders](../../documents/organizing-documents/create-documents-folder.md).

### Expanded Document Details

The Document Details page provides a more full-scale version of the Document Details in the Summary on the right.

## New document area

>[!NOTE]
>
>The global documents area is not available in the new documents area experience. You can only access documents from a programs, portfolios, projects, tasks, or issues.

### Use the summary panel

When you select a document in the documents area, you can use the Summary panel on the right to view details about the document, add and edit attached custom forms, create and manage approval workflows, view versions of the document, and more. 

#### Review and approve with Frame.io

You can review and approve documents in the new documents area using the Frame.io viewer.

For more information, see [Get started with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Manage versions

You can upload new versions of a document in the new documents area. When you upload a new version, the previous version is retained and can be accessed from the Summary panel. Versions are automatically named with the date and time of the upload, but can be renamed as needed. 

You can also kick off a new approval workflow for a specific version of a document.

#### View document history

You can view a document's history in the new documents area. The history includes the following types of information:

* When the document was uploaded
* When new versions were uploaded
* When approval workflows were kicked off for the document
* And more

### System-level folders for document permissions

Workfront automatically creates a system-level folder when the first document is uploaded to a task or issue. These folders inherit permissions from the task or issue and are visible in the project-level documents area. All documents uploaded to that task or issue are stored in that folder and inherit permissions from it. This is the primary way that permissions are managed for documents in the new documents area. For more information, see [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#folders).