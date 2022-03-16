---
filename: edit-proof-stages-and-reviewers
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Edit proof stages and reviewers
description: You must have the following access to perform the steps in this article:
---

# Edit proof stages and reviewers

You can edit the stages and reviewer details in a proof if you are the proof owner or creator or you have the correct proof role assigned.  

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
   <td role="rowheader">Proof role</td> 
   <td>Author or Moderator </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Edit a stage

1. In a document list that contains the document, hover over the row containing the document, then click Proof Details.

   Or

   In the standalone Workfront Proof, click the  `More` (three dot) menu to the right of the proof, then click  `View proof details`.

1. Make any of the following changes in the `Workflow` section:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Edit the deadline</td> 
      <td> <p>Select the date, and choose a new date in the calendar that appears. To remove the deadline completely, select the date, then select <span class="bold">Clear</span> below the calendar that appears.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remove individual reviewer</td> 
      <td> <p>Select the <span class="bold">More</span> menu to the right of the reviewer's name, then click <span class="bold">Remove</span> in the drop-down menu. Click <span class="bold">Confirm</span> in the box that appears to remove the reviewer from the proof.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remove multiple reviewers</td> 
      <td>Select the check boxes next to their names, then click the <span class="bold">Delete </span>icon near the upper-right corner of the stage section.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Message all reviewers</td> 
      <td>Select the <span class="bold">More</span> menu in the upper-right corner of the stage section, then select <span class="bold">Message all</span>. Configure your message, then select <span class="bold">Send</span>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add a reviewer to the stage</td> 
      <td>Select the <span class="bold">More</span> menu in the upper-right corner of the stage section, then select <span class="bold">Share</span>. Add the user and configure their role and email alerts, and repeat if needed. When finished, click <span class="bold">Share</span>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Delete the stage</td> 
      <td> <p>Select the <span class="bold">More</span> menu in the upper-right corner of the stage section, the select <span class="bold">Delete </span>stage.</p> <p>Note: If there’s only one stage, the stage cannot be deleted.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Edit reviewer details

1. In Workfront, hover over the proof, then click `Proof details` to open the Proofing Details page.
1. In the `Workflow` section, click the `More` menu ![](assets/more-button-small.png) to the right of the reviewer's name, then click `Edit` in the drop-down menu that appears.   

1. In the `Edit reviewer` box that appears, edit any of the following details: 

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Display name*</td> 
      <td> <p>To change the reviewer's display name on the proof, click in the text field and in-line edit their name.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Role</td> 
      <td>To change the reviewer's role on the proof, open the drop-down menu and select the preferred role. See <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configure default proofing roles</a> for more information.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Email alerts</td> 
      <td>To change the reviewer's email alert on the proof, open the drop-down menu and select the preferred email alert. For more information, see in the article <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">Notifications for proof comments and decisions overview</a>.</td> 
     </tr> Decision* To change the reviewer's decision on the proof, open the drop-down menu and select the preferred decision. Note that any decision you make on behalf of another user is noted in the Activity section of the proof. This option displays only when the review has made a decision. 
     <tr> 
      <td role="rowheader">Stage</td> 
      <td>It is not possible to move reviewers between stages. However, you can remove and re-add a reviewer with a different deadline.</td> 
     </tr> 
    </tbody> 
   </table>

   &#42; You must be the proof creator or owner to edit this field. 

1. Click `Save`.

