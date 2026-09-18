---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Use the proof approval report
description: You can use the proof approval report to view information about proofs in your environment.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
TQID: https://experienceleague.adobe.com/ZU6Ej5QhI7v9zoAxurBz1YsFVIuVIh2a8tR2h6vYL18
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Use the proof approval report

You can use the proof approval report to view information about proofs in your environment.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront package</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license</p> </td> 
   <td> 
   <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configuration</strong> </td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Use the proof approval report

{{step1-to-reports}}

1. Click **New Report**, then scroll to select **Proof Approval**.

   ![Proof approval report](assets/proof-approval-report.png)

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

## About the Approver Decision field

The Approver Decision field shows the decision a recipient made on the proof. In some cases, this field displays a hyphen (-) instead of a decision value, which indicates that the recipient is no longer in a decision-making role on the proof. For more information, see [Approver Decision shows a hyphen in the Proof Approval report](../tips-tricks-and-troubleshooting/approver-decision-shows-hyphen.md).

&nbsp;
