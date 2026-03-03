---
title: Share a document on enterprise storage
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Your Adobe Workfront administrator grants users access to view or edit documents when they assign access levels, as explained in Grant access to documents.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
---
# Share a document on enterprise storage

Users can upload documents to a project, task or issue. All documents are stored at the project level, but can be interacted with via linked objects on folders at the project level. 

Documents remain in their original project-level folders, preserving the existing folder structure and maintaining compatibility with Frame.io and ESM. 

Users can link or reassign documents and folders.  Linked objects are visible in both grid and list views, and clear indicators show which assets belong to which tasks or issues.

Inheritance rules apply automatically: subtasks inherit associations from their parent tasks, and subfolders inherit associations from their parent folders. Inherited associations cannot be overridden unless the asset is moved to a different parent.


Task/issue permissions inherited from project? And those are automatically applied to documents linked to the task?




## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> 
   <p>Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View access or higher to the objects you want to share</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Share documents in the legacy documents area

If your organization is on legacy Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about legacy Workfront storage, see [Differences between legacy Workfront storage and Adobe enterprise storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Share an individual document 

### Share documents in bulk 

### add a linked object - more of a move?

### Document permissions 

Permissions are specific to one item in Workfront and define what actions one can take on that item. For information about object permissions, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

+++ Expand to view a detailed list of document permissions

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

+++

## Share documents in the new documents area

If your organization uses enterprise storage, you will see the new documents area when you access documents in Workfront. For more information about enterprise storage, see [Enterprise Storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

Workfront is transitioning to the Adobe enterprise storage solution in order to provide greater connectivity with Adobe Creative Cloud products. Existing customers will be moved to the new model in phases. For more information about the benefits of Adobe enterprise storage, visit [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

If your Workfront instance uses Adobe enterprise storage, you cannot share individual documents directly. Instead, you must grant access at the project level.

>[!IMPORTANT]
>
>Sharing a project may also give users access to sensitive project information, such as financials, depending on the permission level you choose.
>
>Be sure to review permission settings carefully before sharing.



## Considerations about sharing documents


ESM documents can be shared by sharing the project, program, portfolio, or template that the document is associated with. Document permissions are determined by project-level permissions in ESM environments, rather than Workfront access levels alone, so some project and doument information may be available in other Adobe projects. For more information about access and permissions for ESM environments, see [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).




>[!NOTE]
>
>A Workfront administrator can add or remove permissions to any items in the system, for all users, without being the owner of those items.

* Sharing a document on ESM is different than sharing a legacy wf doc. Users only get manage access to a document and that happens by sharing task/issue

Individual documents cannot be shared

Can share a link?


* You can also share a document publicly or system-wide ? cant


* You can share a document with someone who does not have a Workfront account, by adding their email address in the Give document access to field. - can't ?



* When you share a document, users have the same access to all the document versions?

* You can inherit permissions to documents from the objects they are associated with. Your Workfront administrator can restrict the inheritance of permissions for documents in your access level. - no?



* An attached document inherits permissions only from the object where it was attached. If you create a folder on the object and move the document into the folder, it inherits the folder's permissions. But, if you create a folder on a parent or grandparent object and move the document into that folder, it does not inherit that folder's permissions. - not applicable ?





  For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  You can manually remove inherited permissions on documents. For more information, see [Remove permissions from objects](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)