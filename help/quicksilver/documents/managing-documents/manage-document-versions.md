---
filename: manage-document-versions
product-area: documents
navigation-topic: manage-documents
title: Manage document versions
description: You can manage multiple versions of a document in Workfront.
---

# Manage document versions

You can manage multiple versions of a document in Workfront.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to the Document</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

* This article assumes that the document has multiple versions.

  If you need information about uploading new versions of a document to Workfront, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).

## View a list of all versions of a document

View and manage details for a previous document version

1. Near the top of the Document Details page, click the drop-down menu next to the name, then click the name of the version you want to view and manage.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Along with viewing the version's Details, you can make changes to the version, such as its name, metadata, and proofing settings (if it's a document proof).

Download a single document version In the Summary, under Versions, click the click the More menu to the right of the version, then click Download in the drop-down list that appears. 

## Download all versions of a document

## Delete a document version

If you upload a version of a document by mistake, or a version is no longer needed, you can delete the version and maintain the original document.

>[!IMPORTANT]
>
>You can't recover a document version that you delete individually.

Keep the following in mind when you consider deleting a document version:

* Only one version can be deleted at a time. If a version is deleted, this action appears in the `Updates` on the document . 
* If you upload a new version after deleting a version, the new version receives the next sequential number. For example, if there are 3 versions of a document and you delete version 3, the next document uploaded will be version 4.
* System updates and comments made on a version are retained in Workfront after the version is deleted.

  <!--
  Deleting a document version in Workfront does not delete the Proof version.
  -->

To delete a document version:

1. Go to the project, task, or issue that contains the document, then select `Documents`.Find the document you need.
1. In the Version area in the Summary, click the version, then click `Delete` in the drop-down list that appears. The `Delete` option is visible only if there are at least two versions. 
   If the document is linked to an outside source, that link is deleted and the document is no longer accessible through Workfront.

