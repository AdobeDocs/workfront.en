---
filename: enhanced-connector-send-document
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Send a Document to Experience Manager Assets
description: You can send documents from Workfront to Experience Manager Assets. Documents uploaded and sent from Workfront to Experience Manager Assets still count against your overall document storage. Assets linked from Experience Manager Assets don't count towards overall storage.
---

# Send a Document to Experience Manager Assets

You can send documents from `Workfront` to `Experience Manager Assets`. Documents uploaded and sent from `Workfront` to Experience Manager Assets still count against your overall document storage. Assets linked from Experience Manager Assets don't count towards overall storage.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Request</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td><span>Experience Manager Assets</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher on Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

Before you begin, you must

* Install the `Workfront for Experience Manager enhanced connector`.

## Send a Document to Experience Manager Assets

When a user sends a document from `Workfront` to `Experience Manager Assets`, mapped metadata transfers along the document. If configured, the metadata syncs continuously each time a change is made. 

<!--
For information on metadata syncing, see
-->

To send a document:

<ol> 
 <li value="1"> <p>Go to the <span class="bold">Documents</span> area in <span>Workfront</span>, and select the document you want to send.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Send to</span>, then choose the Experience Manager Assets integration your administrator set up.</p> <note type="note">
   Any name may be chosen for this integration, so it may not specifically mention 
   <span>Experience Manager Assets</span>.
  </note> <p> <img src="assets/copy-of-send-to-in-toolbar-350x149.png" style="width: 350;height: 149;"> </p> </li> 
 <li value="3"> <p>Choose where you want the asset to go, then click <span class="bold">Select Folder</span>.</p> </li> 
 <li value="4"> <p>When you find your desired destination, click <span class="bold">Save</span>. </p> </li> 
</ol>

## Send a new version to `Experience Manager Assets`

You can add a new version to a document you have previously uploaded to `Workfront`. For more information, see [Upload a new version of a document](../../../documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to `Experience Manager Assets`. If a mapped field in `Workfront` has changed, the new version updates the metadata in `Experience Manager Assets` when it sends.

To send the most recent version:

<ol> 
 <li value="1">Go to the <span class="bold">Documents</span> area in <span>Workfront</span>, and locate the document.</li> 
 <li value="2"> <p>Click <span class="bold">Send to</span>, then choose the Experience Manager Assets integration your administrator set up.</p> <note type="note">
   Any name may be chosen for this integration, so it may not specifically mention 
   <span>Experience Manager Assets</span>.
  </note> <p> <img src="assets/copy-of-send-to-in-toolbar-350x149.png" style="width: 350;height: 149;"> </p> </li> 
 <li value="3"> <p>Click <span class="bold">Save</span>. The new version saves in the same location as the previous version. </p> </li> 
</ol>

