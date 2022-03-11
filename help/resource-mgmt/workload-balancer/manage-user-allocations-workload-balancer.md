---
filename: manage-user-allocations-workload-balancer
product-area: resource-management
navigation-topic: the-workload-balancer
title: Manage user allocations in the Workload Balancer
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Manage user allocations in the `Workload Balancer`

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

As a Resource Manager, you can assign work to users and manage their daily, weekly, `or monthly` allocations from the `Workload Balancer` to ensure they are allocated an amount of hours that fits in their available schedules.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration*</td> 
   <td> <p>Edit access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher that include Make Assignments to the tasks <span>and issues</span> that you want to manage allocations for. </p> <p>Or </p> <p>Manage permissions to the tasks what you want to update the Planned Hours for, in addition to updating allocations. For information about updating Planned Hours in the <span>Workload Balancer</span>, see the <a href="#update" class="MCXref xref">Update task Planned Hours when managing user allocations</a> section in this article. </p> <p>For information about tasks permissions, see <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task in&nbsp;Adobe Workfront</a><span> and for information about issue permissions, see</span> <span href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></span>. </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Understand user allocations

User allocations are amounts of hours that indicate the time that a user should spend on one given day or week day, week, `or month` to complete the work item. They are included in the Planned Hours of the work item.

This article describes how to update daily, weekly, or monthly hourly allocations for users assigned to tasks or issues. For information about managing overall allocations for users and job roles to tasks, see [Manage allocation hours on tasks](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md) .

* [User allocation overview](#overview) 
* [Criteria that reset user allocations](#criteria)

### User allocation overview

You can display user allocation as hours `or as a percentage value` in the `Workload Balancer`. You can adjust hours `or percentages`.

User allocations are included in the number of Planned Hours of a work item. For information about Planned Hours, see [Planned Hours overview](../../manage-work/tasks/task-information/planned-hours.md).

The task Planned Hours are distributed equally between all the days within the Duration of the task for the user assigned to the task. For example, if a task has a Duration of 5 days and a total of 10 Planned Hours, the number of daily allocations for the task is 2 hours. The weekly allocation is 10 hours. This means, that a user is allocated to work on the task for 2 hours each day. However, you can manually change the daily allocation for the user using the `Workload Balancer`.

` `**Warning: **``The `Workload Balancer` displays only up to 1000 Planned Hours per work item. The allocations in the `Workload Balancer` display as zero after the 1000 hour limit is reached. We recommend dividing the task in smaller subtasks to accommodate for a larger number of Planned Hours.

Consider the following when locating daily, weekly `or monthly` allocations for tasks `or issues` in the `Workload Balancer`:

<ul> 
 <li> <p>You can view daily, weekly, <span>and monthly</span> allocations of the users to their work items. Enable the Week <span>or Month</span> view to display weekly <span>or monthly</span> allocations. </p> </li> 
 <li> <p>You can use the <span>Workload Balancer</span> to modify the daily, weekly <span>or monthly</span> allocation of the users to the tasks <span>or issues</span>. For information about adjusting the view of the <span>Workload Balancer</span>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>. </p> <note type="note">
   We recommend that you make a decision which time frame (daily, weekly, 
   <span>or monthly</span>) you want to always use when managing user allocations and not switch between them for the same work items. Updating weekly allocations for the same user for which you previously updated daily allocations changes the daily allocation for the user. 
  </note> </li> 
 <li>You can update allocations for both working and non-working days. </li> 
 <li> <p>The time stamps for the Planned Start and Planned Completion Dates of the work items as well as the Schedule of the project are important when <span>Adobe Workfront</span> automatically calculates the daily allocation for the task. For example, a task may have a Duration of 2 days and 8 Planned Hours and it has a Planned Start time of 4:30 PM with a Project Schedule that ends at 5:00 PM. In this case, the daily allocation for one user is 0.50 hours for the first day of the task and 7.50 hours for the second day. </p> <note type="tip">
   Two users in different timezones or Schedules in different timezones than those of the assigned users can cause the allocation amounts to appear differently to two users viewing the same work items. 
  </note> </li> 
 <li> <p> When a user has scheduled time off, the day or the portion of the day displays in a gray background. If the <span>Workfront administrator</span> enabled the User Time Off setting in the Setup area to take into consideration the user's time off, the allocated hours move to the next available day in the timeline. If the setting is disabled, the allocated hours remain on the day marked for time off and the user displays as overallocated. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> <note type="tip">
   If the time off was marked after the user was assigned to a work item, you must recalculate the project's timeline to display the moved allocation. For information, see 
   <a href="../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.
  </note> </li> 
 <li> <p>If there are multiple users assigned to the task, the amount of the Planned Hours is distributed evenly to each user first, then evenly to each day within the Duration of the task. This distribution becomes the allocation of each user to the task. </p> <p>For example, the following scenarios might exist:</p> 
  <ul> 
   <li>For a task with a Duration of 2 Days and with 10 Planned Hours assigned to one user, the daily allocation for the user is 5 hours for each day by default. </li> 
   <li>For a task with a Duration of 2 days and with 10 Planned Hours assigned to two users, the daily allocation for each user is 2.5 hours for each day by default. </li> 
  </ul> </li> 
 <li> <p>If a task or issue completed before the Planned Completion Date, the number of allocated hours for the remaining days is struck through and does not count towards the user's overall allocation. This displays only when both the Show allocations icon and the Show Projected Dates setting are enabled. For more information about enabling settings in the <span>Workload Balancer</span>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> <p> <img src="assets/allocations-struck-through-highlighted-350x39.png" style="width: 350;height: 39;"> </p> </li> 
</ul>

<ul> 
 <li>When a user is overallocated, their allocated hours display with a red background in the user field.</li> 
 <li>When the user is underallocated or allocated an equal amount of hours to their scheduled available time, the hours display with a blue background. </li> 
 <li> <p>You can display the users' allocation in a chart view in the user line. For information about enabling the chart view for user allocations, see the "Navigate the Workload Balancer" section in the article <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>. </p> <p> <img src="assets/user-allocation-chart-350x237.png" style="width: 350;height: 237;"> </p> </li> 
</ul>

###

### Criteria that reset user allocations

Not all task changes trigger the modified allocations to redistribute. However, there are certain actions that could reset the already adjusted allocations on your resources and redistribute them evenly to all the days during the duration of the work item for each of the assignees.

>[!NOTE]
>
>`If you have not modified the automatic distribution of allocations on work items, the hours redistribute evenly among all the assignees when there is a change in the number of assignees, the Duration of a task, or the amount of Planned Hours on the work item.`

* [Actions that reset adjusted allocations](#actions) 
* [Actions that do not reset adjusted allocations](#actions2)

#### Actions that reset adjusted allocations

The following actions either reset or modify the daily, weekly `or monthly` allocations for users after you have manually adjusted them as described in the [Modify user allocations](#modify) section in this article:

* When you shorten the length of a work item which shortens the amount of days in its Duration, the adjusted allocated hours from the lost days is added to the allocation amount of the last day of the work item. 
* When you change the amount of Planned Hours on an assignment or on the work item, the new number of Planned Hours redistributes uniformly for the entire Duration of the work item.
* When you add or remove an assignee to a work item and this causes the Planned Hours of the task to change, the adjusted values redistribute uniformly.

#### Actions that do not reset adjusted allocations

The following changes to a work item do not trigger the adjusted allocations to reset or modify:

* When you move the days of a work item but the amount of days in the Duration does not change, the adjusted allocated values stay the same and move to the new dates. 
* When you increase the Duration of a work item which increases the number of days in its Duration, the adjusted allocated hours remain the same for the adjusted days. Additional days are added to the work item with 0 allocated hours. 
* When you add or remove an assignee to a work item and this does not cause the Planned Hours of the item to change, the adjusted values remain the same.

## Locate Planned Hours in the `Workload Balancer`

You can modify user allocations to tasks `or issues` using the `Workload Balancer` by finding the Planned Hours of the tasks `or issues` assigned to users.

Consider the following when viewing Planned Hours in the `Workload Balancer`:

* The total Planned Hours for a task `or an issue` display next to the Task `or `Issue` Name` on the left of the `Workload Balancer`.

* The total Planned Hours for a project displays next to the Project Name on the left of the `Workload Balancer`. This represents the total of Planned Hours for all the tasks `and issues` listed under the project in the `Workload Balancer` and not all the Planned Hours of the project. 
* The amount of time allocated daily or weekly for all task and for all project displays only when you manually enable the Show allocations setting. For information about enabling settings in the `Workload Balancer` see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Modify user allocations

As part of assigning work to users, you can modify user allocations in the `Workload Balancer` to ensure that they are never overallocated, or to ensure an accurate balance of hours between your resources. For information about identifying whether a user is overallocated, see the section [User allocation overview](#overview) in this article.

<ol> 
 <li value="1"> <p>Ensure you have tasks <span>and issues</span> assigned to users. For information about assigning work to users in the <span>Workload Balancer</span> see <a href="../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md" class="MCXref xref">Overview of assigning work in the Adobe Workfront Workload Balancer</a>.</p> </li> 
 <li value="2">Go to the <span>Workload Balancer</span> .</li> 
 <li value="3"> <p>(Optional) Click <span class="bold">Week</span> <span>or <span class="bold">Month</span></span> to manage weekly <span>or monthly</span> allocations for users. </p> <p> <img src="assets/month-icon-on-toolbar-selected-wb-350x226.png" style="width: 350;height: 226;"> </p> </li> 
 <li value="4"> <p>In the <span class="bold">Assigned Work</span> area, find the user that you want to manually modify the allocation for, and click the right-pointing arrow to the left of the user name to expand the user.</p> <p> <img src="assets/wb-highlight-on-name-caret-350x106.png" style="width: 350;height: 106;"> </p> </li> 
 <li value="5"> <p>Click the right-pointing arrow to the left of the project name to expand the project and display the work items that the user is assigned to. </p> <note type="tip">
   You can modify user allocations only for tasks and issues. You cannot modify user allocations for projects. 
  </note> </li> 
 <li value="6"> <p>(Optional) Click the <span class="bold">Show allocations icon</span> <img src="assets/show-allocations-icon-small.png"> to display allocations for all work items. </p> <p>The name of the tasks and of the projects is replaced with the allocation of the user for the task or the project. </p> </li> 
 <li value="7"> <p>(Optional)&nbsp;Click the <span class="bold">Settings</span> icon <img src="assets/gear-icon-settings.png"> and select any of the following options:</p> 
  <ol> 
   <li value="1"><span class="bold">Include hours from issues</span>.&nbsp;This allows you to manage issue allocations in addition to task allocations. </li> 
   <li value="2"><span class="bold">Show completed work</span> . This displays items that have been completed and are scheduled during the timeline you manage allocations for. </li> 
   <li value="3"> <p><span class="bold">Show remaining time</span> option. The total number of hours for each user (in the user line) changes. With this setting enabled, the <span>Workload Balancer</span> displays the hours that each user has available for work instead of the number of hours they are allocated for. </p> <note type="tip">
     Modifying allocations when this setting is enabled makes the total number in the user line decrease. 
    </note> </li> Project in the Select color theme section. This displays each project and its respective work items in unique colors and makes it easier to understand which items belong to which project. Percentage in the Display user allocation in section. This displays allocations as a percentage value. The user's capacity according to their schedule is considered to be 100%. For example, if a user is associated with a schedule of 8 hours per day, 8 hours equals 100% capacity. If you want to allocate the user to work 4 hours in a day, you would update his allocation to 50%. 
  </ol> </li> 
 <li value="8"> <p>Click the <span class="bold">More</span> menu <img src="assets/qs-more-menu.png"> for a work item, then click <span class="bold">Edit allocations</span>.</p> <p>Or</p> <p>Double-click the day, week, or month in the bar of a task or issue. </p> <p> <img src="assets/classic-balancer-edit-allocations-link-on-task-350x71.png" style="width: 350;height: 71;"> </p> <p>The allocation boxes become editable. </p> </li> 
 <li value="9"> <p>Click inside the box of each daily, weekly, <span>or monthly</span> allocation to manually update the amount of hours <span>or the percentage value</span> for which you want the user to be allocated each day, week, <span>or month</span> then click the <span class="bold">check mark</span> icon <img src="assets/checkmark-icon.png">. </p> <p> <img src="assets/wb-contouring-with-check-and-x-boxes-350x63.png" style="width: 350;height: 63;"> </p> <p>The allocations for the user update. </p> <note type="tip">
   If a task or issue completed before the Planned Completion Date, the number of allocated hours for the remaining days is struck through and does not count towards the user's overall allocation. This displays only when both the Show allocations icon and the Show Projected Dates setting are enabled. 
  </note> <p>The following scenarios exist:</p> 
  <ul> 
   <li>For tasks with Duration Types that are not Simple <span>or for <span>issues</span></span>, the total of the allocations must match the task Planned Hours before you can click the check mark icon. </li> 
   <li> <p>For tasks with a Simple Duration Type the total of the allocations can be higher or lower than the Planned Hours and you can click the check mark icon even if they don't match. This also updates the amount of Planned Hours for the task. You must have the correct permissions and access to update Planned Hours on tasks from the <span>Workload Balancer</span>. </p> <note type="tip">
     <span>A lock icon displays to the right of the task name as you start adjusting your allocations to indicate that the task has a Simple Duration Type.</span> 
    </note> <p> <img src="assets/lock-icon-on-simple-task-in-the-balancer-350x119.png" style="width: 350;height: 119;"> </p> </li> 
  </ul> <p> For more information about the conditions that need to be met to update Planned Hours in the <span>Workload Balancer</span>, see the following section in this article: <a href="#update" class="MCXref xref">Update task Planned Hours when managing user allocations</a>. For information about task Duration Types, see <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> </li> 
 <li value="10"> <p>(Conditional) If the task is assigned to more than one user, repeat these steps for each user assigned to the task to update the allocations for each user. </p> <p>Anyone that has access to view the <span>Workload Balancer</span> and views the same users and the same projects you managed now views the updated allocation for the users you managed. </p> </li> 
</ol>

## Update task Planned Hours when managing user allocations

You can update the Planned Hours of a task when managing user allocations in the `Workload Balancer` for the task. This happens when the total of the updated allocated hours does not match the original total of the Planned Hours for a task.

>[!IMPORTANT]
>
>* Updating Planned Hours for tasks can impact the progress on your project. 
>* `Manually updating Planned Hours by changing daily allocations can have an impact to the Planned Hours when removing assignments from the tasks in the future. For more information, see` [Planned Hours overview](../../manage-work/tasks/task-information/planned-hours.md). 
>
>* `It's not possible to update Planned Hours for issues by updating allocations in the `Workload Balancer`.` 
>

This is possible when the following conditions exist:

* You have the correct permissions and access to manage Planned Hours from the `Workload Balancer`. These include the following:

  * Manage permissions to the tasks.
  * Update Planned Hours in the `Workload Balancer` access in the Resource Management area of your Access Level.

  For more information about the access needed to use the `Workload Balancer`, see the following section in this article: [Access requirements](#access2) . 

* The task has a Duration Type of Simple.

