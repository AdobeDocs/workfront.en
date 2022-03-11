---
filename: wf-adobe-xd-proofs
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Upload XD art boards as proofs to Workfront
description: You can upload your art boards as proofs directly to Adobe Workfront for a thorough review and approval.
---

# Upload XD art boards as proofs to Workfront

You can upload your art boards as proofs directly to Adobe Workfront for a thorough review and approval.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Proof</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have an Adobe Creative Cloud license in addition to a Workfront license.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Prerequisites

* You must install the Workfront for Adobe XD plugin before you can upload proofs in Adobe XD.

  For instructions, see [Install Workfront for Adobe XD](../../workfront-integrations-and-apps/adobe-workfront-for-xd/wf-adobe-xd-install.md).

## Upload a static Proof

<ol> 
 <li value="1"> <p>Click the <span class="bold">Menu</span> icon in the top-right corner, then select <span class="bold">Work List</span>. You can also use the menu to navigate to parent objects.<br></p> <p> <img src="assets/menu-350x627.png" style="width: 350;height: 627;"> <br> </p> </li> 
 <li value="2">Go to the work item where you want to upload a static proof.</li> 
 <li value="3">Click the <span class="bold">Document</span> icon <img src="assets/documents.png"> in the navigation bar. </li> 
 <li value="4">Click <span class="bold">New File</span> near the bottom of the plugin.</li> 
 <li value="5"> <p>Select the art boards you wish to upload.</p> <note type="tip">
   To select more than one art board, click and drag the mouse over the art boards you want.
  </note> </li> 
 <li value="6">Choose the <span class="bold">Asset Type</span> from the drop-down menu.<br>
  <table cellspacing="0">
   <col>
   <col>
   <tbody>
    <tr>
     <td colspan="2" role="rowheader">Export Format</td>
    </tr>
    <tr>
     <td role="rowheader">.png</td>
     <td>The art board upoads as a .png to the work item's Documents tab in WorkfrontWork. </td>
    </tr>
    <tr>
     <td role="rowheader">.jpg</td>
     <td>The art board uploads as a .jpg to the work item's Documents tab in Workfront. <br></td>
    </tr>
    <tr>
     <td role="rowheader">.svg</td>
     <td>The art board uploads as a .svg to the work item's Documents tab in Workfront. </td>
    </tr>
    <tr>
     <td role="rowheader">.pdf</td>
     <td>The art board uploads as a .pdf to the work item's Documents tab in Workfront.</td>
    </tr>
   </tbody>
  </table></li> 
 <li value="7">In the <b>Proof Approvals</b> section, click <span class="bold">Add Approvers</span>, then type the names of the users you want to tag for approval from the <span class="bold">Approvers</span> drop-down menu that appears.<br>Or<br>Click <span class="bold">Select Proof workflow</span>, then select the workflow from the <span class="bold">Workflow Template</span> drop-down menu that appears.</li> 
 <li value="8"> <p>(Optional) Type a comment in the <span class="bold">Updates</span> area.</p> <p> <img src="assets/proof-approvals-xd-350x847.png" style="width: 350;height: 847;"> </p> </li> 
 <li value="9"> <p>Click <span class="bold">Upload</span>.<br>The document appears in the Documents area in the plugin and the desktop app.</p> </li> 
</ol>

## Upload an interactive proof

You can create an interactive proof for your art boards with the Workfront for Adobe plugin. It is a 2-step process. First you need to create an interactive link, then you need to upload the proof to a work item.

### Create an interactive link for your art board

<ol> 
 <li value="1">Open your art board, then click <span class="bold">Share</span> in the top-left area of the screen.</li> 
 <li value="2"> <p>Specify the link settings:</p> 
  <ol> 
   <li value="1"> <p>Name the link.</p> </li> 
   <li value="2"> <p>Choose a view setting.</p> </li> 
   <li value="3"> <p>In the <span class="bold">Link Access</span> section, ensure <span class="bold">Anyone with this link</span> is selected.</p> <p>You must enable this type of access in order to generate an interactive proof. </p> </li> 
   <li value="4"> <p>Click <span class="bold">Create Link</span>.</p> </li> 
  </ol> </li> 
 <li value="3"> <p>Click back to <span class="bold">Design</span> in the top-left area of the screen. Continue to the <a href="#upload" class="MCXref xref">Upload an interactive proof</a> section below. </p> <note type="note">
   You may need to reopen the plugin panel in the bottom-left corner of the screen.
  </note> </li> 
</ol>

### Upload an interactive proof

<ol> 
 <li value="1"> <p>Click the <span class="bold">Menu</span> icon in the top-right corner, then select <span class="bold">Work List</span>. You can also use the menu to navigate to parent objects.<br></p> <p> <img src="assets/menu-350x627.png" style="width: 350;height: 627;"> <br> </p> </li> 
 <li value="2">Go to the work item where you want to upload an interactive proof.</li> 
 <li value="3">Click the <span class="bold">Document</span> icon <img src="assets/documents.png"> in the navigation bar. </li> 
 <li value="4">Click <span class="bold">New File</span> near the bottom of the plugin.</li> 
 <li value="5"> <p>In the <span class="uitext">Asset Type </span>drop-down menu, choose the link you just created under the <span class="bold">Shared links</span>.<br><img src="assets/shared-links-xd-350x870.png" style="width: 350;height: 870;"></p> </li> 
 <li value="6">In the <span class="bold">Proof Approvals</span> section, click <span class="bold">Add Approvers</span>, then select the users you want to tag for approval from the <span class="bold">Approvers</span> drop-down menu that appears.<br>Or<br>Click <span class="bold">Select Proof workflow</span>, then select the workflow from the <span class="bold">Workflow Template</span> drop-down menu that appears.</li> 
 <li value="7">(Optional) Type a comment in the <span class="bold">Updates</span> area.</li> 
 <li value="8"> <p>Click <span class="bold">Upload</span>.</p> <p>The document appears in the Documents area in the plugin and the desktop app.</p> <note type="important">
   Users must have access to the Desktop Proofing Viewer to review and approve interactive proofs. For more information, see 
   <a href="../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md" class="MCXref xref">Install the Desktop Proofing Viewer with Automatic Updates</a>.
  </note> </li> 
</ol>

## Upload a new proof version

You can upload a new version of a proof. The plugin remembers the proofing workflow set on the previous version, but you can change this if you wish.

<ol> 
 <li value="1"> <p>Click the <span class="bold">Menu</span> icon in the top-right corner, then select <span class="bold">Work List</span>. You can also use the menu to navigate to parent objects.<br></p> <p> <img src="assets/menu-350x627.png" style="width: 350;height: 627;"> <br> </p> </li> 
 <li value="2">Go to the work item you need to upload a document to.</li> 
 <li value="3">Click the <span class="bold">Document</span> icon <img src="assets/documents.png">in the navigation bar. </li> 
 <li value="4">Click <span class="bold">New Version</span> near the bottom of the plugin.</li> 
 <li value="5"> <p>Select the art boards you wish to upload.</p> <note type="note">
   If you want to upload a new version of an .svg, .png, or .jpg, you can upload only one art board.
  </note> </li> 
 <li value="6">Choose the <span class="bold">Asset Type</span> from the drop-down menu.<br>
  <table cellspacing="0">
   <col>
   <col>
   <tbody>
    <tr>
     <td colspan="2" role="rowheader">Export Format</td>
    </tr>
    <tr>
     <td role="rowheader">.png</td>
     <td>The art board uploads as a .png to the work item's Documents tab in Workfront. </td>
    </tr>
    <tr>
     <td role="rowheader">.jpg</td>
     <td>The art board uploads as a .jpg to the work item's Documents tab in Workfront. </td>
    </tr>
    <tr>
     <td role="rowheader">.svg</td>
     <td>The art board uploads as a .svg to the work item's Documents tab in Workfront. </td>
    </tr>
    <tr>
     <td role="rowheader">.pdf</td>
     <td>The art board uploads as a .pdf to the work item's Documents tab in Workfront. </td>
    </tr>
    <tr>
     <td role="rowheader">Shared links</td>
     <td>Proofs with shared links uploaded to Workfront don't technically need to have a new version uploaded. Because they are interactive, the link is always up to date with the most recent changes. However, you can still upload a new version if you want to capture that it is a new iteration of the asset ready for another round of review and approval.</td>
    </tr>
   </tbody>
  </table></li> 
 <li value="7">In the <span class="bold">Proof Approvals</span> section, click <span class="bold">Add Approvers</span>, then select the users you want to tag for approval from the <span class="bold">Approvers</span> drop-down menu that appears.<br>Or<br>Click <span class="bold">Select Proof workflow</span>, then select the workflow from the <span class="bold">Workflow Template</span> drop-down menu that appears.</li> 
 <li value="8"> <p>(Optional) Type a comment in the <span class="bold">Updates</span> area.</p> <p> <img src="assets/proof-approvals-xd-350x847.png" style="width: 350;height: 847;"> </p> </li> 
 <li value="9">Click <span class="bold">Upload</span>.<br>The document appears in the Documents area in the plugin and the desktop app.</li> 
</ol>

