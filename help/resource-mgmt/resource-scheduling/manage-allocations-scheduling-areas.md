---
filename: manage-allocations-scheduling-areas
product-area: resource-management
navigation-topic: resource-scheduling
title: Manage user allocations in the Scheduling areas
description: We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources.
---

# Manage user allocations in the Scheduling areas

>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from `Adobe Workfront`. We recommend that you use the `Workload Balancer` for scheduling your resources. 
>
>For information about scheduling resources using the new `Workload Balancer`, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the `Workload Balancer`, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

User allocations are amounts of hours that indicate the time that a user should spend on one given day to complete a work item. They are included in the Planned Hours of the work item.

This article describes how to update daily hourly allocations for users assigned to tasks or issues. For information about managing overall allocations for users and job roles to tasks, see [Manage allocation hours on tasks](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md). You cannot update overall allocations for users and job roles for issues.

You can display user allocations in the following areas of `Adobe Workfront`:

* On the Scheduling section of the Resourcing area. 
* On the Scheduling section of a project (when scheduling resources for a single project). 
* On the Schedule section of a team (when scheduling resources for a team).

## Access requirements

You must have the following:

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
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to Projects, Tasks,&nbsp;and Issues</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to projects, tasks, and issues</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## User allocations in the Scheduling areas

Before you begin allocating time to users as described in this article, become familiar with how resource scheduling works in `Workfront`, as described in [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

You can schedule resources to work on tasks and issues for an individual team you are a member of, for an individual project where you are a member of the project team, or for multiple projects for which you are the resource manager.

The following sections describe how to enable and manage user allocations in `Workfront`:

* [Use the Scheduling areas to assign work](#using-scheduling-timelines-to-assign-work) 
* [Allocations set on the Edit Task or the Edit Issue boxes vs. in the Scheduling areas](#understanding-allocations-set-on-the-task-or-issue-details-versus-on-the-scheduling-timeline) 
* [Allocation indicators](#understanding-allocation-indicators) 
* [Default allocation for Planned Hours](#understanding-the-default-allocation-for-planned-hours) 
* [Who can view and modify allocations?](#understanding-who-can-view-and-modify-allocations) 
* [Time zone considerations in the Scheduling areas](#time-zone-considerations-on-the-scheduling-timeline)

### Use the Scheduling areas to assign work

When assigning new work to users on the Scheduling timeline, you can determine how the Planned Hours for a task or issue are allocated to users.   
For more information about Planned Hours, see [Planned Hours overview](../../manage-work/tasks/task-information/planned-hours.md).

Planned Hours can be divided in the following ways:

* Among users who are assigned to the task or issue
* Across the duration of the task or issue  
  For example, a sales-related task might require more work toward the end of the task duration. You can plan this uneven distribution of hours into your task.

>[!TIP]
>
>When scheduling resources for multiple projects from the Scheduling areas, not all users and work items are displayed on the Scheduling timeline. For information about what information is displayed on the Scheduling timeline, see [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

### Allocations set on the Edit Task or the Edit Issue boxes vs. in the Scheduling areas

You can modify the user allocations for a task or issue from the following locations within `Workfront`:

<ul> 
 <li>The Scheduling timeline<br>The Scheduling timeline is located in the following areas: 
  <ul>
   <li>On the Scheduling section of the Resourcing area.</li>
   <li>On the Scheduling section of a project (when scheduling resources for a single project).</li>
   <li>On the Schedule section of a team (when scheduling resources for a team).</li>
  </ul>When you modify user allocations from the Scheduling timeline (as described in the <a href="#modifying-user-allocations" class="MCXref xref">Modify user allocations</a> section in this article), you can define allocations for each user on the task or issue, as well as for each day within the task or issue duration.<br><img src="assets/scheduling-contours-350x139.png" alt="scheduling_contours.png" style="width: 350;height: 139;"></li> 
 <li>The Edit Task or Edit Issue dialog box. <br>When you modify user allocations from a Edit Task or Issue dialog box (as described in <a href="../../manage-work/tasks/assign-tasks/manage-allocation-percentage-on-tasks.md" class="MCXref xref">Manage allocation percentage on tasks</a>), you can define allocations for the task or issue only as a whole for each user. If you want to manage those allocations on a per-day basis, you must modify the allocations in the Scheduling timeline, as described in the <a href="#modifying-user-allocations" class="MCXref xref">Modify user allocations</a> section in this article.<br><note type="important">
    When modifying user allocations from an Edit Task or Issue dialog box, allocations you previously configured in the Scheduling timeline are overwritten. In addition, any change you make to allocations in the Scheduling timeline are not reflected on an Edit Task or Issue dialog box.
  </note><br></li> 
</ul>

We recommend managing user allocations from the Scheduling timeline rather than from the Edit Task or Issue to benefit from the following advantages:

* You can clearly see when users are overallocated using allocation indicators, as described in the [Allocation indicators](#understanding-allocation-indicators) section.
* You can allocate more time for one user over another user.  
  Allocation indicators provide a visual representation of how allocated a user is compared to other users, as described in the [Allocation indicators](#understanding-allocation-indicators) section. 

* You can allocate more time for work on one day over another day.  
  Allocation indicators provide a visual representation of how allocated users are on a given day, as described in [Allocation indicators](#understanding-allocation-indicators).

* You can perform all resourcing responsibilities in one place, on the Scheduling timeline.

### Allocation indicators

Various visual indicators are available to provide quick information regarding the level of which a user is allocated to work on a given day.

Your system administrator determines how `Workfront` calculates user availability at the system level (considering hours as well as FTE availability). Depending on this system-wide setting, user availability is calculated either using the default schedule or the user's schedule. For more information, see [Configure how Workfront calculates resource hour and FTE availability for the Scheduling area](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

<ul> 
 <li><span class="bold">Allocation shading</span> <br>Allocation is visually displayed on tasks assigned to users in the form of shading. Darker shading indicates the allocated hours as a percentage of the assigned users' FTE (Full Time Equivalent) on a given day. (For more information about how to configure FTE in <span>Workfront</span>, see <a href="../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md" class="MCXref xref">Configure how Workfront calculates resource hour and FTE&nbsp;availability for the Scheduling area</a>.) <br>For example, a single user is assigned to a task that has an amount of 4 Planned Hours and a Duration of 1 day. The FTE for the user is defined in the system as 1 (meaning that the user is scheduled to work at full-time status, or rather 40 hours a week, or 8 hours a day). The shading for the task on a given day occupies half of the vertical space of the task, this indicates that the user is allocated half of his or her FTE (4 hours) on that day.<br><img src="assets/scheduling-shading-allocation.png" alt=""><br>The task or issue displays the cumulative allocation across all users assigned to the work item. You can expand a work item to view more details, including who is assigned to the work item and how many hours each user is assigned.<br>Shading is not displayed on tasks in the <span class="bold">Unassigned</span> area on the Scheduling timeline.<br><img src="assets/resource-allocation-expanded-350x192.png" alt="resource_allocation_expanded.png" style="width: 350;height: 192;"></li> 
 <li><span class="bold">Daily totals for each day for each user:</span> You can display the total Planned Hours allocated to a given user on each day. This information is displayed at the top of each user's row on the Scheduling timeline. This information is not displayed by default. You can enable this as described in <a href="#enabling-user-allocations" class="MCXref xref">Enable user allocations</a>. Tasks from projects with any of the following statuses are included when determining daily totals: Current, Planning, or Approved.<br><img src="assets/resource-daily-totals-350x55.png" alt="resource_daily_totals.png" style="width: 350;height: 55;"></li> 
 <li><span class="bold">Overallocation indicators</span> <br>When the total number of Planned Hours assigned to a user on a given day exceeds the number of hours the user works in a day (across all tasks), that user is considered overallocated on that day. <br>When a user is overallocated, a red bar is displayed, outlining each task on the day. <br>Tasks from projects with any of the following statuses are included when determining a user's overallocation: Current, Planning, or Approved.<br>The number of hours a user works in a day is defined via the FTE field in the each user's profile, as described in see <a href="../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md" class="MCXref xref">Configure how Workfront calculates resource hour and FTE&nbsp;availability for the Scheduling area</a>.<br><img style="font-size: small;width: 350;height: 72;" src="assets/resource-over-allocation-350x72.png" alt="resource_over_allocation.png"><br>When you enable the <span class="bold">Show Totals for Daily Planned Hours</span> and the <span class="bold">Show Resource Allocation Highlighting</span> options in your settings, the daily total number of Planned Hours displays in red when the user is overallocated. Hours are displayed to the nearest tenth by default (for example, 1.3).<br><img src="assets/rs-planned-hours-in-red-with-decimals--1--350x56.png" alt="RS_planned_hours_in_red_with_decimals__1_.png" style="width: 350;height: 56;"></li> 
</ul>

### Default allocation for Planned Hours

`Workfront` attempts to distribute Planned Hours among the assigned users and days as follows:

* When multiple users are assigned to a task or issue, hours are divided evenly among the users.  
  The distribution reflects any advanced assignments that have already been made on the task.   
  For more information about advanced assignments, see [Create advanced assignments](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

* When the Duration of the task or issue spans multiple days, the Planned Hours are distributed equally among the days, and among all users assigned to the task, based on the user's schedule.
* When the Planned Hours of a task span multiple days, a user viewing the task from a different time zone might see a difference in the task duration or the Planned Start Date or Planned Completion Date.

Hours are displayed to the nearest hundredth by default (for example, 1.33). You can scroll to the right to see more.   
![RS_Planned_Hours_with_two_decimals_in_contour_screen__1___1_.png](assets/rs-planned-hours-with-two-decimals-in-contour-screen--1---1--350x252.png)

### Who can view and modify allocations?

The following types of users can view or modify user allocations in `Workfront`:

* `Resource Managers:` You can view and modify user allocations for tasks and issues on any projects for which you are the Resource Manager. You can do this either in the Scheduling timeline in the People area, or in the Staffing tab of a project.  
  For information about how Resource Managers can make changes to tasks and issues across projects, see [Manually assign unassigned tasks and issues in the Scheduling areas](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md). 

* `Plan and Work Users:` You can view allocations for any tasks and issues you are assigned to by using either the new My Work Calendar or the Working On calendar on a team that you are a member of.   
  In addition to viewing allocations, you can modify your allocations if you have Contribute access to the tasks and issues.

### Time zone considerations in the Scheduling areas

In rare cases, users viewing the Scheduling timeline might see inconsistencies where the Planned Hours of a task do not equal the total allocated hours of individual days. This can occur when the operating system time zone setting of one user is such that the Planned Start Date or Planned Completion Date differs from another user.

For example, if the Planned Completion Date of a task is set to 11:00am on 11/3/18, MST, a user in Australia who views the task would see the Planned Completion Date as 1:00am on 11/4/18, the following day. If the user in Australia allocates hours on 11/4/18, these allocated hours are not visible to the user on MST. However, these hours are always taken into consideration on the Planned Hours of the project.

## Enable user allocations

User allocation functionality is disabled by default on the Scheduling timeline. Before you can use the user allocation functionality described in this section, you must first enable it.

>[!NOTE]
>
>User allocations can be enabled only when the Scheduling timeline is configured to use Planned Dates. If the Scheduling timeline is configured to use Projected Dates, user allocations cannot be displayed. For more information about configuring the Scheduling timeline to use Planned or Projected Dates, see "Configuring Projected Dates to Display on the Scheduling Timeline" in [Configure settings in the Scheduling areas](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md).

To enable user allocations on the Scheduling timeline:

<ol> 
 <li value="1">Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
  <ul>
   <li><p><b>For multiple projects</b>:&nbsp; Click the Main Menu icon in the upper-right corner of Workfront, click Resourcing > Workload Balancer, then select Scheduling in the upper-left drop-down menu.</p></li>
   <li><p><b>For an individual project</b>: Go to a project, click the Workload Balancer section in the left panel, then select Scheduling from the upper-left drop-down menu.</p></li>
   <li><p><b>For a team</b>: Click the Main Menu icon in the upper-right corner of Workfront, then click Teams, select a team, click Workload Balancer in the left panel, then select Scheduling from the upper-left drop-down menu.</p></li>
  </ul><p></p></li> 
 <li value="2">Click the <span class="bold">Settings</span> icon on the Scheduling timeline.<br><img src="assets/scheduling-settings-icon-350x169.png" alt="scheduling_settings_icon.png" style="width: 350;height: 169;"><br>The Resource Scheduling Settings dialog box is displayed.<br><img src="assets/rs-scheduling-tab-all-settings--4--350x348.png" alt="RS_scheduling_tab_all_settings__4_.png" style="width: 350;height: 348;"></li> 
 <li value="3"> <p>Enable one or both of the following options to show user allocations on the Scheduling timeline:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Show Resource Allocation Highlighting</td> 
     <td> <p>Display user allocation shading on tasks and issues on the Scheduling timeline. </p> <p>This option is disabled by default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Show Totals for Daily Planned Hours</td> 
     <td>Displays the total number of Planned Hours that are allocated to each user for each day on the Scheduling timeline. The Planned Hours display to the nearest tenth (for example, 1.3).<br>This option is disabled by default.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">(Optional) In the <span class="bold">Include Issues</span> section, select whether you want issues to be displayed on the Scheduling timeline.<br>This option is disabled by default.</li> 
 <li value="5">Click <span class="bold">Return to Scheduling</span>.<br>User allocations are now displayed on the Scheduling timeline.<br><img src="assets/rs-daily-planned-totals-and-allocation-highlighting--1--350x123.png" alt="RS_daily_planned_totals_and_allocation_highlighting__1_.png" style="width: 350;height: 123;"></li> 
</ol>

## Modify user allocations

You can modify the user allocations for a task or issue from the Scheduling timeline (as described in this section) or from the Edit Task or Issue dialog box. For more information, see [Allocations set on the Edit Task or the Edit Issue boxes vs. in the Scheduling areas](#understanding-allocations-set-on-the-task-or-issue-details-versus-on-the-scheduling-timeline).

By default, users are allocated to a task or issue evenly among assignees and among days in the duration, as described in [Default allocation for Planned Hours](#understanding-the-default-allocation-for-planned-hours).

To modify user allocations for a task or issue from the Scheduling timeline:

<ol> 
 <li value="1">Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
  <ul>
   <li><p><b>For multiple projects</b>:&nbsp; Click the Main Menu icon in the upper-right corner of Workfront, click Resourcing > Workload Balancer, then select Scheduling in the upper-left drop-down menu.</p></li>
   <li><p><b>For an individual project</b>: Go to a project, click the Workload Balancer section in the left panel, then select Scheduling from the upper-left drop-down menu.</p></li>
   <li><p><b>For a team</b>: Click the Main Menu icon in the upper-right corner of Workfront, then click Teams, select a team, click Workload Balancer in the left panel, then select Scheduling from the upper-left drop-down menu.</p></li>
  </ul><p><img src="assets/scheduling-contours-350x139.png" alt="scheduling_contours.png" style="width: 350;height: 139;"></p></li> 
 <li value="2">Ensure that user allocations are enabled on the Scheduling timeline, as described in the <a href="#enabling-user-allocations" class="MCXref xref">Enable user allocations</a> section in this article.</li> 
 <li value="3">Expand the task where you want to manage user allocations.<br>By default, Planned Hours are divided evenly among the assigned users and days of the task Duration. Hours are not added on weekends (Saturdays and Sundays). For more information, see the <a href="#understanding-the-default-allocation-for-planned-hours" class="MCXref xref">Default allocation for Planned Hours</a> section in this article.</li> 
 <li value="4">Click the field for the user whose hours you want to adjust on a given day.<br><note type="note">
    To maintain the original distribution after modifying hours, click 
   <span class="bold">Cancel</span>.
  </note></li> 
 <li value="5">Specify the adjusted number of hours.</li> 
 <li value="6">Click <span class="bold">Save</span>.<br>You can save your changes only when the total number of hours for the task is equal to the number of original Planned Hours. This number is shown in the <span class="bold">Planned Hours</span> field on the task. The number is displayed in red when the total is not equal to the total number of Planned Hours.<br><img src="assets/resource-allocation-expanded-modified-350x226.png" alt="resource_allocation_expanded_modified.png" style="width: 350;height: 226;"></li> 
</ol>

## Criteria that reset user allocations

`Workfront` resets the user allocations that you manually edit in the Scheduling timeline when a number of actions occur on the tasks or the project. Generally, `Workfront` resets user allocations any time the timeline of the project is recalculated if the number of Planned Hours on the tasks and issues has changed in this process.  
For more information about recalculating the timeline of projects, see [Recalculate project timelines](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Some of the most common criteria that could reset user allocations in the Scheduling timeline are:

* Adding a task to an Iteration.  
  Because iterations have fixed dates, the dates of the tasks and the allocations are recalculated.  
  For information about how Iterations can affect task dates, see [Add stories to an existing iteration](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

* Changing the Duration Type of a task to Effort Driven. 
* Changing the Duration Type of a task to Calculated Assignment when more than 1 person is assigned.   
  For information about Task Duration, see [Overview of Task Duration and Duration Type](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Changing the project Planned Start and Planned Completion Dates.  
  For information about project planned dates, see [Overview of the project Planned Start Date](../../manage-work/projects/planning-a-project/project-planned-start-date.md) and [Set the project Planned Completion Date](../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

  For information about the task Planned Completion Date, see [Overview of the task Planned Completion Date](../../manage-work/tasks/task-information/task-planned-completion-date.md).

* Changing the dates of a predecessor task if the Task Constraint is a flexible constraint.  
  For example, As Soon as Possible or As Late as Possible.  
  For information about Task Constraint, see [Task Constraint overview](../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Changing the amount of Planned Hours of tasks or issues.

  For information about Planned Hours in `Workfront`, see [Planned Hours overview](../../manage-work/tasks/task-information/planned-hours.md).

