---
filename: assign-tasks
product-area: projects;user-management
navigation-topic: assign-tasks
title: Assign tasks
description: You can assign tasks to users, roles, or teams to indicate who is responsible for completing the tasks. You can assign a task to more than one resource at a time.
---

# Assign tasks

You can assign tasks to users, roles, or teams to indicate who is responsible for completing the tasks. You can assign a task to more than one resource at a time. 

` `**Tip: **`` You can assign multiple users or job roles, and you can assign only one team. `You can assign only active users, `job roles`, and teams.`

`If a user, `job role`, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:`

* `Reassign the work item to active resources.` 
* `Associate the users in a deactivated team with an active team and reassign the work item to the active team.`

The number of users assigned to a task and the schedule of the task Owner can modify the planned dates of a task which results in changing the timeline of the project. For information about the impact of assigning multiple users to a task, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

In addition to this article, we recommend that you read the following articles for more information about assigning tasks:

* [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md) 
* [Smart assignments overview](../../../manage-work/tasks/assign-tasks/smart-assignments.md) 
* [Make smart assignments](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md) 
* [Create advanced assignments](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) 
* [Modify multiple user assignments in a task list](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md) 
* [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md) 
* [Plan a project overview](../../../manage-work/projects/planning-a-project/plan-project.md) 
* [Overview of the task Planned Completion Date](../../../manage-work/tasks/task-information/task-planned-completion-date.md) 
* [Set the project Planned Completion Date](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md) 
* [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 
* [Overview of assigning work in the Adobe Workfront Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Work</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Considerations for multiple assignments to job roles, teams, and users

Consider the following when assigning multiple resources to a work item:

* Users can have more than one job role associated with their profile. For information about associating users with job roles, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Tasks or issues are usually first assigned to one or multiple job roles or to a team. When projects are ready to start, they might need to also be assigned to users.   
  If a task or an issue is assigned to one or multiple roles and then you also assign a user, `Adobe Workfront` decides which job role to associate with the additional user (if any)&nbsp;according to the following rules:

  * If there is only one job role assigned and it matches the user's Primary Role, then the task or issue is assigned only to the user fulfilling their&nbsp;Primary Role. 
  * If there are multiple roles assigned and at least one of the roles matches the user's secondary roles, then the task or issue is assigned to the user fulfilling one of their Other Roles — which `Workfront` selects at random if there are multiple matches — as well as any additional roles that are assigned.
  * If there is one or more job roles assigned and there are no matches to the user's roles, then the task or issue is assigned to both&nbsp;the role or roles as well as to the user.

* If a task or an issue is assigned to a team and you also assign a user, the task or issue remains assigned to both the team and the user.

<!--
Considerations for multiple user assignments and using schedules You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. When you assign multiple users to a task, your Workfront administrator or a group administrator determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: The Primary Assignee's schedule: this is the schedule associated with the user designated as the task Owner. For information about associating users with schedules, see Edit a user's profile. The Project's schedule: this is the schedule associated with the project. For adding a schedule to a project, see Edit projects. For information about setting up which schedule a project uses in the case of multiple assignments, see Configure system-wide project preferences.
-->

##

## Assign a single task

1. Go to a task that you want to assign.
1. Click Assign to in the upper-right corner of the task header, in the Assignments area Or Click the name of the current assignments, if the task is already assigned.  
1. Do one of the following:

  * Start typing the name of a user, role, or team that you want to assign, then click it when it appears on the list.

1. Click Save. 
1. (Optional) Click the X icon next to the name of the assignments in the Assignments area in the header of the task to remove an assignment.

## Assign a task in a list

You can assign tasks in a list or a report when any of the assignments fields are visible in the list's view. This is a faster way to assign tasks. This article describes how to modify assignments for one task in a list.&nbsp;For information about modifying multiple assignments for multiple tasks in a list, see [Modify multiple user assignments in a task list](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Depending on which field is visible in the view, you can assign the following entities to the task: 

| `Assign To`  |Assign one user  |
|---|---|
| `Assigned`  |Assign one user |
| `Assignments`  |Assign users, job roles, or a team |

To assign tasks in a list:

<ol> 
 <li value="1"> <p>Go to a list of tasks that has the Assigned To, Assigned, or Assignments fields in the view.</p> </li> 
 <li value="2"> (Optional) Click the Plan Mode icon and select one of the following options: 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Autosave</td> 
     <td>Changes you make to the tasks are automatically saved and you cannot revert them</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Manual save</td> 
     <td>You must manually save your changes. You can revert your changes before you save them. You have the option of selecting Standard Manual save or Timeline Planning.</td> 
    </tr> 
   </tbody> 
  </table> <p>For more information about saving tasks as you edit them in a list, see <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Edit tasks in a list</a>.</p> </li> 
 <li value="3"> <p>To assign tasks do one of the following:</p> 
  <ul> 
   <li> <p>Click inside the <span class="bold">Assigned To</span> or <span class="bold">Assigned</span> fields and start typing the name of an active user that you want to assign to the task, then click it when it displays in the list.</p>  </li> 
   <li> <p>Click inside the <span class="bold">Assignments</span> field and start typing the name of an active user, <span>job role</span>, or team that you want to assign to the task, then click it when it displays in the list.</p>  </li> 
  </ul> </li> 
 <li value="4"> <p>After adding your assignees to the task, press Enter or click anywhere on the page to save your changes if you selected Autosave. Otherwise, click<span class="bold"> Save</span>. </p> </li> 
</ol>

## Assign multiple tasks to a user

<ol> 
 <li value="1">Go to a list of tasks that you want to assign in bulk. </li> 
 <li value="2"> <p>(Conditional) Ensure that the <span class="bold">Autosave</span> option is selected if you are on a list of tasks under a project.</p> <note type="important">
   You cannot edit tasks in bulk when saving tasks manually on a project.
  </note> </li> 
 <li value="3"> Select several tasks in the tasks list. </li> 
 <li value="4"> Click the Edit icon . <p>The <span class="bold">Edit Tasks</span> dialog box opens.</p> </li> 
 <li value="5"> <p>In the <span class="bold">Assignments</span> area, select the <span class="bold">Assignee</span> box, then start typing the name of a user, job role, or team that you want to assign to all the tasks. </p> <note type="important">
   If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks. 
  </note> </li> 
 <li value="6">(Optional) Select the radio button in the <span class="bold">Task Owner</span> column to indicate which resource is the primary assignee or the Owner of the task, when you assign more than one resource to the task. This is not available for teams. </li> 
 <li value="7"> <p>(Conditional) Specify the <span class="bold">Allocation %</span> for each resource assigned to the task if all the tasks you selected have a Duration Type of Effort Driven or Calculated Assignment. This indicates how much of their time these resources should spend on completing the task. This is only available for users and job roles. </p> <p>Or </p> <p>Specify the amount of <span class="bold">Hours</span> for each resource assigned to the task if all the tasks you selected have a Duration Type of Simple. The total of all hours for all resources should equal the number of Planned Hours for the task. </p> <note type="important">
   You cannot specify the allocation percentage or the number of hours per resource if the tasks you selected have different Duration Types or of the tasks you selected have different Duration Types.
  </note> <p> For information about Duration Type on tasks, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> </li> 
 <li value="8">(Optional) Select a role that the user should fulfill on the task from the <span class="bold">Pick a role</span> drop-down menu in the <span class="bold">Assignee's Role</span> column when you assign users to tasks. If you do not select a role, <span>Workfront</span> automatically selects the user's Primary Role. </li> 
 <li value="9">(Optional) If you want to remove existing assignees from all tasks do one of the following:
  <ol>
   <li value="1">Start typing the name of a user, role, or team you want to remove from the task, then select it when it appears on the list and click <span class="bold">Remove Assignee</span> to remove more assignees.</li>
   <li value="2">Click <span class="bold">Remove All Existing Assignees</span> to remove all assignees from all selected tasks.</li>
  </ol></li> 
 <li value="10">Click <span class="bold">Save Changes</span>.</li> 
 <li value="11">(Optional and conditional) When the Assigned to or the Assignments fields display in your list of tasks, click inside one of these columns for a task, then click the <span class="bold">X icon</span> next to the name of an assignee to remove it from the task. </li> 
</ol>

<!--
Considerations about unassigning tasks You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk. For more information about removing assignments from tasks in bulk, see Modify multiple user assignments in a task list. Consider the following when removing assignments from tasks: When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task. When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources.
-->

