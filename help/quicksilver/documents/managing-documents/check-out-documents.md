---
product-area: documents
navigation-topic: manage-documents
title: Check out documents
description: You can check out a document to prevent other users from deleting it or uploading a new version of it. Only one user can check out a document at a time. You can check out any document uploaded to Adobe Workfront as well as documents linked to third-party document providers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint, or any other custom provider).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
---
# Check out documents

You can check out&nbsp;a document to prevent other users from deleting it or uploading a new version of it. Only one user can check out a document at a time.&nbsp;You can check out any document uploaded to Adobe Workfront as well as documents linked to third-party document providers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint, or any other custom provider).&nbsp;

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
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the Document</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Actions allowed on&nbsp;checked out documents

Users with manage access to the document&nbsp;can do the following:

* Edit&nbsp;the document (document name, description, custom data)
* Move the document
* Share the document
* Preview the document
* Download the document

  >[!TIP]
  >
  >&nbsp;Although a user can download a document when it is checked out by another user, we&nbsp;recommend that users wait until the document has been checked back in before downloading it. When a document is checked out, it often indicates that work is still being done on the document. Waiting until a document is checked back in to download it ensures the user has the most recent version.

* Approve a document or apply an approval to the document.
* Review the document in the proofing viewer

  For more information about proofing, see [Proofing](../../review-and-approve-work/proofing/proofing.md)

## Check a document out

If you have manage permissions to a document, you can check it out to forbid&nbsp;certain actions on the document.&nbsp;

1. Go to the area where your document is stored, then select the document.&nbsp;

   For information about adding documents, see [Add documents to Adobe Workfront from your file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Click the **Check Out** icon ![](assets/check-out-25x23.png).    
   
1. A lock icon ![](assets/lock-icon-locked-qs.png) displays to the right of the document name. The document stays checked out after you log out of Workfront.
1. Only the user who checked out&nbsp;the document or the Workfront administrator can check&nbsp;the document in.

## Manage checked out documents

Consider the following about checked out documents:

* Before you can delete an object where a checked out document is stored, you must first check the document back in.&nbsp;
* If the Workfront administrator deletes a user who checked out a document they didn't own, Workfront automatically checks in the document.
* If the Workfront administrator deletes a user who checked out a document they own, and the document is uploaded on an object, the document remains checked out. Only a Workfront administrator can check it back in.
* If the Workfront administrator deletes a user who checked out a document they own, and the document is uploaded only in the Documents area (not on an object), the document is deleted with the user.

  For information about deleting users, see [Delete users](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* If the Workfront administrator deactivates a user, any documents they have checked out remain checked out. Only a Workfront administrator can check them back in.&nbsp;

## Check a document in

You must check a document back in before you can upload a new version or delete it.&nbsp;

To check in a document:

1. Go to the area where your document is stored and select the document.&nbsp;

   A lock icon ![](assets/lock-icon-locked-qs.png) displays to the right of the document name.

1. Click the **Check In** icon ![](assets/check-in-25x22.png).
