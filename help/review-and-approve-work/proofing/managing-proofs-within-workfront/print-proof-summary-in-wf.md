---
filename: print-proof-summary-in-wf
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Print a proof summary within Adobe Workfront
description: You can print a proof summary, save it as a PDF, or export it as an XLS file or PDF file that is optimized for Adobe Reader.
---

# Print a proof summary within Adobe Workfront

You can print a proof summary, save it as a PDF, or export it as an XLS file or PDF file that is optimized for Adobe Reader.

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

## Print a proof summary or save it as a PDF file

You can print a proof summary directly from the document list.

>[!NOTE]
>
>You cannot print multiple proof summaries from the document list at the same time.

<ol> 
 <li value="1"> <p>From the document list that contains the proof, hover over the row containing the document, then click <span class="bold">Print Summary</span>.</p>  <p>Or</p> <p>While viewing the proof in the the proofing viewer, click the <span class="bold">Print&nbsp;</span>icon <img src="assets/print-icon-in-pv.png"> in the left toolbar. (If the left toolbar is not visible, click the Menu icon <img src="assets/menu-icon-in-pv.png"> in the upper-left corner of the proofing viewer.)</p> </li> 
 <li value="2"> <p>Use any of the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Show</td> 
     <td> <p>Specify what you want to print:</p> 
      <ul> 
       <li>The <span class="bold">Current version</span> or <span class="bold">All versions</span> of the proof</li> 
       <li>Only the <span class="bold">Pages with comments</span> or <span class="bold">All pages</span></li> 
       <li>Only the <span class="bold">Page thumbnails</span> (a small rendering of each page)&nbsp;or <span class="bold">Full pages</span> (a full rendering of the proof)<br></li> <note type="note">
         In order to see pin numbers on markup in your printed output, you need to select Full pages, not Page thumbnails.&nbsp;
       </note> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Sort comments by</td> 
     <td> <p>(Available only if you selected Page Thumbnails above) Specify the order in which you want the proof's comments to print:</p> 
      <ul> 
       <li><span class="bold">Oldest</span>: From first comment made to last</li> 
       <li><span class="bold">Latest</span>: From last comment made to first</li> 
       <li><span class="bold">Page</span>: By page, from the first page to the last or from the last page to the first</li> 
       <li><span class="bold">Creator</span>: By the names of the users who added them, from A-Z or from Z-A</li> 
      </ul> <p>These options do not affect output you export as an XLS or PDF file.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Filter comments by</td> 
     <td> <p>You can use any combination of these options to include only certain comments in the output you print or export as an XLS or PDF file:</p> 
      <ul> 
       <li>Authors you select (default)</li> 
       <li>Actions you select</li> 
       <li><span class="bold">Unresolved</span> status</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Workflow</td> 
     <td> <p>(Available only if the proof has an Automated Workflow) You can click <span class="bold">Show diagram</span> to include a diagram in printed output showing the stages on the proof and decisions made on each stage. In the diagram that appears, the colors represent decisions made on a stage:</p> <p><span class="bold">Green</span>: Approved</p> <p><span class="bold">Blue</span>: Pending a decision</p> <p><span class="bold">Red</span>: Changes required decision</p> <p><span class="bold">Grey</span>: Not started yet</p> <p><span class="bold">Yellow</span>: Approved with changes</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3">Click <span class="bold">Print</span>.</li> 
 <li value="4"> <p>In the right panel in the window that appears, if you want to print the summary, click the <span class="bold">Destination</span> menu, then click <span class="bold">See more</span>. Click the printer you want to use in the list that appears, then click <span class="bold">Print</span>.</p> <p>Or</p> <p>If you want to save the summary as a PDF file, click the <span class="bold">Destination</span> menu, click <span class="bold">Save as PDF</span>, then click <span class="bold">Save</span>.<br></p> </li> 
</ol>

<!--
For information about using and customizing decisions, see Configure approval decision options in Workfront Proof.
-->

## Export a proof summary as an XLS or PDF

You can export a proof summary for static content as an XLS file or as a PDF file. Proof exports include only the content of the proof.

<!--
You can't include a diagram showing the stages and decisions made on the proof.
-->

<ol> 
 <li value="1"> <p>From the document list that contains the proof, hover over the row containing the document, then click <span class="bold">Print Summary</span>.</p>  </li> 
 <li value="2"> <p>Click the XLS icon or PDF icon near the upper-right corner of the page. </p> <p> <img src="assets/xls-pdf-icons-350x136.png" style="width: 350;height: 136;"> </p> </li> 
</ol>

When the exported file is ready, you receive an email from which you can download the file.

If you exported the summary as a PDF file, comments on the proof appear in the PDF reader. If a comment has multiple markups associated with it, the comment will appear multiple times in the comments list (once for each markup).
