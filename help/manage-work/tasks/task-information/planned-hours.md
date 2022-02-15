---
filename: planned-hours
content-type: overview
product-area: projects
navigation-topic: task-information
---



# Planned Hours overview {#planned-hours-overview}

The Planned Hours associated with a task, issue, or project represent the amount of time required for the assigned users to complete the task, issue, or project.


You must define the value of Planned Hours for tasks and issues if you want to use the Resource Management tools in *`Adobe Workfront`*. 


You can modify the value of Planned Hours on tasks, depending on the Duration Type of the tasks. For more information about modifying Planned Hours on tasks in relation to the Duration Type of the tasks, see [Update task Planned Hours based on Duration Type](#planned-hours-and-duration-type).


You can modify the value of Planned Hours on issues at any time. 


You cannot modify the value of Planned Hours of projects, as they are a calculated sum of all Planned Hours of all the tasks on the project. 


## Update task Planned Hours based on Duration Type {#update-task-planned-hours-based-on-duration-type}

You can only update Planned Hours on tasks if the tasks have a certain Duration Type. The following scenarios exist: 



*  You can modify Planned Hours for tasks only when using the Calculated Assignment or Simple Duration Types.


  For more information about the Calculated Assignment Duration Type, see [Duration Type overview: Calculated Assignment](calculated-assignment.md).


  For more information about the Simple Duration Type, see [Duration Type overview: Simple](simple-duration-type.md).

* You can update task Planned Hours only for Simple Duration Type tasks in the *`Workload Balancer`* when you manage users' allocations to tasks. For information about managing user allocations in the *`Workload Balancer`*, see [Manage user allocations in the Workload Balancer](manage-user-allocations-workload-balancer.md).

*  You cannot modify Planned Hours for tasks with a Duration Type of Effort Driven or Calculated Work. In these cases, *`Workfront`* determines Planned Hours based on the value input in the Duration field; however, in this case the Planned Hours are always equal to the Duration (in hours) and they are not impacted by the percent allocation of the assigned resources. 


  For more information about the Effort Driven Duration Type, see [Duration Type overview: Effort Driven](effort-driven.md).


  For more information about the Calculated Work Duration Type, see [Duration Type overview: Calculated Work](calculated-work.md).






## Update task Planned Hours automatically using *`Work Effort`*  {#update-task-planned-hours-automatically-using-work-effort}

When you use *`Work Effort`* to estimate the effort needed for a task to complete, the amount of Planned Hours for the tasks updates automatically. This is possible only for tasks with a Simple Duration&nbsp;Type. 


For information about using *`Work Effort`* to estimate task effort, see [Work Effort overview](work-effort.md). 


## Distribution of Planned Hours across the Duration of a task {#distribution-of-planned-hours-across-the-duration-of-a-task}

By default, *`Workfront`* distributes the Planned Hours evenly across the Duration of a task, allocating an equal number of Planned Hours for each day of the task, according to the availability of the project schedule. 


For example, if a task is set to start at 4 PM and the schedule has one hour left in the first day of the task, *`Workfront`* puts one Planned Hour in the first day of the task Duration, then divides the remainder of the Planned Hours equally between the rest of the days in the task Duration. 


>[!NOTE]
>
>The Planned Hours per Day is the allocation of Planned Hours for each day during the Duration of the task. If the task has one assignment, then this number represents the Planned Hours per Day per assignment, as well. If the task has multiple assignments, the Planned Hours per Day per assignment is different than the Planned Hours per Day for the task. There is no visual representation in *`Workfront`* for the Planned Hours per Day per assignment, for tasks with multiple assignments.





## Planned Hours on tasks vs. Planned Hours on projects {#planned-hours-on-tasks-vs-planned-hours-on-projects}




* [Planned Hours on tasks](#planned-hours-on-tasks) 
* [Planned Hours on projects](#planned-hours-on-projects) 




### Planned Hours on tasks {#planned-hours-on-tasks}

When a task contains subtasks, the Planned Hours of the parent task is the sum of all Planned Hours on any subtasks. You cannot update the Planned Hours of a parent task.


>[!NOTE]
>
>Unlike Planned Hours, Actual Hours on a parent task are hours logged directly on the parent task. They do not represent a sum of the Actual Hours of the children tasks.   
>For more information about Actual Hours, see [View Actual Hours](actual-hours.md).




### Planned Hours on projects {#planned-hours-on-projects}

You cannot edit the amount of Planned Hours on a project. Planned Hours on a project are a calculated sum of all Planned Hours from all the tasks on the project.


Whether issues are included in the calculation for Planned Hours depends on the location within the project where you are viewing Planned Hours. You can view Planned Hours in the following locations within a project:



* `Project Details` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">section</span> </MadCap:conditionalText>` `:` Only the Planned Hours for the tasks on the project are taken into account. The Planned Hours for the issues on the project are not taken into account when viewing the total number of Planned Hours for the project in the Project Details `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`. 

* `Utilization `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">section</span></MadCap:conditionalText>`:` The Planned Hours for tasks and the issues on the project are taken into account when viewing the total number of Planned Hours for the project in the Utilization `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`.

* **Role Allocation panel** in the task list : The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see [View project Planned Hours in the Role Allocation panel](view-planed-hours-in-role-allocation-panel.md). 





## Locate Planned Hours  {#locate-planned-hours}

You can find the Planned Hours information on tasks, issues, or projects in the following locations:



*  [Planned Hours in the Details section](#planned2) 
* [Planned Hours when editing a task or issue](#plan-hours-on-edit-task-or-issue) 
* [Planned Hours in reports](#reports) 
* [Planned Hours in Resource Management tools](#resource-grid) 





### Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View or higher access to Tasks, Projects, or Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


### Planned Hours in the Details section {#planned-hours-in-the-details-section}

Finding the Planned Hours in the Details `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`is identical for tasks, issues, and projects. 


To locate the Planned Hours value on the Details `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>` of a task: 



1. Go to a task for which you want to review the Planned Hours.
1.  Click `Task Details` in the left panel. 
1.  Click the `Overview` area and notice the Planned Hours value.


   This value represents the time it would take the user assigned to the task to complete it. 





### Planned Hours when editing a task or issue {#planned-hours-when-editing-a-task-or-issue}

Finding the Planned Hours while editing a task or an issue is identical. 


>[!TIP] {type="tip"}
>
>You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project. 


To locate the value of Planned Hours while editing a task:



1. Go to the task or issue you want to view Planned Hours for.
1.  Click the `More` icon ![](assets/qs-more-icon-on-an-object.png) next to the task name, then click `Edit`.


   The Planned Hours are located in the `Overview` section. ``





### Planned Hours in reports {#planned-hours-in-reports}

The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. 


Adding the Planned Hours column to a project view is similar to building a view in a project report. 


To show Planned Hours in a project report:



1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Reports`. 
1. Click `New Report`, then choose `Project` as your object.

1. Click `Add Column`, and start typing `Planned Hours` when the `Show in this column` drop-down field is displayed. Select the field when it appears in the list.

1.  Click `Save + Close` to save the report. 


   The Planned Hours column shows the total number of Planned Hours on each project. 





### Planned Hours in Resource Management tools {#planned-hours-in-resource-management-tools}

You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:



*  Resource Planner.


  For information about using the Resource Planner, see [Resource Planner overview](get-started-resource-planner.md).

*  Utilization Report.


  For information about the utilization report, see [Overview of the Resource Utilization report](resource-utilization-report.md).

*  
  The following sections:

    
    
    * Scheduling or *`Workload Balancer`* sections in the Resourcing area
    * Scheduling section at the project level
    * Schedule section at the team level
    
    
  For information about scheduling resources, see [Get started with Resource Scheduling](get-started-resource-scheduling.md).


  For information about the Workload Balancer, see [Overview of the Workload Balancer](overview-workload-balancer.md). 

*  **Role Allocation panel** in the project `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> task list or</MadCap:conditionalText>` *`Workload Balancer`*: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see [View project Planned Hours in the Role Allocation panel](view-planed-hours-in-role-allocation-panel.md). 


