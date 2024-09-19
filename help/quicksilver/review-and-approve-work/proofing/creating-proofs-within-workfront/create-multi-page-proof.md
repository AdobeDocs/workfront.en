---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Create a multi-page proof
description: You can combine multiple files into a single multi-page proof. Reviewers can use the navigation tools in the proofing viewer to browse through the pages in a multi-page proof.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
---
# Create a multi-page proof

You can combine multiple files into a single multi-page proof. Reviewers can use the navigation tools in the proofing viewer to browse through the pages in a multi-page proof.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
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

&#42;To find out what plan, license, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Create a multi-page proof

When this option is enabled, static files and websites are available in a single proof. When this option is disabled, all documents and websites are generated as individual proofs, and you can upload up to 100 files at a given time.

To create a multi-page proof:

1. Go to the project, task, or issue where you want the proof, then click the **Documents** section.
1. Click **Add new** > **Proof** . 
1. Drag and drop the files or browse and select them from your file explorer. You can upload up to 50 files at a time. For information on file limits, see the [Considerations](#considerations) section in this article.

   >[!NOTE]
   >
   >Interactive files, including videos and interactive websites, cannot be combined into a single proof.

1. Under **Single proof**, enable the option, **Combine all compatible files into single proof**.
1. In the&nbsp;**Proof name**&nbsp;field, specify a new name for the combined proof.
1. (Optional) In list of files you have uploaded,&nbsp;reorder the files by dragging them. The order of the files is&nbsp;the page order of the combined&nbsp;proof.
1. (Optional) To remove a single file from the New&nbsp;proof page, hover over the file and click the **Trash** icon that appears on the right.

   Or

   To delete all uploaded files at once, click **Delete all**&nbsp;in the upper-right corner of the list.

1. Once all of your files are uploaded, you must decide if you want to configure a basic proof or an automated proof:

   * With a basic proof, you can add as many reviewers as you want to a proof, but they are not organized into stages. All of the reviewers you add can access the proof immediately after you create it. To configure a basic proof, see [Create an advanced proof with a Basic workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * With an automated proof, the proof moves from stage to stage and Adobe Workfront notifies each user when it is their turn to review it. to configure an automated proof, see [Create an advanced proof with an Automated workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Considerations {#considerations}

Consider the following when combining files into a single proof:

* You can upload up to 500 separate files.
* You can combine static files of different types (for example, PDF, JPG, DOC, PPT, EXC), up to a total of 2,000 pages.
* You can combine static web captures.
* You can combine GIF files; however, animated GIFs are processed as static files.
* You cannot combine AV files and Interactive web captures.
* The proof's thumbnail image is taken from the first page of the proof (see [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* You can check the names of files that were combined to create the proof on the Proof details page. For more information, see [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* If the option to&nbsp;download the original files is enabled on the proof, you can download all the files that have been combined in order to create the proof as a .zip file. For more information, see&nbsp; [Download Files Stored in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
