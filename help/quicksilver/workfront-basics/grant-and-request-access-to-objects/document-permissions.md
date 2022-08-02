---
title: Share a document
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Your Adobe Workfront administrator grants users access to view or edit documents when they assign access levels, as explained in Grant access to documents.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
---
# Share a document

Your Adobe Workfront administrator grants users access to view or edit documents when they assign access levels, as explained in [Grant access to documents](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

The access level that the Workfront administrator grants to users allows them to either view or edit documents. In addition to this, other users can also grant others permissions to view or manage specific documents that they uploaded themselves or that they have access to share.

Permissions are specific to one item in Workfront and define what actions one can take on that item. For information about object permissions, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

The user who uploads a document to Workfront has Manage permissions to it, by default.

For information about sharing an entire document folder, see [Share a document folder](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Considerations about sharing documents

In addition to the considerations below, also see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>A Workfront administrator can add or remove permissions to any items in the system, for all users, without being the owner of those items.

* Sharing a document is similar to sharing any other object in Workfront. For information about how to share documents in Workfront, see [Share an object](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* You can grant the following permissions to documents:

   * View
   * Manage

* You can also share a document publicly or system-wide.

  >[!CAUTION]
  >
  >We recommend that you use caution when sharing an object containing confidential information with external users. This allows them to view information without being a Workfront user or part of your organization.

* You can share a document with someone who does not have a Workfront account, by adding their email address in the Give document access to field.
* When you share a document, users have the same access to all the document versions and all the document proofs.  
  For more information about proofing in Workfront, see the [Proofing](../../review-and-approve-work/proofing/proofing.md) section.

* You can inherit permissions to documents from the objects they are associated with. Your Workfront administrator can restrict the inheritance of permissions for documents in your access level.

  For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  You can manually remove inherited permissions on documents. For more information, see [Remove permissions from objects](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* An attached document inherits permissions only from the object where it was attached. If you create a folder on the object and move the document into the folder, it inherits the folder's permissions. But, if you create a folder on a parent or grandparent object and move the document into that folder, it does not inherit that folder's permissions.

## Document permissions

The following table displays what permissions you can grant users when allowing them to view or manage documents:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Action</strong> </p> </th> 
   <th> <p><strong>Manage</strong> </p> </th> 
   <th> <p><strong>View</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Create</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Edit Document Details</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delete*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Download</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Checkout</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Add Approvers</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Approve Document</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Attach Custom Form</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Edit Custom Fields</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Move to (object)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Send To (integration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Updates/ Comments</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Upload new version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delete Version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">View Document(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Preview</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Proof**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Generate Proof**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Remove Proof**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Share*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Share System-wide*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Share Documents Publicly*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Share with an external email address</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Add/ Remove</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Rename</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Link (with integration)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Unlink (with integration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Action is shared by both Documents and Document Folders.

&#42;&#42; You must have a separate proofing license associated with your Workfront account to be able to proof documents. Contact your account manager about acquiring a proofing license. For more information about proofing in Workfront, see [Proofing](../../review-and-approve-work/proofing/proofing.md).
