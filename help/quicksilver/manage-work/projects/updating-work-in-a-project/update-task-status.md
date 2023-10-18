---
product-area: projects
navigation-topic: update-work-in-a-project
title: Update task status
description: You can update a task's status to inform others about where the task is (and the overall project) and how it is progressing.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
---
# Update task status

You can update a task's status to inform others about where the task is (and the overall project) and how it is progressing.

The default statuses are New, In Progress, and Complete. Your Adobe Workfront administrator can add custom statuses for your organization. For more information, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

You can manually update task statuses or you can let Workfront automatically update them when certain actions take place.

## Access requirements

<!--drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

You must have the following access to manually update tasks: 

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations about updating the Status of tasks

* When you mark a task as Complete, the percent complete of the task updates to 100%. 
* The following scenarios exist for parent tasks: 
  * You cannot update the Status of a parent task to Complete when the Summary Completion Mode of the project is set to Automatic and the subtasks are not completed.
  * You can update the Status of a parent task to Complete when the Summary Completion Mode of the project is set to Manual and the subtasks are completed or incomplete. 

  For more information, see [Edit projects](../manage-projects/edit-projects.md).

## Manually update task status

When you are updating a task status, you can also type an explanation about the new status and change other task information such as the due date.

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![](assets/drag-the-progress-bar-350x155.png)

## Automatically update task status

Workfront automatically updates the existing status of a task to a different status when the actions listed in the table below occur.

>[!NOTE]
>
>The statuses in the following table are default system statuses. Your Workfront administrator or a group administrator can rename the statuses in your instance of Workfront. For information about creating and managing statuses in Workfront, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Action</td> 
   <td>Original Status</td> 
   <td>New Status</td> 
  </tr> 
  <tr> 
   <td>Update the task percent complete to 100%</td> 
   <td>New or In Progress</td> 
   <td>Complete</td> 
  </tr> 
  <tr> 
   <td>Update the task percent complete from 100% to a lower number</td> 
   <td>Complete</td> 
   <td>In Progress</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Click the Start Task button to accept working on a task assigned to you</span> </td> 
   <td><span>New</span> </td> 
   <td> <p>Any status associated with the Start Task button in your Home Team settings.</p> <p>For information about replacing the Work On It button with a Start Task button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <p>Tip: <span>Clicking</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">the Undo button</span>after clicking Start Task reverts the status to New. </p> </td> 
  </tr> 
 </tbody> 
</table>
