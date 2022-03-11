---
filename: generate-proof-for-a-document
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Create a proof for a document
description: You can generate a proof for a document at the time you are uploading it to Workfront.
---

# Create a proof for a document

You can generate a proof for a document at the time you are uploading it to Workfront.

You can also generate a proof for a document already uploaded in Adobe Workfront or for a new version of a proof already in Workfront.

If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Upload a document and create a proof

<ol> 
 <li value="1">Go to the project, task, or issue where you want to create a new proof.</li> 
 <li value="2">Click the <span class="bold">Documents</span>&nbsp;tab.</li> 
 <li value="3">Click Documents <img src="assets/document-icon.png"> in the left panel.</li> 
 <li value="4"> <p>Click&nbsp;<span class="bold">Add New</span>, then click <span class="bold">Proof</span> in the menu that appears.</p> <note type="tip">
   You can enable the 
   <span class="bold">Automatically generate proofs when uploading documents</span> setting in your user profile to automate this process. For more information, see 
   <a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a> .
  </note> </li> 
 <li value="5">In the <span class="bold">New proof</span> page that appears, continue with <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-proof.md#add-files" class="MCXref xref">Add files</a> in <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-proof.md" class="MCXref xref">Configure a proof</a>.</li> 
</ol>

## Upload a document and create a new version of a proof

1. Go to the project, task, or issue where you want to create a new version of an existing proof.
1. Click the `Documents`&nbsp;tab.
1. Select the document where you want to add a new version. 
1. Click `Add New` > `Version` > `Proof`.
1. In the `New Proof Version` page that appears, you can

  * [Create an advanced proof with a Basic workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) 
  * [Create an advanced proof with an Automated workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Use drag-and-drop to generate a&nbsp;simple proof for a new version

You can drag-and-drop a document from your file system (such as your desktop) to create a new proof or a new version of an existing proof. The proof contains the following settings, depending on whether you are creating a new proof or a new version:

* `New proof:` Creates a&nbsp;simple proof that is shared only with you.&nbsp;You can modify share settings after the proof is created as described in [Edit proof settings](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* `New version of existing proof:` Creates a new version&nbsp;with the same proof settings as the previous version.

To use drag-and-drop to generate a new proof or new proof version:

1. Ensure that proofs are configured to be automatically generated, as described in [Configure a user's proofing access](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md#configuring-proofs-to-automatically-generate) in [Configure a user's proofing access](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

1. Continue with&nbsp; [Add documents to Adobe Workfront from your file system](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), which explains the drag-and-drop method of adding documents.&nbsp;

## Create a proof for an existing document

<ol> 
 <li value="1"> <p>Go to the project, task, or issue where you want the proof, then click the <span class="bold">Documents</span> section.</p> </li> 
 <li value="2"> <p>Hover over the document, then click the <span class="bold">Create Proof</span> link that appears below the document name. </p> <note type="note">
   If you have 
   <span class="bold">Automatically generate proofs when uploading documents</span> enabled in your user profile, the system automatically creates a simple proof.
  </note> </li> 
 <li value="3">Choose one of the following:<br></li> 
 <li value="4"> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Simple Proof</td> 
     <td>This option creates a proof with no workflow attached and applies the default proof settings. You can update the default proofsettings or add a workflow after you've created the proof. For more information on proof settings, see <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Edit proof settings</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Advanced Proof</td> 
     <td> <p>This option allows you to configure a Basic or Advanced workflow and modify proof settings for the proof you create. For more information, see </p> 
      <ul> 
       <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Create an advanced proof with a Basic workflow</a> </p> </li> 
       <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Create an advanced proof with an Automated workflow</a> </p> </li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

