---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Use the proof approval report
description: You can use the proof approval report to view information about proofs in your environment.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
---
# Use the proof approval report

You can use the proof approval report to view information about proofs in your environment.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following:

<table style="table-layout:auto"> 
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
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level*</strong> </td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Use the proof approval report

{{step1-to-reports}}

1. Click **New Report**, then scroll to select **Proof Approval**.

   ![](assets/proof-approval-report.png)

1. (Optional) Add any additional fields. 
1. Click **Save + Close**.

## Additional fields

You can add the following fields to the proof approval report:

* **Decision Date**: Displays the date an approver makes a decision on a proof. You can also find this date on the Print Summary of the proof.
* **Approver Stage**: Displays the current stage information.
* **Workflow Template**: Displays any workflow templates attached to the proof. If there is no template attached, the column is blank.
* **Awaiting decision**: Displays true to signal a decision has not been met on the latest version when the following are true:

   * The proof has not been archived
   * The stage the approver is on is active
   * The proof is pending approval

* **Proof deadline**: Displays the deadline of the proof. Every stage must have a deadline assigned in order for this field to populate. The field displays the deadline for the most recently activated stage.

&nbsp;
