---
product-area: projects
navigation-topic: manage-tasks
title: Delete Tasks
description: You can delete tasks that might be duplicates, or have been created in error.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6O1uHSRp9a7NndhRMlRRCdozG56yiVBqhactYgL0aHg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Delete tasks

You can delete tasks that might be duplicates, or have been created in error.

For tasks that have historical information (updates, changes of schedule, status, or other fields), we recommend that you close them or mark them Dead, instead of deleting them. This helps you keep the historical information for your projects.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p> 
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects with access to Delete</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p></td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
Old:

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
   <td> <p>Edit access to Tasks and Projects with access to Delete</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Understand the process of deleting tasks

* [Limitations for deleting tasks](#limitations-for-deleting-tasks) 
* [The impact of deleting tasks](#the-impact-of-deleting-tasks)

### Limitations for deleting tasks  {#limitations-for-deleting-tasks}

* When a project has a status of Complete you can delete tasks only if your Workfront administrator or a group administrator has allowed this in your Project Preferences area. For information about setting up project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* If the task has logged hours, the Workfront  or group administrator must allow the deletion of these tasks by configuring the Task & Issue Preferences in your Workfront instance. This also applies when you try to delete projects that have tasks with hours logged on them. 

  <!--
  (NOTE: the last statement is NWE only; not possible in classic)
  -->

  For more information about enabling the deletion of tasks where hours are logged, see the "Deletion" section in [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### The impact of deleting tasks {#the-impact-of-deleting-tasks}

When you delete a task, you impact other objects linked to the task.

Consider the following: 

* The following objects attached to a task are also deleted when you delete a task:

   * Documents

   You cannot delete a task that has a document which has been checked out attached to it. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

   You cannot restore individual documents that were deleted when the task was deleted from the Documents tab in the Recycle Bin. You can only restore the documents deleted when the task was deleted when you restore the task.

   * Issues
   * Subtasks
   * Notes
   * Approvals

* Depending on how your Workfront administrator configures the Project, Task, or Issue Deletion Preferences in the Timesheet & Hour Preferences of your Workfront instance, hours logged for the tasks are handled in one of the following ways when deleting a task:

   * Move to the project and will not be restored on the task, if the task is later restored.
   * Are deleted and will be restored on the task, if the task is later restored.

   This also applies when you try to delete projects that have tasks with hours logged on them.

   For more information about configuring the deletion preferences for hours logged on issues, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
   * Expenses on the task will move to the project.

   * The users assigned to the task or to the task approval remain on the project team.

   For more information about project teams, see [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

* When you delete a child task and you move its parent to another project, then restore the deleted child task, the task is added back on the original project as a main task. 

<!--
   
  (NOTE: this stays NWE; not possible in classic;)
   
  -->

## Delete tasks

* [Delete multiple tasks in a project simultaneously](#delete-multiple-tasks-in-a-project-simultaneously) 
* [Delete a single task](#delete-a-single-task)

### Delete multiple tasks in a project simultaneously  {#delete-multiple-tasks-in-a-project-simultaneously}

{{step1-to-projects}}

1. Click the project name that contains the tasks you want to delete.
1. Click **Tasks** in the left panel.  
1. Do one of the following:

   1. (Conditional) When the **Autosave** toggle is enabled:

      1. Select the tasks you want to delete, then click **More**
      1. Click **Delete**, then **Delete** to confirm the deletion.

         The tasks are deleted.

   1. (Conditional) Click the **Plan Mode** icon and select **Manual save** if you want to reverse the changes you make to the task list.

      ![Select Manual Save](assets/manual-save-option.png)

      Do the following:

      1. Select the tasks you want to delete. 
      1. Click **Delete**.
      1. (Optional) Click **Undo** to reverse your change and not delete the tasks.
      1. Click **Redo** if you want to keep the change and delete the task.
      1. Click **Save** to delete the tasks.

         Tasks are deleted only after you save your changes.

### Delete a single task {#delete-a-single-task}

{{step1-to-projects}}

1. Click the project name that contains the task you want to delete.
1. Click **Tasks** in the left panel. 
1. Click the name of the task you want to delete.
1. Click the **More** icon ![More menu](assets/qs-more-menu.png)in the upper-right corner.

   ![Delete tasks at the task level](assets/delete-tasks-task-level-nwe-350x225.png)

1. Click **Delete Task**.
1. If the deletion is allowed, click **Delete**.

   Your Workfront administrator or group administrator might not allow the deletion of tasks where hours are logged.

   For more information about the access and permissions needed to delete a task, see the section [Limitations for deleting tasks](#limitations-for-deleting-tasks) in this article.

## Restore deleted tasks

A Workfront or group administrator can restore tasks within 30 days after they are deleted, as described in [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
