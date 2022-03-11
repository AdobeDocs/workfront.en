---
filename: link-to-aem
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Link assets and folders from Experience Manager Assets Essentials
description: You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents. Assets sent from Assets Essentials don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.
---

# Link assets and folders from `Experience Manager Assets Essentials`

You can link an asset or folder from `Experience Manager Assets Essentials` to any `Adobe Workfront` object that supports documents. Assets sent from `Assets Essentials` don't count towards your overall document storage in `Workfront`. Documents uploaded and sent from `Workfront` to `Assets Essentials` do count towards overall storage.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> licenses*</td> 
   <td> <p><span>Request</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have <span>Experience Manager Assets Essentials</span>.</td> 
  </tr> <!--
   AEM assets permisson
  --> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Link an asset from `Experience Manager Assets Essentials`

You can link an asset from `Experience Manager Assets Essentials` to `Workfront`. Once the asset is linked you can

* [Proof a linked asset for Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md) 
* [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md)

<ol> 
 <li value="1">Go to the <span class="bold">Documents</span> area in <span>Workfront</span> where you want to add the document.</li> 
 <li value="2"> <p>Select <span class="bold">Add New</span>, then select the <span>Assets Essentials</span> integration your administrator set up.</p> <note type="note">
   The 
   <span>Workfront administrator</span> can choose any name for this integration, so it may not specifically mention 
   <span>Assets Essentials</span>.
  </note> </li> 
 <li value="3"> <p>Select the assets you want.</p> <p> <img src="assets/select-an-asset.png"> </p> </li> 
 <li value="4"> <p>Click <span class="bold">Select</span>.</p> </li> 
</ol>

## Link a folder from `Experience Manager Assets Essentials`

Permissions to view individual assets inside of a folder rely on `Experience Manager Assets Essentials` permissions.

<ol> 
 <li value="1"> <p>Go to the <span class="bold">Documents</span> area in <span>Workfront</span> where you want the folder.</p> </li> 
 <li value="2"> <p>Select <span class="bold">Add New</span>, then select the <span>Assets Essentials</span> integration your administrator set up.</p> <note type="note">
   The 
   <span>Workfront administrator</span> can choose any name for this integration, so it might not specifically mention 
   <span>Assets Essentials</span>.
  </note> </li> 
 <li value="3"> <p>Select the folders you want.</p> <p> <img src="assets/select-a-folder.png"> </p> </li> 
 <li value="4"> <p>Click <span class="bold">Select</span>.</p> </li> 
</ol>

## Link a new version from `Experience Manager Assets Essentials`

You can pull a new asset over from `Assets Essentials` and add it to an existing asset as a new version. If the document is already linked and a new version is added in `Assets Essentials`, the new version appears automatically in `Workfront`.

To link a new version from `Assets Essentials`:

<ol> 
 <li value="1">Go to the <span class="bold">Documents</span> area in <span>Workfront</span> where you want to add the document.</li> 
 <li value="2"> <p>Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder. </p> </li> 
 <li value="3"> <p>Select <span class="bold">Add New</span> > <span class="bold">Version</span>, then select the <span>Assets Essentials</span> integration your administrator set up.</p> <note type="note">
   The 
   <span>Workfront administrator</span> can choose any name for this integration, so it might not specifically mention 
   <span>Assets Essentials</span>.
  </note> </li> 
 <li value="4"> <p>Select the asset you want.</p> <p> <img src="assets/select-an-asset.png"> </p> </li> 
 <li value="5"> <p>Click <span class="bold">Select</span>. </p> </li> 
</ol>

>[!TIP]
>
>You can view all versions of an asset if you go to `Document Details` > `Versions`.

