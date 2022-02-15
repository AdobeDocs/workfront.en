---
filename: automatically-assign-items-scheduling-areas
product-area: resource-management
navigation-topic: resource-scheduling
---



# Automatically assign unassigned tasks and issues in the Scheduling areas {#automatically-assign-unassigned-tasks-and-issues-in-the-scheduling-areas}



>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from *`Adobe Workfront`*. We recommend that you use the *`Workload Balancer`* for scheduling your resources. 
>
>
>For information about scheduling resources using the new *`Workload Balancer`*, see the section [The Workload Balancer](_workload-balancer.md).
>
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the *`Workload Balancer`*, see [Deprecation of Resource Scheduling tools in Adobe Workfront](deprecate-resource-scheduling.md).



You can allow *`Adobe Workfront`* to analyze current work assignments across your available users and propose intelligent, logical assignments for any tasks or issues that are not yet assigned. You can modify any proposed assignments prior to finalizing the assignments.


*`Workfront`* looks at the tasks and issues available in the Unassigned area within the currently selected date range and proposes assignments for each item at one time. You can create a filter to limit the number of items available in the Unassigned area.


Your system administrator determines how *`Workfront`* calculates resource availability at the system level (considering hours as well as FTE availability). Depending on this system-wide setting, resource availability is calculated either using the default schedule or the user's schedule. For more information, see [Configure how Workfront calculates resource hour and FTE availability for the Scheduling area](calculate-hours-fte-scheduling-area.md).



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View or higher access to&nbsp;Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Contribute permissions or higher to the projects, tasks, and issues you update assignments for</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

*`Workfront`* uses a proprietary algorithm to determine assignment proposals. To facilitate the best results, ensure that the following information is accurate in *`Workfront`*:



* Task and issue information, including: 
    
    
    * Role assignments   
      No proposal is made for tasks and issues that are not assigned to a role.
    * Planned Hours  
      If a task or issue currently has no planned hours, *`Workfront`* assumes 4 planned hours per workday when automatically assigning work. These hours are not automatically assigned to the work item; they are used only to ensure more realistic assignment distributions.
    
    * Planned Start Dates and Planned Completion Dates
    
    
* User information, including: 
    
    
    * Primary and secondary role assignments on the user profile
    * Project team information
    
    




## Configure role limits {#configure-role-limits}

Role limits control the number of users, with a specific role, who can be assigned work automatically. Role limits work on a per-project basis to ensure role-based tasks are not spread out among a large number of users.


The following scenarios outline how role limits apply to projects:



* `Scenario 1`: If there are no users assigned to the project team, the system uses the role limit to assign tasks.  
  For example, you have a project with no users assigned to the project team. This project has 10 project management tasks that need to be assigned, and you have set a role limit of 1 for the Project Manager role. The system assigns all 10 tasks to 1 project manager because the role limit is set to 1.

* `Scenario 2`: If the role limit is greater than the number of users assigned to the project team, additional users are assigned tasks.  
  For example, you have a project with one writer assigned to the project team. This project has 12 writer tasks that need to be assigned, and you have a role limit of 2 set for the Writer role. The system assigns all 12 tasks between the project team writer and an additional writer because the role limit is set to 2.

* `Scenario 3`: If the role limit is less than the number of users assigned to the project team, the role limit is overridden.  
  For example, you have a project with 4 designers assigned to the project team. This project has 8 designer tasks that need to be assigned, and you have set a role limit of 2 for the Designer role. The system assigns all 8 tasks between each of the 4 project team designers even though the role limit is set to 2. 



To set limits for job role assignments: 



1. Go to the scheduling timeline for multiple projects or for an individual project:
1.  `<li> <p><b>For multiple projects</b>:&nbsp; <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">   Click the    <span class="bold">Main Menu</span> icon    <img src="assets/main-menu-icon.png"> in the upper-right corner of    <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click    <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select    <span class="bold">Scheduling</span> in the upper-left drop-down menu.   </MadCap:conditionalText></p> </li>` `<li> <p><b>For an individual project</b>: <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">    Go to a project, click the    <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select    <span class="bold">Scheduling</span> from the upper-left drop-down menu.   </MadCap:conditionalText></p> </li>` 

1. Click the `Settings` icon.  
   ![Automode_settings.png](assets/automode-settings.png)


1. In the Automated Resource Scheduling section, click in the `Limit` column inline with the item in the `Role` column and enter a positive number.  
   *`Workfront`* automatically saves your changes.  


   >[!NOTE]
   >
   >All current project team members are automatically eligible for all recommended work regardless of the role limit set.


  
   ![Set_Role_Limits.png](assets/set-role-limits-350x341.png)


1. (Optional) Click the `Showing` menu at the top of the Limit column and select the desired display options.
1. To go back to the resource scheduling area, click `Return to Scheduling`.




## Automatically assign tasks and issues {#automatically-assign-tasks-and-issues}

You can assign tasks and issues to users on the scheduling timeline whether you are on the Scheduling tab (when scheduling resources for multiple projects) or the Staffing tab (when scheduling resources for an individual project).


To allow *`Workfront`* to automatically propose assignments for tasks and issues in the Unassigned area:



1.  Go to the scheduling timeline for multiple projects or for an individual project:

    
    
    *  **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    *  **For an individual project**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Go to a project, click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    

1.  (Optional) Create a filter to customize what content is displayed in the Unassigned area on the scheduling timeline.  
   For more information about creating a filter, see [Filter information in the Scheduling area](filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) in [Filter information in the Scheduling area](filter-scheduling-area.md) [Filter information in the Scheduling area](filter-scheduling-area.md)

   ` `**Tip: **`` To ensure that *`Workfront`* assigns work to the most eligible users:

    
    
    * Filter only information that affects which tasks are displayed in the Unassigned area (such as Portfolios, Programs, an Projects). 
    * We recommend that you do not filter information that affects which users are available to assign on the scheduling timeline. Doing so limits *`Workfront`* from viewing all potential assignees, which can result in less satisfactory assignments.
    
    

1. (Optional) Modify the date range that is displayed on the scheduling timeline, as described in [Adjust the date range of the Scheduling areas](get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Get started with Resource Scheduling](get-started-resource-scheduling.md). *`Workfront`* makes assignments only for tasks and issues within the visible date range on the scheduling timeline.

1.  Click the `Auto` button in the upper-right corner of the scheduling timeline.  
   ![scheduling_auto.png](assets/scheduling-auto-350x221.png)  
   *`Workfront`* proposes assignments for each task or issue in the `Unassigned` area. 


   >[!TIP] {type="tip"}
   >
   >Tasks and issues must already be assigned to a role in order for an assignment to be proposed. To ensure the best results, tasks and issues should contain the information described in [Prerequisites](#prerequisites).


   Proposed assignments are differentiated with a dotted outline around each task or issue, as follows:  
   `Proposed task assignment:`


   ` ![assignment_auto_proposed.png](assets/assignment-auto-proposed-350x116.png)

   ` 


   `Existing task assignment:` 


   ` ![assignment_auto_existing.png](assets/assignment-auto-existing-350x116.png)

   ` 

1. (Optional) You can modify any proposed or existing assignments prior to finalizing the assignments:  


   >[!NOTE]
   >
   >If you modify an existing assignment, it changes to a proposed state.


  

    
    
    * To assign an item to a different user:     
        
        
        * Drag the task or issue from the proposed user to the row of a different user you want to assign.  
          A maximum of 10 tasks per day are displayed for a given user. You can expand the list to view all tasks currently assigned to that user. (After making assignments on the scheduling timeline, more than 10 tasks might be temporarily displayed.)  
          As you drag an item, the following information is displayed prior to releasing the task or issue and completing the assignment:         
            
            
            * A drop indicator is displayed in the row of the user. This enables you to see where an item is being assigned prior to making the assignment.
            * If user allocations are enabled on the scheduling timeline, the red overallocation indicators are displayed if completing the assignment will result in the user being overallocated.  
              For more information about overallocation indicators, see [Allocation indicators](manage-allocations-scheduling-areas.md#understanding-allocation-indicators).
            
            * Users who are not eligible to receive the assignment are dimmed.
            
            
        
        * `Expand the task or issue you want to assign, click the drop-down arrow in the `Assignments` field, begin typing the name of the user you want to assign, then click the user's name in the drop-down list.  
          ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)        
        
          `
        
        
    * `To postpone making an assignment, drag any task or issue that you are not yet ready to assign back to the `Unassigned` area.`
    
    

1. Click the `Make Assignments` button at the top of the scheduling timeline to finalize any proposed assignments.  
   Or  
   Click `Cancel` to return all proposed assignments to their former positions.



