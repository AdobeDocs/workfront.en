---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Overview of modifying task assignments
description: You can assign tasks to or unassign tasks from users, teams, or job roles. You can assign multiple resources at the same time, or just one resource. You can assign one task at a time, or multiple tasks in bulk.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
---
# Overview of modifying task assignments

You can assign tasks to or unassign tasks from users, teams, or job roles. You can assign multiple resources at the same time, or just one resource. You can assign one task at a time, or multiple tasks in bulk.

>[!TIP]
>
>You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
>
>If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following: 
>
>* Reassign the work item to active resources. 
>* Associate the users in a deactivated team with an active team and reassign the work item to the active team. 
>

This article contains general information about the impact of modifying task assignments. For information about how to assign tasks, see the following articles:

* For information about assigning tasks, see [Assign tasks](../../../manage-work/tasks/assign-tasks/assign-tasks.md) and [Modify multiple user assignments in a task list](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md). 

* For information about modifying assignments on multiple tasks in the Scheduling area, see "Modify multiple users assignments to tasks in the Scheduling areas".
* For information about assigning tasks using the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Some information in this article also applies to assignments to issues. For more information about assigning issues, and additional considerations, see [Overview of modifying issue assignments](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## When to modify user assignments on tasks

You might want to modify the user assignments for tasks for a variety of reasons, including the following:

* Users join or leave your team
* A user takes a vacation that extends beyond task due dates

  >[!NOTE]
  >
  >When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role

## Considerations for multiple assignments to job roles, teams, and users

Consider the following when assigning multiple resources to a work item:

* Users can have more than one job role associated with their profile. For information about associating users with job roles, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Tasks or issues are usually first assigned to one or multiple job roles or to a team. When projects are ready to start, they might need to also be assigned to users.   
  If a task or an issue is assigned to one or multiple roles and then you also assign a user, Adobe Workfront decides which job role to associate with the additional user (if any)&nbsp;according to the following rules:

   * If there is only one job role assigned and it matches the user's Primary Role, then the task or issue is assigned only to the user fulfilling their&nbsp;Primary Role. 
   * If there are multiple roles assigned and at least one of the roles matches the user's secondary roles, then the task or issue is assigned to the user fulfilling one of their Other Roles — which Workfront selects at random if there are multiple matches — as well as any additional roles that are assigned.
   * If there is one or more job roles assigned and there are no matches to the user's roles, then the task or issue is assigned to both&nbsp;the role or roles as well as to the user.

* If a task or an issue is assigned to a team and you also assign a user, the task or issue remains assigned to both the team and the user.

## How removing assignees affects task hours and allocation percentages

Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

When you delete a user from a task with the following Duration&nbsp;Types:

* **Simple:** The planned hours assigned to that user are subtracted from the task's total planned hours.

  >[!IMPORTANT]
  >
  >This could negatively affect your project plan because it changes the total planned hours for the task and the project.

* **Effort Driven:** The allocation percentage does not change for other users. 
* **Calculated Assignment:** The allocation percentages of other users are adjusted so that the total equals 100%. 
* **Calculated Work:** The allocation percentage does not change for other users.

## Considerations about unassigning tasks

You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.

For more information about removing assignments from tasks in bulk, see [Modify multiple user assignments in a task list](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Consider the following when removing assignments from tasks:

* When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.
* When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources.
