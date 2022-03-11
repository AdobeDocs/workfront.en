

# Link assets and folders from `Experience Manager Assets`

You can link an asset or folder from `Experience Manager Assets` to any Workfront object that supports documents. Assets sent from `Experience Manager Assets` don't count towards your overall document storage in `Workfront`. Documents uploaded and sent from `Workfront` to `Experience Manager Assets` do count towards overall storage.

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
   <td> <p>View access or higher on a Document</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

Before you begin, you must

* Install the `Workfront for Experience Manager enhanced connector`

## Link an asset from `Experience Manager Assets`

You can link an asset from `Experience Manager Assets` to `Workfront`. Once the asset is linked you can

* [Proof a linked asset for Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md) 
* [Upload a new version of a document](../../../documents/managing-documents/upload-new-document-version.md)

To link an asset to `Experience Manager Assets`:

<ol> 
 <li value="1">Go to the <span class="bold">Documents</span> area in <span>Workfront</span> where you want to add the document.</li> 
 <li value="2"> <p>Click <span class="bold">Add new</span>, then choose the Experience Manager Assets integration your administrator set up.</p> </li> 
 <li value="3"> <note type="note">
   Any name may be chosen for this integration, so it may not specifically mention 
   <span>Experience Manager Assets</span>.
  </note> </li> 
 <li value="4"> <p>Select the assets you want.</p> <p> <img src="assets/select-an-asset.png"> </p> </li> 
 <li value="5"> <p>Click <span class="bold">Link</span>.</p> </li> 
</ol>

## Link a folder from `Experience Manager Assets`

Permissions to view individual assets inside of a folder rely on `Experience Manager Assets` permissions.

To link a folder to `Experience Manager Assets`:

<ol> 
 <li value="1">Go to the <span class="bold">Documents</span> area in <span>Workfront</span> where you want to add the document.</li> 
 <li value="2"> <p>Click <span class="bold">Add new</span>, then choose the Experience Manager Assets integration your administrator set up.</p> </li> 
 <li value="3"> <note type="note">
   Any name may be chosen for this integration, so it may not specifically mention 
   <span>Experience Manager Assets</span>.
  </note> </li> 
 <li value="4"> <p>Select the folders you want.</p> <p> <img src="assets/select-a-folder.png"> </p> </li> 
 <li value="5"> <p>Click <span class="bold">Link</span>.</p> </li> 
</ol>

## Link a new version from `Experience Manager Assets`

You can pull a new asset over from `Experience Manager Assets` and add it to an existing asset as a new version in `Workfront`. If the document is already linked and a new version is added in `Experience Manager Assets`, the new version appears automatically in `Workfront`.

>[!TIP]
>
>You can view all versions of an asset if you go to `Document Details` > `Versions`.

To link a new version from `Experience Manager Assets`:

<ol> 
 <li value="1">Go to the <span class="bold">Documents</span> area in <span>Workfront</span> where you want to add the document.</li> 
 <li value="2"> <p>Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder. </p> </li> 
 <li value="3"> <p>Click <span class="bold">Add new</span>, then choose the Experience Manager Assets integration your administrator set up.</p> <note type="note">
   Any name may be chosen for this integration, so it may not specifically mention 
   <span>Experience Manager Assets</span>.
  </note> </li> 
 <li value="4"> <p>Select the asset you want.</p> <p> <img src="assets/select-an-asset.png"> </p> </li> 
 <li value="5"> <p>Click <span class="bold">Link</span>. </p> </li> 
</ol>

