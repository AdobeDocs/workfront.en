---
title: Configure Global Approval Settings
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: As an Adobe Workfront administrator, you can determine the global settings for approval processes in Workfront. These settings impact all work item approval processes in your system.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
---
# Configure global approval settings

As an Adobe Workfront administrator, you can determine the global settings for approval processes in Workfront. These settings impact all work item approval processes in your system.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be either a System Administrator or have a Plan license with administrative access to Approval processes</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Configure global approval settings

{{step-1-to-setup}}

1. Click **Processes** > **Approvals**.  

1. Click the **Settings** icon ![](assets/gear-icon-settings.png) next to the **Approvals** area name.   

1. In the **Approval Settings** box that appears, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Add &lt;number&gt; Days to planned completion date to accommodate for approval processes</td> 
      <td> <p>Specify the number of minutes, hours, days, weeks, or months to add time to the planned completion date of the task that needs approval. Select "Elapsed" minutes, hours, days, or weeks to add time that includes any weekends, holidays, and non-working hours that have been designated in the system work schedule calendar.</p> 
      <p>For example, if a task is assigned on Friday and has a duration of 3 elapsed days, the task completion date is set for Monday (assuming that Saturday and Sunday is a weekend). If the task has a duration of 3 days (not elapsed), the task completion date is set for Wednesday.</p>
      <p><b>NOTE</b>: Enabling the addition of extra time to accommodate for approval on tasks will affect the timeline of the task and that of the project.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approver not required to be on the project team (for approval processes that include a role)</td> 
      <td> <p>Select this if an approver is not required to be on the project team when an approval process includes a role. When assigning the approval decision to a job role, only the users who have a role associated with them on the project will see the approval. If you enable this setting, any user with that job role receives the approval request whether they are on the project team or not. For information about editing a user's project role, see <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Manage the Project Team</a>. </p> 
      <p><b>TIP</b>: When you assign an approval to a role and the option <b>Approver not required to be on the project team (for approval processes that include a role)</b> is disabled, but there are no roles in the project team that match the role on the approval, the approval is reassigned to the Project Owner. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disable approval delegation</td> 
      <td> <p>Select this option to disable the functionality for users in your system to delegate approvals to another user. When this option is selected, the option to delegate approvals is removed from Workfront, and any existing approval delegations are stopped.</p> <p>For more information about delegating approvals in Workfront, see <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegate approval request</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow Editing the custom form when the project, task, or issue is in pending approval status</td> 
      <td> <p>Select this option to allow users to edit the custom form of projects, tasks, and issues when in the Pending Approval status. This is the default setting.</p> 
      <p>When this option is selected:</p> 
       <ul> 
       <li>All approvers (and any other users who have access to edit the custom form) can make changes to the custom form when the object is pending approval, regardless of the current approval path or approval step.</li> 
       <li>Changes that are made to the custom form during an approval process do not affect any approval decisions that were made prior to the change.</li> 
       <li> <p>Any changes made to the project, task, or issue are tracked in the same way, regardless of this setting. </p> <p>For example, if you added custom form fields to be tracked on the update stream, any changes to the form are tracked on the update stream on the object.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow users to recall newly created requests pending approval</td> 
      <td> <p>Select this option to configure whether users can recall an issue or a request pending approval for their first status. You can associate the first status of an issue or a request with an approval process by configuring requests queues. </p> 
      <p>For more information about request queues, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>.</p> 
      <p>Do one of the following:</p> 
       <ul> 
       <li>Select this option to allow users to recall an approval for the first status of an issue or a request. In this case, they can see a Recall< button on a new issue or request which is pending approval status. When they select to recall the issue, they will receive a warning that the issue will also be deleted. The issue is deleted after they have confirmed their recalling it. </li> 
       <li> <p>Deselect this option to prevent users from recalling an issue or a request whose first status is pending approval. They cannot see a Recall< button on the new issue or request and the approval must be granted. This is the default option.</p> 
       <p>For more information about reviewing items waiting for approval, see <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save Changes.**
