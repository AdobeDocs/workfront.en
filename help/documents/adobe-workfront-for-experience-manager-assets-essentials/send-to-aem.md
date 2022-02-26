---
filename: send-to-aem
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Send a Document to Experience Manager Assets Essentials
description: You can send documents from Workfront to Experience Manager Assets Essentials. Documents uploaded and sent from Workfront to Assets Essentials still count against your overall document storage. Assets linked from Assets Essentials don't count towards overall storage.
---

# Send a Document to *Experience Manager Assets Essentials*

You can send documents from *Workfront* to *Experience Manager Assets Essentials*. Documents uploaded and sent from *Workfront* to *Assets Essentials* still count against your overall document storage. Assets linked from *Assets Essentials* don't count towards overall storage.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a>*</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p><em>Request</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have <em>Experience Manager Assets Essentials</em>.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Experience Manager User Permissions</td> 
    <td>Administrator</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Experience Manager User Permissions</td> 
   <td>Administrator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher on Documents</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Send a Document from *Workfront*

When a user sends a document from *Workfront* to *Assets Essentials*, mapped metadata transfers along the document. After the document is sent, changes made to the document's metadata in *Workfront* are not reflected in *Assets Essentials*. If a mapped field in *Workfront* is changed, you must send a new version of the document with the updated metadata to *Assets Essentials*. To set up or edit metadata, see [Configure the Experience Manager Assets Essentials integration](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

To send a document:

<ol> 
 <li value="1"> <p>Go to the <span class="bold">Documents</span> area in <em>Workfront</em>, and select the document you want to send.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Send to</span>, then choose the <em>Assets Essentials</em> integration your administrator set up.</p> <note type="note">
   The 
   <em>Workfront administrator</em> can choose any name for this integration, so it may not specifically mention 
   <em>Assets Essentials</em>.
  </note> <p> <img src="assets/copy-of-send-to-in-toolbar-350x149.png" style="width: 350;height: 149;"> </p> </li> 
 <li value="3"> <p>Choose where you want the asset to go, then click <span class="bold">Select Folder</span>.</p> </li> 
 <li value="4"> <p>When you find your desired destination, click <span class="bold">Save</span>. </p> </li> 
</ol>

## Send a new version

You can add a new version to a document you have previously uploaded to *Workfront*. For more information, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to *Assets Essentials*. If a mapped field in *Workfront* has changed, the new version updates the metadata in *Assets Essentials* when it sends.

>[!IMPORTANT]
>
>Before you upload a new version to Workfront, we recommend renaming the file. If you upload a new version with the exact same file name as a previous version, only the most recent version can be downloaded from Workfront. All versions can be downloaded from AEM Assets Essentials regardless of the file name.

To send the most recent version:

<ol> 
 <li value="1">Go to the <span class="bold">Documents</span> area in <em>Workfront</em>, and locate the document.</li> 
 <li value="2"> <p>Select <span class="bold">Send to</span>, then choose the <em>Assets Essentials</em> integration your administrator set up.</p> <note type="note">
   The 
   <em>Workfront administrator</em> can choose any name for this integration, so it might not specifically mention 
   <em>Assets Essentials</em>.
  </note> <p> <img src="assets/copy-of-send-to-in-toolbar-350x149.png" style="width: 350;height: 149;"> </p> </li> 
 <li value="3"> <p>Click <span class="bold">Save</span>. The new version saves in the same location as the previous version. </p> </li> 
</ol>

