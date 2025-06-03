---
product-area: projects
navigation-topic: manage-tasks
title: Move Tasks
description: You can move tasks to different projects or to different parent tasks in Adobe Workfront. 
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
---
# Move tasks

<!--Audited: 5/2025-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


You can move tasks in Adobe Workfront between the following objects:

* An ad hoc task to a project.
* A task from a project to another project.
* A task from a project under a different parent in another project. 
* A task within the same project under a different parent.

You can move a task at the task level, or you can move a task from a list of tasks.

You can move a single task, or you can move several tasks at a time from a list of tasks. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
 <p>or</p>  
<p>Current: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks</p> <p>Contribute or higher permissions to the project with ability to Add Tasks</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations for moving tasks

Consider the following when moving a task: 

* Your system or group administrator can prevent you from moving tasks that have logged hours depending on how they configure the Allow users to move tasks and issues with logged hours preference in the Setup area. For information, see [Configure system-wide task and issue preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md). 

* When you move a task from one project to another, the task dates might be recalculated. The recalculation will take into consideration the schedule that the new project uses and the project's Schedule From information.

* You can move some items associated with the task to the moved task during the moving process. However, by default, the following objects transfer to the moved task:

   * Issues
   * Logged hours
   * User comments
   * Custom forms and custom field information
   * Subtasks

* By default, the following items don't move with the task:

   * Milestones

## Move tasks in a list

{{step1-to-projects}}

1. On the **Projects** page, select the project that contains the task or tasks you want to move.
1. Click **Tasks** in the left panel to display the task list. 
1. Click the **Plan Mode** icon ![Plan mode icon](assets/plan-mode.png) and ensure that the **Autosave** toggle is enabled, then select the task or tasks that you want to move.

   ![Autosave option](assets/autosave-icon.png)

   >[!IMPORTANT]
   >
   >You cannot move tasks when the **Autosave** toggle is disabled.

1. (Optional and conditional) If you want to move the selected tasks within the same project, click the tasks you selected, then drag and drop them to where you want them moved to on the project. The task hierarchy changes save immediately and the information associated with each task is moved with the tasks.

1. (Conditional) Select the task or tasks that you want to move and do one of the following:

   * Click the **More** menu ![More icon](assets/main-more-icon.png) at the top of the task list, then click **Move to**. 
   * Right-click the selected tasks, then click **Move to**.
   * When selecting one task, click the **More** menu ![](assets/more-icon-task-list.png) next to the task name in the list, then click **Move to**.

   The **Move Task** box displays.

1. Continue with moving the task, as described in the section [Move a task at the task level](#move-a-task-at-the-task-level) in this article. 

   <!--
   is this still accurate?!
   -->

## Move a task at the task level {#move-a-task-at-the-task-level}

In addition to moving tasks from a list of tasks, you can move a task at the task level after you have opened it. 

1. Find a task in your Workfront system by searching for it.
1. Click the name of the task to open it.
1. Click the **More** drop-down menu ![More icon](assets/main-more-icon.png) next to the task name, then click **Move to**. The **Move Task** side panel displays.

1. (Optional) Update the **Task Name**. The task moves with the new name in the new location.

   >[!TIP]
   >
   >The **Task Name** field is dimmed and not editable when selecting to move multiple tasks in a list. You can hover over the **Task Name** field and a list of all selected tasks will display.
   >
   >
   >![Display task names](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. In the **Select Destination Project** field, type the name of the project you want the task to move to. If you want to move the task within the same project, type the name of the current project.

   >[!TIP]
   >
   >* The project name is case sensitive. 
   >* You can search for a project by typing the Reference Number or entering the ID of the project. This can help you distinguish between projects with identical names. 
   >* Only 100 projects display in the list.

1. (Conditional) If you don't have access to the project, click **Request access**. 
1. (Conditional) Continue to move the task to the destination project without requesting access if you have access to add tasks to one of the tasks on the destination project.

   ![Moving a task without requesting access](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Similar messages display if the project selected is in pending approval, completed, or dead when the Workfront administrator prevents adding tasks to these projects. For more information, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optional) In the **Options** section, deselect any of the items listed in the table below to remove them from the moved tasks. All options are selected by default.

   >[!IMPORTANT]
   >
   >Deselecting items in the **Options** list results in loss of data. Information from the existing task will be removed and can't be recovered.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Select all</td> 
      <td>Deselect this option to remove all information from the task when moving it to its new location. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Constraint</td> 
      <td> <p>The task constraint is set to As Soon As Possible or As Late As Possible based on the project Schedule Mode setting.</p> <p> When selected, the current constraint of the task transfers with the task. </p> 
      <p>Note: When moving or copying a task with date-specific constraints to another project and the constraint dates of the task are outside the new project dates, either the Task Constraint changes to As Soon as Possible or As Late as Possible, or the Planned Start or Planned Completion dates of the projects are adjusted. 
      
      The following are examples of date-specific constraints:
      <ul>
      <li> Start On</li>
      <li> Must Finish On</li>
      <li> Start No Earlier Than</li>
      <li> Start No Later Than</li>
      </ul>
      
      For more information, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assignments</td> 
      <td> <p>All the assignments are removed from the task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approval Process</td> 
      <td>All approval processes are removed from the task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress</td> 
      <td>The task status is set to New. Otherwise, the existing task status is preserved. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financial Information</td> 
      <td>The financial information of the task is removed and the Workfront updates the task Cost Type to No Cost and the task Revenue Type as Not Billable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">All Predecessors</td> 
      <td> <p>When selected, the dependency becomes a cross-project predecessor when you move the task to another project. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>The documents attached to the task aren't transferred to the moved task. This includes versions, proofs, and linked documents.</p> <p>This doesn't include document approvals. Document approvals can never be moved when a task is moved.</p> 
      <p>Note: If you opt to not have the documents moved with the task, the documents will be deleted and placed in the Recycle Bin for 30 days. An administrator can restore them and they will be restored on the moved task. </p>
    
    <p>If the task is deleted after it's moved, the restored documents will be placed in the Documents area of the user page of the administrator who restores them.</p>
      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reminder Notifications</td> 
      <td>The task reminders do not transfer to the moved task. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Expenses</td> 
      <td>The expenses logged on the task do not transfer to the moved task. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permissions</td> 
      <td> <p>Workfront removes the names of all the entities displaying in the Sharing list of the task. </p> </td> 
     </tr> 
    </tbody> 
   </table>

 

1. (Optional) In the **Select Parent** section, select the task in the destination project that will become the parent of the moved task.

   >[!TIP]
   >
   >When selecting to move multiple tasks in a list, all selected tasks become the children of the selected parent.

   Select a parent by doing one of the following:

   * In the task list, select one of the parents in the project plan.
   * Click the search icon ![Search icon](assets/search-icon.png) and search for a parent task by name.

   The task displays in the list.

   ![Select parent task when moving a task with search functionality ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

   >[!NOTE]
   >
   >If you do not select a parent task, the tasks are moved as main tasks rather than subtasks, and they are placed at the end of the task list on the destination project.

1. Click **Move task**. The tasks move to the specified project as either subtasks to a parent task or the last tasks on the project.
