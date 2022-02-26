---
filename: proof-approval-report
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Use the proof approval report
description: You can use the proof approval report to view information about proofs in your environment.
---

# Use the proof approval report

You can use the *proof* approval report to view information about proofs in your environment.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses overview*</p> </td> 
   <td> <p>Plan</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><span class="bold">Access level*</span> </td> 
    <td> <p>Edit access to:</p> 
     <ul> 
      <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
      <li> <p>Create Filters, Views, and Groupings</p> </li> 
     </ul> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><span class="bold">Access level*</span> </td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Use the proof approval report

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <b>Reports</b>. </p> </li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <b>Reports</b>. </p> </li> 
 <li value="2"> <p>Click <b>New Report</b>, then scroll to select <b>Proof Approval</b>.</p> <p> <draft-comment>
    <img src="assets/proof-approval-report.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/proof-approval-report.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <br> </p> </li> 
 <li value="3"> <p>(Optional) Add any additional fields. </p> </li> 
 <li value="4"> <p>Click <span class="bold">Save + Close</span>.</p> </li> 
</ol>

## Additional fields

You can add the following fields to the proof approval report:

* **Decision Date**: Displays the date an approver makes a decision on a proof. You can also find this date on the Print Summary of the proof.
* **Approver Stage**: Displays the current stage information.
* **Workflow Template**: Displays any workflow templates attached to the proof. If there is no template attached, the column is blank.
* `Awaiting decision`: Displays true to signal a decision has not been met when the following are true:

  * The proof has not been archived
  * The stage the approver is on is active
  * The proof is pending approval

* `Proof deadline`: Displays the deadline of the proof. Every stage must have a deadline assigned in order for this field to populate. The field displays the deadline for the most recently activated stage.

&nbsp;
