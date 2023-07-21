---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modify multiple user assignments in a task list
description: When managing task assignments, you can simultaneously modify them for multiple tasks at a time by using the bulk editing feature in a list of tasks. 
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
---
# Modify multiple user assignments in a task list

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

When managing task assignments, you can simultaneously modify them for multiple tasks at a time by using the bulk editing feature in a list of tasks. 

This article refers to modifying multiple user assignments for multiple tasks in a task list. Also see the following articles for modifying assignments on multiple tasks in other areas:

* For information about assigning tasks using the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

For information about assigning a task to one resource in a list, see [Assign tasks](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Access requirements

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Modify assignments for multiple tasks

1. Go to the list that contains the tasks where you want to modify assignments.
1. (Optional) Create a filter to display only tasks assigned to the assignee that you want to modify.

   For example, if your project contains a specific role as the default assignee for multiple tasks, you can create a filter to display only tasks with that role as the assignee. Then, you can replace the role with a specific user.

   For information about creating a filter, see [Create or edit filters](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md). 


1. To filter on a role, select **Assignment Roles**, then click **ID**.

      >[!TIP]
      >
      >Do not use the **Assigned to** field. This finds only the Primary Owner for the task instead of any of the roles that could be assigned to them.

      Or

      To filter for a user, select **Assignment Users,** then click **ID.**

      >[!TIP]
      >
      >Do not use the **Assigned to** field. This finds only the Primary Owner for the task instead of any of the users that could be assigned to them.

1. Select the tasks for which you want to modify assignments, then click the **Edit** icon ![](assets/edit-icon.png).

   The Edit Tasks page displays. The items that you edit display in the upper-left corner of the page.

1. Go to the **Assignments** section.
1. Do one of the following to add or remove assignees:

   >[!IMPORTANT]
   >
   >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

   * To add a new assignee:

      1. In the **Assignments** section, select **Assignee**.

         Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
      
      1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.


      >[!TIP]
      >
      > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
      >   
      > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
      > 
      >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
      >   
      >     * Reassign the work item to active resources.
      >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


   * To remove individual assignees:

      1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

         Or

         (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

   * To remove all existing assignees:

      1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

         This removes not only common assignees (assignees that are displayed in the edit&nbsp;dialog box), but also all assignees on all the selected tasks.

      Removing users from tasks can affect task hours and allocation percentages.
      
      For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Optional) Modify any of the following options for assignees:

   * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

     >[!NOTE]
     >
     >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration&nbsp;Type is Simple you can update the Hours. For information about Duration&nbsp;Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

   * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
   * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user.

1. Click **Save Changes.**
