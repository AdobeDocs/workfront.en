---
filename: view-hours-fte-user-view-resource-planner
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view
description: In addition to budgeting resources in the Project and Role views, you can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources.
---

# View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view

In addition to budgeting resources in the Project and Role views, you can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources.

## Overview of the User View in the Resource Planner

Consider the following when viewing the Hours or FTE information in the Resource Planner:

<ul> 
 <li>You can view the Available and Planned Hours or the FTE information for users, job roles, and projects in all views of the Resource Planner.</li> 
 <li> You can view the following information only in the User View: 
  <ul>
   <li> The difference between the amount of Planned Hours or FTE and the amount of Available Hours or FTE. You can then budget the allocation of your users according to this difference in the Project and Role views. </li>
   <li> The Actual Hours or FTE. </li>
  </ul></li> 
 <li> You can display the difference between the User Available and the amount of Planned Hours or FTE either as a number or as a percentage value in the User view. </li> 
 <li> You cannot display the information in the User view by Cost. </li> 
 <li><![CDATA[
			]]>Adobe Workfront populates Available Hours or FTE according to the working time associated with the users in their schedules.<br>Users not associated with a schedule show availability according to the Default Schedule.<br>For information about the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li> 
 <li><![CDATA[
				]]>Workfront populates Planned Hours or FTE from the Planned Hours information on the tasks and issues on the projects. </li> 
 <li><![CDATA[
				]]>Workfront populates Actual Hours with the actual time logged to tasks and issues by the users who are assigned to them. This includes time logged on a project. </li> 
 <li> When in the User view, you can do the following: 
  <ul>
   <li><p> Expand each user to display a list of projects where that user is assigned. </p><note type="note">
     Only users who are associated with the projects included in the filters can be expanded. 
    </note></li>
   <li> Expand every project to display a list of job roles that user can fulfill on those projects. </li>
   <li> Expand each role to display a list of tasks the user in that role is assigned to.<br></li>
  </ul> If users have no job roles associated with them, their Available, Planned, and Actual Hours or FTE are listed in the <span class="bold">No Role</span> section.<br>For information about what fields and items display when applying the User view to the Resource Planner, see the "Project/ Role/ User View Selection" section in <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>.</li> 
</ul>

## Overview of fields visible in the User View of the Resource Planner

Refer to the following table for understanding the information displayed in the User view of the Resource Planner. 

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Column Name<br> (Hours or FTE)</span> </td> 
   <td><span class="bold">Displayed By</span> </td> 
   <td> <p><span class="bold">Description</span> </p> </td> 
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
   <td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <span class="bold">Percentage of FTE Availability</span> of the role.</p> </td> 
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
  <tr> 
   <td colspan="2"> <p>Consider the following when viewing Planned Hours:</p> 
    <ul> 
     <li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li> 
     <li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p> 
      <ul> 
       <li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <p>Tip: If tasks are assigned to teams, their allocation will appear under <span class="bold">No Role</span> and <span class="bold">No User</span> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following: 
      <ul>
       <li>parent tasks</li>
       <li>unassigned tasks</li>
       <li>issues, when the <span class="bold">Include hours from Issues</span> setting is disabled.</li>
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
   <td colspan="2"> <p> <p>Important:  The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.</p> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td> 
  </tr> 
  <tr> 
   <td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td> 
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
  <tr> 
   <td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td> 
   <td>User</td> 
   <td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>This information is not available for the Project when applying the <span class="bold">View by User</span> view to the Resource Planner.</td> 
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

