---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Print a proof summary within Adobe Workfront
description: You can print a proof summary, save it as a PDF, or export it as an XLS file or PDF file that is optimized for Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
---
# Print a proof summary within Adobe Workfront

You can print a proof summary, save it as a PDF, or export it as an XLS file or PDF file that is optimized for Adobe Reader.

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

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Print a proof summary or save it as a PDF file

You can print a proof summary directly from the document list.

>[!NOTE]
>
>* Summaries larger than 1 GB are not supported.
>* You cannot print multiple proof summaries from the document list at the same time.

1. From the document list that contains the proof, hover over the row containing the document, then click **Print Summary**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Or

   While viewing the proof in the the proofing viewer, click the **Print**icon ![](assets/print-icon-in-pv.png) in the left toolbar. (If the left toolbar is not visible, click the Menu icon ![](assets/menu-icon-in-pv.png) in the upper-left corner of the proofing viewer.)

1. Use any of the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Show</td> 
      <td> <p>Specify what you want to print:</p> 
       <ul> 
        <li>The <strong>Current version</strong> or <strong>All versions</strong> of the proof</li> 
        <li>Only the <strong>Pages with comments</strong> or <strong>All pages</strong></li> 
        <li>Only the <strong>Page thumbnails</strong> (a small rendering of each page)&nbsp;or <strong>Full pages</strong> (a full rendering of the proof)<br></li> 
        <p>Note:  In order to see pin numbers on markup in your printed output, you need to select Full pages, not Page thumbnails.&nbsp;</p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sort comments by</td> 
      <td> <p>(Available only if you selected Page Thumbnails above) Specify the order in which you want the proof's comments to print:</p> 
       <ul> 
        <li><strong>Oldest</strong>: From first comment made to last</li> 
        <li><strong>Latest</strong>: From last comment made to first</li> 
        <li><strong>Page</strong>: By page, from the first page to the last or from the last page to the first</li> 
        <li><strong>Creator</strong>: By the names of the users who added them, from A-Z or from Z-A</li> 
       </ul> <p>These options do not affect output you export as an XLS or PDF file.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filter comments by</td> 
      <td> <p>You can use any combination of these options to include only certain comments in the output you print or export as an XLS or PDF file:</p> 
       <ul> 
        <li>Authors you select (default)</li> 
        <li>Actions you select</li> 
        <li><strong>Unresolved</strong> status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workflow</td> 
      <td> <p>(Available only if the proof has an Automated Workflow) You can click <strong>Show diagram</strong> to include a diagram in printed output showing the stages on the proof and decisions made on each stage. In the diagram that appears, the colors represent decisions made on a stage:</p> <p><strong>Green</strong>: Approved</p> <p><strong>Blue</strong>: Pending a decision</p> <p><strong>Red</strong>: Changes required decision</p> <p><strong>Grey</strong>: Not started yet</p> <p><strong>Yellow</strong>: Approved with changes</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Print**.
1. In the right panel in the window that appears, if you want to print the summary, click the **Destination** menu, then click **See more**. Click the printer you want to use in the list that appears, then click **Print**.

   Or

   If you want to save the summary as a PDF file, click the **Destination** menu, click **Save as PDF**, then click **Save**.

## Export a proof summary as an XLS or PDF

You can export a proof summary for static content as an XLS file or as a PDF file. Proof exports include only the content of the proof.

1. From the document list that contains the proof, hover over the row containing the document, then click **Print Summary**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Click the XLS icon or PDF icon near the upper-right corner of the page.

   ![](assets/xls-pdf-icons-350x136.png)

When the exported file is ready, you receive an email from which you can download the file.

If you exported the summary as a PDF file, comments on the proof appear in the PDF reader. If a comment has multiple markups associated with it, the comment will appear multiple times in the comments list (once for each markup).
