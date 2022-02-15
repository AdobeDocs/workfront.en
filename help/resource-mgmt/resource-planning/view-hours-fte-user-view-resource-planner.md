---
filename: view-hours-fte-user-view-resource-planner
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
---



# View Available, Planned, and Actual Hours or FTE in the *`Resource Planner`* when using the User view {#view-available-planned-and-actual-hours-or-fte-in-the-resource-planner-when-using-the-user-view}

In addition to budgeting resources in the Project and Role views, you can use the User View of the *`Resource Planner`* to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. 


## Overview of the User View in the *`Resource Planner`* {#overview-of-the-user-view-in-the-resource-planner}

Consider the following when viewing the Hours or FTE information in the *`Resource Planner`*: 



* You can view the Available and Planned Hours or the FTE information for users, job roles, and projects in all views of the *`Resource Planner`*.
*  You can view the following information only in the User View: 
    
    
    *  The difference between the amount of Planned Hours or FTE and the amount of Available Hours or FTE. You can then budget the allocation of your users according to this difference in the Project and Role views. 
    *  The Actual Hours or FTE. 
    
    
*  You can display the difference between the User Available and the amount of Planned Hours or FTE either as a number or as a percentage value in the User view. 
*  You cannot display the information in the User view by Cost. 
* <![CDATA[			]]> *`Adobe Workfront`* populates Available Hours or FTE according to the working time associated with the users in their schedules.  
  Users not associated with a schedule show availability according to the Default Schedule.  
  For information about the Default Schedule, see [Create a schedule](create-schedules.md).

* <![CDATA[				]]> *`Workfront`* populates Planned Hours or FTE from the Planned Hours information on the tasks and issues on the projects. 
* <![CDATA[				]]> *`Workfront`* populates Actual Hours with the actual time logged to tasks and issues by the users who are assigned to them. This includes time logged on a project. 
*  When in the User view, you can do the following: 
    
    
    *  Expand each user to display a list of projects where that user is assigned. 
    
    
      >[!NOTE]
      >
      >Only users who are associated with the projects included in the filters can be expanded. 
    
    
    
    *  Expand every project to display a list of job roles that user can fulfill on those projects. 
    *  Expand each role to display a list of tasks the user in that role is assigned to.  
    
    
  If users have no job roles associated with them, their Available, Planned, and Actual Hours or FTE are listed in the `No Role` section.  
  For information about what fields and items display when applying the User ``view to the *`Resource Planner`*, see the "Project/ Role/ User View Selection" section in [Resource Planner navigation overview](resource-planner-navigation.md).





## Overview of fields visible in the User View of the *`Resource Planner`* {#overview-of-fields-visible-in-the-user-view-of-the-resource-planner}

Refer to the following table for understanding the information displayed in the ``User view of the *`Resource Planner`*. 

<table style="width: 636.285px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 174px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 156px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 555px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Column Name<br> (Hours or FTE)</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Displayed By</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="bold">Description</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td rowspan="5" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">AVL <br>(Available Hours or FTE)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The total of Available Hours or FTE for the user according to their schedule. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This information is not available for the Project when applying the User view to the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span>. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Role</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <span class="bold">Percentage of FTE Availability </span>of the role.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Task or Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This information is not available for the Task, Issue, or Project.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td colspan="2" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td rowspan="5" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">PLN <br>(Planned Hours or FTE)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span>, the data in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><p>Note:  This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users. </p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Role</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <p>Note:  This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role. </p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task or Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The Planned Hours or FTE associated with the task or the issue on the project.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td colspan="2" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Consider the following when viewing Planned Hours:</p> 
    <ul> 
     <li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li> 
     <li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p> 
      <ul> 
       <li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <p>Tip: If tasks are assigned to teams, their allocation will appear under <span class="bold">No Role</span> and <span class="bold">No User</span> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> Planned Hours in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> do not include Planned Hours associated with the following: 
      <ul>
       <li>parent tasks</li>
       <li>unassigned tasks</li>
       <li>issues, when the <span class="bold">Include hours from Issues</span> setting is disabled.</li>
      </ul></li> 
     <li>Planned Hours do not display in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> if the task or issue Duration is zero.</li> 
     <li>Planned Hours associated with deactivated users do not display. </li> 
    </ul> <p>For more information about Planned Hours and FTE in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span>, see <a href="overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td rowspan="5" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">ACT<br>(Actual Hours or FTE) </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">User </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p> 
    <ul> 
     <li>Tasks and issues that are assigned to the user but not associated with any job role.</li> 
     <li>Tasks and issues that are not on projects for which you have access to Manage.. </li> 
    </ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p> 
    <ul> 
     <li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li> 
     <li> <p>Time logged on parent tasks. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Role</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p> 
    <ul> 
     <li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li> 
     <li>Time logged directly on the project or parent tasks. </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Task or Issue </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td colspan="2" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> <p>Important:  The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.</p> </p> <p>For more information about Actual Hours, see <a href="actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td rowspan="4" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">DIF <br>(Hour or FTE Difference) <br><br></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Note:  If the value displays in negative red numbers, the user is overallocated. </p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This information is not available for the Project. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Role</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Note:  If the value is displayed in negative red numbers, the role is overallocated. </p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task or Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This information is not available for the Task, Issue, or Project. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td rowspan="5" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planned Hours or FTE Allocation Percentage (%)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This information is not available for the Project when applying the <span class="bold">View by User</span> view to the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Role</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task or Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This information is not available for the Task, Issue, or Project. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td colspan="2" class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span>, see <a href="budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and&nbsp;Role views</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

