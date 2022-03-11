---
filename: check-out-documents
product-area: documents
navigation-topic: manage-documents
title: Check out documents
description: You can check out a document to prevent other users from deleting it or uploading a new version of it. Only one user can check out a document at a time. You can check out any document uploaded to Adobe Workfront as well as documents linked to third-party document providers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint, or any other custom provider).
---

# Check out documents

You can check out a document to prevent other users from deleting it or uploading a new version of it. Only one user can check out a document at a time. You can check out any document uploaded to `Adobe Workfront` as well as documents linked to third-party document providers (Box, Dropbox, Google Drive, Webdam, `Workfront DAM`, SharePoint, or any other custom provider).&nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Review</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the Document</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Actions allowed on&nbsp;checked out documents

Users with manage access to the document&nbsp;can do the following:

<ul> 
 <li>Edit&nbsp;the document (document name, description, custom data)</li> 
 <li>Move the document</li> 
 <li>Share the document</li> 
 <li>Preview the document</li> 
 <li>Download the document<br><note type="tip">
   &nbsp;Although a user can download a document when it is checked out by another user, we&nbsp;recommend that users wait until the document has been checked back in before downloading it. When a document is checked out, it often indicates that work is still being done on the document. Waiting until a document is checked back in to download it ensures the user has the most recent version.
  </note></li> 
 <li>Approve a document or apply an approval to the document.</li> 
 <li> <p>Review the document in the <span>proofing viewer</span></p> <p>For more information about <span>proofing</span>, see <a href="../../review-and-approve-work/proofing/proofing.md" class="MCXref xref">Proofing</a></p> </li> 
</ul>

## Check a document out

If you have manage permissions to a document, you can check it out to forbid&nbsp;certain actions on the document.&nbsp;

<ol> 
 <li value="1"> <p>Go to the area where your document is stored, then select the document.&nbsp;</p> <p>For information about adding documents, see <a href="../../documents/adding-documents-to-workfront/add-documents-from-file-system.md" class="MCXref xref">Add documents to Adobe Workfront from your file system</a>.</p> </li> 
 <li value="2"> <p> Click the Check Out icon. <br><![CDATA[               ]]></p> </li> 
 <li value="3"> <p>A lock icon <img src="assets/lock-icon-locked-qs.png"> displays to the right of the document name. The document stays checked out after you log out of <span>Workfront</span>.</p> </li> 
 <p>Only the user who checked out&nbsp;the document or the <span>Workfront administrator</span> can check&nbsp;the document in.</p> 
</ol>

## Manage checked out documents

Consider the following about checked out documents:

* Before you can delete an object where a checked out document is stored, you must first check the document back in.&nbsp;
* If the `Workfront administrator` deletes a user who checked out a document they didn't own, `Workfront` automatically checks in the document.

* If the `Workfront administrator` deletes a user who checked out a document they own, and the document is uploaded on an object, the document remains checked out. Only a `Workfront administrator` can check it back in.

* If the `Workfront administrator` deletes a user who checked out a document they own, and the document is uploaded only in the Documents area (not on an object), the document is deleted with the user.

  For information about deleting users, see [Delete users](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* If the `Workfront administrator` deactivates a user, any documents they have checked out remain checked out. Only a `Workfront administrator` can check them back in.&nbsp;

## Check a document in

You must check a document back in before you can upload a new version or delete it.&nbsp;

To check in a document:

<ol> 
 <li value="1"> <p>Go to the area where your document is stored and select the document.&nbsp;</p> <p>A lock icon <img src="assets/lock-icon-locked-qs.png"> displays to the right of the document name.</p> </li> 
 <li value="2"> <p> Click the Check In icon . <br> </p> </li> 
</ol>

