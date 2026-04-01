---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Create Advanced Assignments
description: You can manage task or issue assignments using Advanced Assignments.
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
---
# Create advanced assignments

{{highlighted-preview}}

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

You can manage task or issue assignments using Advanced Assignments.

You can adjust the following assignment information when making advanced assignments:

* Assign users to the task or issue (this can be accomplished outside of an advanced assignment).
* Adjust and redistribute the number of hours each assignee is allocated.
* Determine which user should be designated as the owner or the Primary assignee of the task or issue.
* Specify which role each user is fulfilling when working on the task or issue.
* <span class="preview">Add billing and cost rate information at the assignment level.</span>
* <span class="preview">Review the following details for each assignment: time-based planned hours, total cost, and total revenue.</span>

>[!NOTE]
>
>When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks and issues. For information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Areas of Adobe Workfront where you can make advanced assignments

This article describes how to access Advanced Assignments in the task or issue's header.

In addition, you can make advanced assignments in the following areas of Workfront:

* In lists and reports when the Assignments field displays in the view.
* In the Assignments section when editing a task. For more information, see [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md). <!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* In the task or issue header, in the Assignments area.
* In the Workload Balancer. For more information, see [Assign work manually using the Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>To add billing and cost rates on task assignments and use the advanced search: Workflow Ultimate</p> <p>To create advanced assignments: Any Workfront or Workflow package</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td> <p>Standard</p>
   <p>Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role>Access level configurations</td> 
   <td> <p>Edit access to Tasks and Issues</p>  </td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task or issue</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Create Advanced Assignments – Workflow Ultimate package

This layout of Advanced Assignments applies to tasks only. For issues, see [Create Advanced Assignments – all other packages](#create-advanced-assignments--all-other-packages).

1. Go to the project where you want to assign a task.
1. Click **Tasks** or **Issues** in the left panel, then click the name of a task in the list.

   >[!TIP]
   >
   >You can make advanced assignments directly on the task list. Click inside the **Assignments** field on the same line as the task, then click **Advanced** at the bottom of the list, or the **People icon** in the upper-right corner of the assignments box, to open the Advanced Assignments window. Skip to step 5 to continue creating advanced assignments.
   >![Click Advanced or the People icon](assets/access-aa-from-lists.png)

1. Click **Assign to** in the **Assignments** field in the header of the task

   Or

   Click one of the assigned names if the task is already assigned.

1. Click **Advanced**.

   ![Click Advanced](assets/assignments-from-task-header-0825.png)

   The Advanced Assignments window appears.

   ![Advanced Assignments window](assets/advanced-assignments-031826.png)

1. Review the task duration information as needed. These fields are all view-only from Advanced Assignments and you can update them in the task.

   For information about the task duration, duration types, units of time, and planned hours, see [Overview of Task Duration and Duration Type](/help/quicksilver/manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Optional) Select **Hours**, **FTE**, or **Percentage** for viewing the allocations.

   You can see how much a user is assigned in planned hours, as a percentage of their capacity, or in FTE (full-time equivalent, 0–1 scale). The default setting is Hours.

   For information on FTE, see [Configure Resource Management preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Click **New row** to add an assignment to the task.

1. Click in the **Assignee** column to add a user or a team. Start typing the name of the user or team, then click the name when it appears in the drop-down list.

   >[!NOTE]
   >
   >If the name contains a special character, you must include the special character in the search field.

   When you add a user who has a primary job role, then the **Assignee Role** is populated.

   If the user has attributes assigned to their profile, the attributes are populated on the task assignment.

1. To add a job role when you don't know the user who will work on the task, click in the **Assignee Role** column. Start typing the name of the job role, then click the name when it appears in the drop-down list.

   >[!NOTE]
   >
   >If the name contains a special character, you must include the special character in the search field.

   If the job role has attributes assigned from a project's rate card, the attributes are populated on the task assignment.

   When you assign a user later using the Assignee field, the basic search follows this algorithm:

   * Full match: Job role and all attributes
   * Partial match: Job role and some attributes
   * Job role match only

   For information about the advanced search, see [Use the advanced search](#use-the-advanced-search) in this article.

1. (Optional) Continue adding assignees in new rows to add multiple resources to the task.

   >[!TIP]
   >
   >* You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams. A maximum of 200 assignees per task is allowed.
   >
   >
   >* When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. 
   >Users must be associated with at least one job role to view it as you add them.
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* If a user, job role, or team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following: 
   >   
   >   * Reassign the work item to active resources. 
   >   * Associate the users in a deactivated team with an active team and reassign the work item to the active team.
   
1. To mark an assignee as the task owner, select the check box for the row, and click **Set primary** in the action bar at the bottom of the Advanced Assignments window.

   By default, Workfront marks the first user or job role that you assign to a task as the Owner or Primary Assignment. A team cannot be designated the Primary Owner of a task.

   If the Primary Owner of the task is not displayed, you can add the **Is Primary** column to the table.

   >[!IMPORTANT]
   >
   >Depending on how your Workfront administrator or group administrator set up your project preferences, Workfront might use the schedule of the task owner to calculate the timeline of the task when you have multiple users assigned to the task. For information about multiple task assignees, see the [Considerations for multiple assignments to job roles, teams, and users](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) section in the article [Assign tasks](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

1. For each user in the **Assignee** column, specify the following information:

   * (Optional) **Job role for billing**: Search for and select the job role for billing for this specific assignee and task.

      The job role for billing is only used on this assignment and is not automatically applied to the user's other assignments. For example, a user's primary job role is Designer, but on one task they are acting as a Senior Designer and the billing rate should reflect that. The job role for billing applies only to users and cannot be used on other job roles.

      When a job role for billing is applied on the user assignment, the rate attached to the job role for billing may be used instead of the user or job role rates in billing and revenue calculations.

      A project-level job role for billing can also be set for a user, and that value is used on all of the user's assignments on that project.

      For more information, see [Set up a Job Role for Billing](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

   * **Allocation**: When the Duration Type of a task is Simple, specify the number of hours each user or job role should be assigned to the task. The sum of all assigned hours for each user is equal to the number in the **Planned Hours** field at the top of the Advanced Assignments window. In all other cases, specify the percentage of time (or allocation) that you want the assignee to spend solving the task.

     >[!TIP]
     >
     >After you manually modify assignment allocations on tasks, the Planned Hours of the tasks might update accordingly. Note that you cannot manually modify allocations for teams assigned to tasks. For more information, see the section [Update task Planned Hours when managing user allocations](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) in the article [Planned Hours overview](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

   * **Attributes**: Any attributes available for the user are shown in the attribute fields. The administrator sets up the attributes and they are added to the user profile or associated with a job role in a rate card. For more information, see [Define rate attributes](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) and [Edit a user's profile](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Attributes are currently read-only on user assignments. They are editable for job roles.

   * **Rate currency**: The currency for the billing and cost rates is defaulted from the project, but you can change the currency for this assignment.

   * (Optional) **Billing rate**: The billing rate can come from other areas of the system, such as rate cards. For more information, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). You can manually override the billing rate for this specific assignment in this field, and it will override all other rates for the user in revenue calculations.
   * (Optional) **Cost rate**: The cost rate can come from other areas of the system. For more information, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). You can manually override the cost rate for this specific assignment in this field, and it will override all other rates for the user in cost calculations.
   * **Is Billable**: Select this option to include the assignment in financial calculations. Clear this option to exclude the assignment from financial calculations.

     This field is turned on by default for all assignments when the task has a revenue type.

1. (Optional) To view assignment data by date for a user or role, select the table row and click **View by dates** in the action bar at the bottom of the Advanced Assignments window. For more information, see [View assignment data by dates](#view-assignment-data-by-dates) in this article.
1. (Optional) To delete one or more assignments from the list, select the check box for each row, and click **Delete** in the action bar at the bottom of the Advanced Assignments window.
1. Click **Save** or **Save and close** when you are finished editing the Advanced Assignments.

### Add and remove columns on the Advanced Assignments list

Fields must exist before you can add them to the list.

1. Click **+** on the top right of the list to open the **Column manager**.

   ![Advanced Assignments Column manager](assets/aa-column-manager.png)

1. Select the **Properties** tab or the **KPIs** tab to choose the type of field you want to add.

   Properties such as location or cost center provide contextual information. Time-phased KPIs such as revenue or cost break down values across time periods.

1. Search for an existing object field in the **Available** section, then click **+** to the right of the field name it to add it to the **Selected** column.
1. Click **-** to the right of a field in the **Selected** section to remove it from the list.
1. Click **Save**.

   For more information on the Column manager, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Apply a view to the Advanced Assignments list

A view is a personalized set of column arrangements that you can apply to the list.

1. Click the **Views** dropdown and select the view you want to apply to the list.

   **System Views** are views that the system administrator added, and they cannot be changed. **My Views** are views that you created or were shared with you.

1. Click **New view** in the **Views** dropdown to create a view.

   When you add, remove, or reorder the columns the changes are saved to the view automatically. The next time you apply this view, the columns remain the way you set them.

   For more information on views, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Use the Advanced search

The advanced search helps you locate the correct user or job role to add to the assignment.

1. To open the advanced search window, do one of the following:

   * Click **Advanced Search** at the top right of the Advanced Assignments window.
   * Select an assignment row and click **Advanced Search** in the action bar at the bottom of the Advanced Assignments window. This opens the advanced search with filters automatically applied for that specific assignment.

1. Select the Users or Job Roles tab on the advanced search window.
1. Apply filters as needed:

   1. Click **Filter** above the list.
   1. In the Filter box, click **Add condition**.
   1. Select a field to filter by.
   1. Select a filter modifier, such as "Has any of," "Has none of," "Is before," or "Is after." The modifier options are different depending on the type of field you are filtering by.
   1. Select the field value or values. Depending on the field type you are filtering by, you might be prompted to select the item from a list, search for it, or use a calendar to select a date range.

   The filter is applied to the list automatically. For more information on filters, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

1. Search for a job role or user.

   When searching for a user who matches a job role assignment, only full matches (job role and all attributes) are displayed.

1. Click **+** to add columns to the table. For more information, see [Add and remove columns on the Advanced Assignments list](#add-and-remove-columns-on-the-advanced-assignments-list).
1. Select one or more users or job roles, and click **Add Users** or **Add Roles** in the action bar at the bottom of the window.

   The assignments are added on the Advanced Assignments window.

### View assignment data by dates

The **View by dates** window for Advanced Assignments shows the entire date-effective history of the assignment for a specific user or role. Both past and future changes are displayed.

Examples of date-effective items that could affect the assignment history are:

* User's Primary/Other Job Roles
* Project-level Job Role for Billing
* User profile billing/cost rates
* Project override billing/cost rates (user or job role)
* Rate card rates by job role/attributes
* User Attributes
* User schedule

Note that this is not a comprehensive list, and the field that changed is not necessarily displayed in the table of assignment data, but it affects the billing and cost rates or attributes for the user or job role.

You can only view assignment data by dates for a single user or role.

1. Select the table row for a user or role, and click **View by dates** in the action bar at the bottom of the Advanced Assignments window.

   The **View by dates** window appears. The data is read-only.

   Each row in the table represents a date-effective change on the assignment. If no date-effective changes have taken place, the table will have one row showing the current data. Highlighted fields point out what has changed, and the start and end date for each update is listed. For example, if the billing rate changed from 202 on August 20 to 205 on August 21, the rate is highlighted. The text in parentheses indicates where the change was made to the rate, such as a project.

   ![View by dates window](assets/resource-changes-view-by-dates.png)
 
   When you are finished reviewing the data, click the arrow on the top left to return to the Advanced Assignments window.

</div>

## Create Advanced Assignments – all other packages

This layout of Advanced Assignments applies to both tasks and issues.

1. Go to the project where you want to assign a task or an issue.
1. Click **Tasks** or **Issues** in the left panel, then click the name of a task or issue in the list.

   >[!TIP]
   >
   >You can make advanced assignments directly on the task or issue list. Click inside the **Assignments** field on the same line as the task or issue, then click **Advanced** at the bottom of the list, or the **People icon** in the upper-right corner of the assignments box, to open the Advanced Assignments window. Skip to step 5 to continue creating advanced assignments.
   >![Click Advanced or the People icon](assets/access-aa-from-lists.png)

1. Click **Assign to** in the **Assignments** field in the header of the task or issue

   Or

   Click one of the assigned names if the task or issue is already assigned.

1. Click **Advanced**.

   ![Click Advanced](assets/assignments-from-task-header-0825.png)

1. In the **Search people, role and teams** field, start typing the name of a user, role, or team, then click the name when it appears in the drop-down list.

   >[!NOTE]
   >
   >If the user's name contains a special character, you must include the special character in the search field.

1. (Optional) Continue adding assignees in the **Search people, role and teams** box to add multiple resources to the task or issue.

   >[!TIP]
   >
   >* You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
   >
   >
   >* When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. 
   >Users must be associated with at least one job role to view it as you add them.
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* If a user, job role, or team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following: 
   >   
   >   * Reassign the work item to active resources. 
   >   * Associate the users in a deactivated team with an active team and reassign the work item to the active team.

1. For each user in the **Assignee** column, specify the following information:

   * **Owner**: Hover over the name of the assignee and click **Make Primary** in the Owner field if you want to mark the assignee as the task or issue owner. A green checkbox indicates that the specified user is the Primary Contact of the task or issue. Adobe Workfront marks the first user or job role that you assign to a task or issue as the Owner or Primary Assignment. A team cannot be designated the Primary Owner of a task or issue.

     >[!IMPORTANT]
     >
     >Depending on how your Workfront administrator or group administrator set up your project preferences, Workfront might use the schedule of the task owner to calculate the timeline of the task when you have multiple users assigned to the task. For information about multiple task assignees, see the [Considerations for multiple assignments to job roles, teams, and users](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) section in the article [Assign tasks](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Allocations**: When the Duration Type of a task is Simple, specify the number of hours each user or job role should be assigned to the task. The sum of all assigned hours for each user is equal to the number in the **Planned Hours** field at the bottom of the  Allocations  column. In all other cases, specify the percentage of time (or allocation) that you want the assignee to spend solving the task or issue.

     >[!TIP]
     >   
     >   * After you manually modify assignment allocations on tasks, the Planned Hours of the tasks might update accordingly. For more information, see the section [Update task Planned Hours when managing user allocations](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) in the article [Planned Hours overview](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).
     >   * You cannot manually modify assignment allocations on issues. 
     >   * You cannot manually modify allocations for teams assigned to tasks.

   * **Assignee's Role:** Select the role the user should use when fulfilling this assignment.  The Primary Role of the user displays by default. Click in the **Assignee's Role** box to select another role. When you assign the task or the issue to a role first, and then add a user who can fulfill that role as a second assignment, the list of suggested users is filtered for the users who can fulfill the roles already assigned to the task and issue.

     ![Assignee's Role](assets/advanced-assignments-select-role.png) 

   * **Duration Type**: This is only available for tasks. Click the name of the Duration Type and select a Duration Type from the drop-down menu. For information about Duration Types, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
   
   * **Duration:** You can update this field for a task when you have Manage permissions to the task.

     For more information, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). When bulk editing assignment information, a similar dialogue box appears to assign users, hours, allocation, and task owner.
   
   * **Planned Hours**: When the Duration Type is Calculated Assignment or Simple, update the number of Planned Hours. The allocation percentages or the hours for each resource are distributed evenly as a result. Workfront calculates the Planned Hours when the Duration Type is Calculated Work or Effort Driven. For more information, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. Click **Save**.


