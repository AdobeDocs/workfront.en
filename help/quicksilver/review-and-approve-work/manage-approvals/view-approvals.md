---
product-area: projects
navigation-topic: approvals
title: View approvals
description: Approval processes provide the flexibility to create multistep approvals for projects, tasks, and issues. Adobe Workfront administrators define approval processes to provide consistency throughout the system.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
---
# View approvals

Approval processes provide the flexibility to create multistep approvals for projects, tasks, and issues. Adobe Workfront administrators define approval processes to provide consistency throughout the system.

For information about creating approval processes, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

For information about associating approvals with work in Workfront, see [Associate a new or existing approval process with work](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the objects associated with approvals</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the objects associated with approvals</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Locate approvals in Adobe Workfront

You can view or manage approvals from several areas of Workfront. For information about how to manage approvals in various areas, see [Approving work](../../review-and-approve-work/manage-approvals/approving-work.md).

You can view or manage approvals from the following areas:

* In the Home area

   * All projects, tasks, issues, timesheets, documents, and access awaiting your approval are displayed in the My Approvals widget in the Home area.
   * Approvals that you submitted yourself also display in the My Approvals widget in the Home area when you choose the Approvals I've submitted filter option. For more information, see the [Review work you submit for approval in the Home area](#review-work-you-submit-for-approval-in-the-home-area) section in this article.
   * Approvals are removed from the My Approvals widget in the Home area when the associated project, task, or issue is marked Resolved, On Hold, Closed, or Canceled.

  For information about using Home, see [Get started with Home](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md). 

* In the header of a project, task, issue, document, or proof 
* In the Approvals section of a project, task, or issue
* In a report

  >[!NOTE]
  >
  >You cannot make a decision on an approval from a report.

  You can create a project, task, issue, or document approval report that contains approval information.

  For information about creating reports, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Review work you submit for approval in the Home area {#review-work-you-submit-for-approval-in-the-home-area}

1. Click the **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) Click **Customize** to add the **My Approvals** widget.
1. (Conditional) Click the **Filter** drop-down menu, then select **Approvals I've submitted** to see approvals you've submitted.


## View the approval status of an object

You can view the approval status of an object in the following sections of the object:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Updates </td> 
   <td> <p>Displays all approval statuses when they occur. Approval statuses display in line with other statuses displayed on the <strong>Updates</strong> section.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Approvals</td> 
   <td> <p>Displays more detailed information about the approval process, such as each stage of the approval process and whether approvers have granted the approval.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Use the Updates area to view&nbsp;an approval status {#use-the-updates-area-to-view-an-approval-status}

When an approval is initiated on a project, task, or issue, a status displays in the **Updates** tab of the object, indicating the approval status. A new status displays any time the object transitions through the approval process. This includes the following events:

* An approval process is initiated on an object. The approval process is initiated when the status is changed.
* The object is rejected
* The object is approved

>[!TIP]
>
>If an approval is applied to a task, the approval updates are shown on the Updates tab of the task, not on the Updates tab of the project where the task resides.

### Use the Approvals area to view an approval status {#use-the-approvals-area-to-view-an-approval-status}

You can gain visibility into where a task or issue that you are working on currently is in the approval process. You can see the following information:

* The phase of the approval process
* Which approvers have already approved it
* Which approvers have not yet approved it

To see the current state of where a task or issue is in the approval process:

1. Go to the project, task, or issue that the approval is associated with.
1. In the left panel, click **Approvals**. You might need to first click **Show More**.

   The Approvals tab displays&nbsp;the full information about all past approval paths and stages. You can see exactly who made a decision on the approval or whether the approval is set for a team, job role, or user.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   For information about creating an Approval Process, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
