---
filename: view-approvals
product-area: projects
navigation-topic: approvals
title: View approvals in Adobe Workfront
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# View approvals in Adobe Workfront

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

Approval processes provide the flexibility to create multistep approvals for projects, tasks, and issues. Adobe Workfront administrators define approval processes to provide consistency throughout the system.

For information about creating approval processes, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

For information about associating approvals with work in Workfront, see [Associate a new or existing approval process with work](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>View or higher permissions to the objects associated with approvals</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Locate approvals in Adobe Workfront

You can view or manage approvals from several areas of Workfront. For information about how to manage approvals in various areas, see [Approving work in Adobe Workfront](../../review-and-approve-work/manage-approvals/approving-work.md).

You can view or manage approvals from the following areas:

<ul> 
 <li> <p>In the Home area</p> 
  <ul> 
   <li> <p>All projects, tasks,&nbsp;issues, timesheets,&nbsp;documents, and access awaiting your approval are displayed in the Home area when you select to view All or Approvals.</p> </li> 
   <li> <p>Approvals that you submitted yourself also display in the Home area, in the Approvals I've Submitted section of the Work List. For more information, see the <a href="#review" class="MCXref xref">Review work you submit for approval in the Home area</a> section in this article.</p> </li> 
   <li> <p>Approvals&nbsp;are removed from the Home area when the associated&nbsp;project, task, or issue&nbsp;is marked&nbsp;Resolved, On Hold, Closed, or Canceled. </p> </li> 
  </ul> <p>For information about using Home, see <a href="../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Get started with Home</a>. </p> </li> 
 <li> <p>In the header of a project, task, issue, document, or proof </p> </li> 
 <li> <p>In the Approvals sectionof a project, task, or issue</p> </li> 
 <li> <p>In a report</p> <note type="note">
   You cannot make a decision on an approval from a report.
  </note> <p>You can create a project, task, issue, or document approval report that contains approval information.</p> <p>For information about creating reports, see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
</ul>

## Review work you submit for approval in the Home area

<ol> 
 <li value="1"> 
  <div> 
   <p>Click the <span class="bold">Home</span> icon <img src="assets/home-icon-30x29.png" style="width: 30;height: 29;"> in the upper-left corner of Adobe Workfront.</p> <note type="note"> 
    <p>Your Workfront administrator might make the following changes to the Home icon in your environment:</p> 
    <ul> 
     <li> <p>Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. </p> </li> 
     <li> <p>Replace the page linked to it with a different page. In this case, click the <span class="bold">Main Menu</span> <img src="assets/main-menu-icon.png"> in the upper-right corner of the page, then click <span class="bold">Home</span>.</p> </li> 
    </ul> 
   </note> 
  </div> </li> 
 <li value="2"> <p>Select <span class="bold">Work List</span>, then click the <span class="bold">Filter</span> drop-down menu  and select <span class="bold">Approvals</span>.</p> </li> 
 <li value="3"> <p>Expand the <span class="bold">Approvals I've Submitted</span> section and find the approvals you submitted. </p> <p> <img src="assets/approvals-i've-submitted-section-in-home-350x532.png" style="width: 350;height: 532;"> </p>  </li> 
</ol>

##

## View the approval status of an object

You can view the approval status of an object in the following sectionsof the object:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Updates </td> 
   <td> <p>Displays all approval statuses when they occur. Approval statuses display in line with other statuses displayed on the <span class="bold" style="font-weight: normal;">Updates</span> section.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Approvals</td> 
   <td> <p>Displays more detailed information about the approval process, such as each stage of the approval process and whether approvers have granted the approval.</p> </td> 
  </tr> 
 </tbody> 
</table>

* [Use the Updates area to view an approval status](#using-the-updates-tab-to-view-approval-status) 
* [Use the Approvals area to view an approval status](#using-the-approvals-tab-to-view-approval-status)

### Use the Updates area to view&nbsp;an approval status

When an approval is initiated on a project, task, or issue, a status displays in the `Updates` tab of the object,&nbsp;indicating the approval status. A new status displays&nbsp;any time the object transitions through the approval process. This includes the following events:

* An approval process is initiated on an&nbsp;object. The approval process is initiated when the status is changed.
* The object is&nbsp;rejected
* The object&nbsp;is approved&nbsp;

>[!TIP]
>
>If an approval is applied to a task, the approval updates are shown on the Updates tab of the task, not on the Updates tab of the project where the task resides.

### Use the Approvals area to view an approval status

You can gain visibility into where a task or issue that you are working on currently is in&nbsp;the approval&nbsp;process. You can see the following information:

* The phase of the approval process
* Which approvers have already approved it
* Which approvers have not yet approved it

To see the current state of where a task or issue is in the approval process:

1. Go to the project, task, or issue that the approval is associated with.
1. In the left panel, click Approvals. You might need to first click Show More. The Approvals tab displays the full information about all past approval paths and stages. You can see exactly who made a decision on the approval or whether the approval is set for a team, job role, or user. For information about creating an Approval Process, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

