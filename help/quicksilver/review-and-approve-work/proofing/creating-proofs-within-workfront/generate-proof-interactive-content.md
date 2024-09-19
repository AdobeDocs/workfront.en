---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Create a proof for interactive content in a ZIP file
description: You can generate a proof for non-website interactive content stored in a ZIP file. Examples of this type of web content include ads with streaming video or audio, HTML animations, Interactive banners.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
---
# Create a proof for interactive content in a ZIP file

You can generate a proof for non-website interactive content stored in a ZIP file. Examples of this type of web content include ads with streaming video or audio, HTML animations, Interactive banners.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
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

+++

## Create a proof for interactive content in a ZIP file

Once you add interactive content in a ZIP file to a proof, Adobe Workfront&nbsp;creates a proof of the zipped&nbsp;documents. Depending on the file size, the upload loading time can vary. Larger files take longer to create. You can navigate away from the page and Workfront&nbsp;continues to create your file.&nbsp;The maximum file upload size is 4GB.&nbsp;

1. Prepare your content by creating a ZIP bundled file.

   The ZIP file must meet the following requirements:

   * All assets, such as CSS, JavaScript, videos, sounds, and images should be included in the bundle file.
   * Make sure the main file (such as index.html, index.htm) is in the root folder and that it is the only .html/.htm file stored there.

     If the main file is not placed in the root folder, Workfront searches the folder to find the main file.
   
   * Maximum bundle size is 500 MB.
   * In the case of ZIP files created in iOS, the tool automatically identifies the right folder where the content is placed.

1. Go to the project, task, or issue where you want to upload the ZIP file.
1. Click **Documents**&nbsp;in the left panel .
1. Click **Add New**, then click**Proof** in the menu that appears.
1. In the **Add Files** section, drag and drop or browse for the ZIP&nbsp;file you need.
1. Click **Create proof** to create a simple proof with no review process.  
   or  
   Continue by configuring an advanced proof:

   * [Create an advanced proof with a Basic workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Create an advanced proof with an Automated workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
