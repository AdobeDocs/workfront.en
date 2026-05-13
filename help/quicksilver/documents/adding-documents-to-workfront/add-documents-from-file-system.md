---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Add documents to Adobe Workfront from your file system
description: You can add documents to projects, tasks, or issues in multiple areas in Adobe Workfront.
author: Courtney, Alina
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/uM4y--i0xyZtRuB-PCZQLnLb8mNwc6YOW6jk4o6LAw0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Add documents to Adobe Workfront from your file system

Adobe Workfront currently has the following two types of document storages: 

   * Legacy Workfront storage 
   * Adobe enterprise storage

For more information about these storage types, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Some customers have both types of document storage and some have only Workfront or Adobe storage.

Adding documents to Workfront differs depending on which version of the documents area your organization uses. 

* [Add documents from your file system in the legacy Documents area](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Add documents to Workfront in the new Documents area](#add-documents-to-workfront-in-the-new-documents-area)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any Workfront package to manage documents using legacy Workfront storage</p>
<p>Any Workflow package to manage documents using Adobe enterprise storage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses</td> 
   <td> 
   <p>Contributor or higher</p> 
   <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Legacy Workfront Storage: Edit access to Documents</p> 
   <p>Enterprise storage: Edit access to Documents is enabled by default and cannot be changed</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Add documents from your file system in the legacy Documents area

If your organization is using legacy Workfront storage, you will see the legacy Documents area when you access documents in Workfront. 

For more information about Workfront storage, see [Differences between Adobe enterprise storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

You can add documents to the following areas in Workfront:

* The Documents area in the Main Menu
* The Documents area of a Workfront object (project, task, issue, template, template task, portfolio, program)
* A connected card on a Workfront board

You can also upload new versions of documents and add links to documents from third-party cloud vendors, such as Google Drive, Dropbox, and Microsoft OneDrive. 

For information about adding new versions of documents, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md). 

For information about adding documents from third-party cloud vendors, see [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

There are no restrictions on the types and sizes of files that you can upload to Workfront. However, in order to be successful, the upload must be completed within five minutes and you must have adequate storage space available.

If you need information about uploading new versions of a document to Workfront, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).


### Add documents to Workfront in the legacy Documents area 

You can add new documents to Workfront from the file system on your workstation. You can also link documents from third-party applications such as Google Drive and SharePoint.

>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.

To add a document:

1. Go to the Workfront object where you want to add a new document.
1. Click the **Documents** tab, then click the **Add new** drop-down menu.

   ![Add new document](assets/add-new-doc.png)

1. Depending on the type of document you want to add, do any of the following: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Upload documents from your file system on your workstation</td> 
      <td> 
       <ol> 
        <li value="1">From the <strong>Add new</strong> drop-down menu, select <strong>Document.</strong></li> 
        <li value="2"> <p>Browse to and select the document that you want to add from the file system on your workstation.<br></p> <p>You can select multiple documents by pressing the Shift key as you select additional files.</p> </li> 
        <li value="3">Click <strong>Open</strong>.</li> 
       </ol> 
       <p><b>NOTE</b>: You can also drag and drop files directly from your file manager into the document list.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Upload documents from a third-party application such as Google Drive or SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>From the <strong>Add new</strong> drop-down menu, select <strong>From &lt;name_of_third-party_application&gt;</strong>.</p> <p>For example, to upload a document from Google Drive, click <strong>From Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Follow the prompts to select the document in the third-party application.<br></p> <p>For more information about linked documents, see <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Link documents from external applications</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Request a document from another Workfront user</td> 
      <td> 
       <ol> 
        <li value="1">From the <strong>Add new</strong> drop-down menu, select <strong>Request a Document</strong>.</li> 
        <li value="2">In the <strong>Who are you requesting it from</strong> box, type the name of the user from whom you are requesting the document.</li> 
        <li value="3">In the <strong>Tell them what you're requesting</strong> box, type the name of the document.</li> 
        <li value="4"> <p>Click <strong>Send Request</strong>.</p> <p>Your request displays on your Documents tab.</p> <p>For more information about requesting documents, see <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Request a Document</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

   The document is added to the Documents section of the object you selected. 

## Add documents to Workfront in the new Documents area 

You can add documents to objects using the Adobe enterprise storage model. For more information about enterprise storage, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

Functionality not currently supported in the new Documents area:

* Uploading documents to the Documents area in the Main menu
* Adding links to documents from third-party cloud vendors, such as Google Drive, Dropbox, and Microsoft OneDrive.
* Requesting documents
* Copying a link to a folder
* Checking out documents
* Pasting images from the clipboard
* Adding Smart folders

### Add documents to Workfront in the new Documents area 

If your organization uses enterprise storage, you will see the new Documents area when you access documents in Workfront. For more information about enterprise storage, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To add a document:

1. Go to the Workfront object where you want to add a new document.
1. Click the **Documents** section in the left panel.
1. Click **New** on the right side of the page or drag and drop the file into the drop zone that appears. You can add multiple documents at one time.

   ![Add a new document](assets/add-new-doc-new-doc.png)

If you need information about uploading new versions of a document to Workfront, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).

   A folder with the same name as the object you are uploading the document to is automatically created in the Documents section and the document is added to the folder. 

## Document security for enterprise storage 

Workfront prevents viruses and other malicious content from entering the site via documents in the following ways:

**How Workfront detects corrupted files**

Document scanning is automatically enabled for objects using the Adobe enterprise storage model.

All files under 500 MB are scanned when they are uploaded. Files over 500 MB are not scanned. If Workfront detects a corrupted document, it is automatically removed.

**File name restrictions**

Because this integration is built using Adobe enterprise storage, there are some enforced structure and naming conventions to be aware of when managing projects and documents.

* Object names must be unique and can't be duplicated
* Adobe enterprise storage requires unique names for peer objects with the same parent in the hierarchy tree
* Documents can't have the same name if they belong to the same project
* Document names can't contain any of the following special characters: `\ / : * ? " | < >`
* Document names are limited to 255 characters maximum

With these limitations in mind, Workfront automatically renames objects or documents as needed to prevent conflicts.


## Document security for legacy Workfront storage

Workfront prevents viruses and other malicious content from entering the site via documents in the following ways:

**How Workfront detects corrupted files**

Document scanning is enabled for your organization only upon request.

If document scanning is enabled, files under 25 MB are scanned when they are uploaded. Files over 25 MB are not scanned.

If Workfront detects a corrupted document, a message appears indicating that the file is corrupt. You also receive an email notification when Workfront detects potentially malicious content and the file is slated for removal.

Corrupted files are removed within 24 hours of detection unless you remove them manually. If you delete a corrupted file, Workfront tracks this action as an update. If you allow Workfront to remove it, then no updates are recorded.

**File name restrictions**

Files that are uploaded to Workfront cannot contain certain characters in file names. If a file contains any of the following characters in the file name, the characters are removed from the file name when the file is uploaded: `! # % * \ | ' " / ? < > { } [ ]`.
