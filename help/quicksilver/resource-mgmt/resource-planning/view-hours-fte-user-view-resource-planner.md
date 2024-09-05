---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: View Available, Planned, and Actual Hours or FTE in the Resource Planner when Using the User View
description: View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User viewPlanning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)"
author: LIsa
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
---
# View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

In addition to budgeting resources in the Project and Role views, you can use the User View of the Adobe Workfront Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources.

## Overview of the User View in the Resource Planner

Consider the following when viewing the Hours or FTE information in the Resource Planner:

* You can view the Available and Planned Hours or the FTE information for users, job roles, and projects in all views of the Resource Planner.
* You can view the following information only in the User View:

   * The difference between the amount of Planned Hours or FTE and the amount of Available Hours or FTE. You can then budget the allocation of your users according to this difference in the Project and Role views. 
   * The Actual Hours or FTE.

* You can display the difference between the User Available and the amount of Planned Hours or FTE either as a number or as a percentage value in the User view. 
* You cannot display the information in the User view by Cost. 
* Adobe Workfront populates Available Hours or FTE according to the working time associated with the users in their schedules.  
  Users not associated with a schedule show availability according to the Default Schedule.  
  For information about the Default Schedule, see [Create a schedule](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront populates Planned Hours or FTE from the Planned Hours information on the tasks and issues on the projects. 
* Workfront populates Actual Hours with the actual time logged to tasks and issues by the users who are assigned to them. This includes time logged on a project. 
* When in the User view, you can do the following:

   * Expand each user to display a list of projects where that user is assigned.

     >[!NOTE]
     >
     >Only users who are associated with the projects included in the filters can be expanded.

   * Expand every project to display a list of job roles that user can fulfill on those projects. 
   * Expand each role to display a list of tasks the user in that role is assigned to.

  If users have no job roles associated with them, their Available, Planned, and Actual Hours or FTE are listed in the **No Role** section.  
  For information about what fields and items display when applying the User view to the Resource Planner, see the "Project/ Role/ User View Selection" section in [Resource Planner navigation overview](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Overview of fields visible in the User View of the Resource Planner

Refer to the following tables for understanding the information displayed in the User view of the Resource Planner. The information displays in Hours or FTE values.

* [The AVL (Available) column](#the-avl-available-column) 
* [The PLN (Planned) column](#the-pln-planned-column) 
* [The ACT (Actual) column](#The%C2%A0ACT) 
* [The DIF (Difference) column](#the-dif-difference-column) 
* [The % (Planned Hours Allocation Percentage) column](#the-planned-hours-allocation-percentage-column)

### The AVL&nbsp;(Available) column {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Displayed By</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td>The total of Available Hours or FTE for the user according to their schedule. </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>This information is not available for the Project when applying the User view to the Resource Planner. </td> 
  </tr> 
  <tr> 
   <td>Role</td> 
   <td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td> 
  </tr> 
  <tr> 
   <td>Task or Issue</td> 
   <td>This information is not available for the Task or Issue. </td> 
  </tr> 
 </tbody> 
</table>

For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see [Overview of calculating hours and FTE for users and roles in the Resource Planner](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### The PLN (Planned) column {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Displayed By</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><p>Note:  This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users. </p></td> 
  </tr> 
  <tr> 
   <td>Role</td> 
   <td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <p>Note:  This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Task or Issue</td> 
   <td>The Planned Hours or FTE associated with the task or the issue on the project.</td> 
  </tr> 
 </tbody> 
</table>

Consider the following when viewing Planned Hours:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.  
  Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.

  If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.  
  Weekend days, schedule exceptions, and time-off days are excluded from this distribution.

* The following categories of tasks are included in calculating the Planned Hours for each resource:

   * tasks assigned to users in Resource Pools, job roles, or teams on the project.

     >[!TIP]
     >
     >If tasks are assigned to teams, their allocation will appear under **No Role** and **No User** sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.

* Planned Hours in the Resource Planner do not include Planned Hours associated with the following:

   * parent tasks
   * unassigned tasks
   * issues, when the **Include hours from Issues** setting is disabled.

* Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.
* Planned Hours associated with deactivated users do not display.

For more information about Planned Hours and FTE in the Resource Planner, see [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### The&nbsp;ACT (Actual)&nbsp;column

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Displayed By</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>User </td> 
   <td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p> 
    <ul> 
     <li>Tasks and issues that are assigned to the user but not associated with any job role.</li> 
     <li>Tasks and issues that are not on projects for which you have access to Manage. </li> 
    </ul> <p>This includes the time logged on the project only when the user is assigned to tasks or issues on that project.  </p> </td> 
  </tr> 
  <tr> 
   <td>Project </td> 
   <td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p> 
    <ul> 
     <li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li> 
     <li> <p>Time logged on parent tasks. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Role</td> 
   <td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p> 
    <ul> 
     <li>Time logged on tasks and issues assigned to this role but not to this user in this role.</li> 
     <li>Time logged directly on the project or parent tasks. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Task or Issue </td> 
   <td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>The time logged displays in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.

For more information about Actual Hours, see [View Actual Hours](../../manage-work/tasks/task-information/actual-hours.md).

### The DIF (Difference) column {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Displayed By</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Note:  If the value displays in negative red numbers, the user is overallocated. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>This information is not available for the Project. </td> 
  </tr> 
  <tr> 
   <td>Role</td> 
   <td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Note:  If the value is displayed in negative red numbers, the role is overallocated. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Task or Issue</td> 
   <td>This information is not available for the Task, Issue, or Project. </td> 
  </tr> 
 </tbody> 
</table>

### The % (Planned Hours Allocation Percentage) column {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Displayed By</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td> 
  </tr> 
  <tr> 
   <td>Role</td> 
   <td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td> 
  </tr> 
  <tr> 
   <td>Task or Issue</td> 
   <td>This information is not available for the Task, Issue, or Project. </td> 
  </tr> 
 </tbody> 
</table>

If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated.

For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see [Budget resources in the Resource Planner using the Project and Role views](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
