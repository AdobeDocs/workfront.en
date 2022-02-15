---
filename: configure-settings-scheduling-areas
product-area: resource-management;setup
navigation-topic: resource-scheduling
---



# Configure settings in the Scheduling areas {#configure-settings-in-the-scheduling-areas}



>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from *`Adobe Workfront`*. We recommend that you use the *`Workload Balancer`* for scheduling your resources. 
>
>
>For information about scheduling resources using the new *`Workload Balancer`*, see the section [The Workload Balancer](_workload-balancer.md).
>
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the *`Workload Balancer`*, see [Deprecation of Resource Scheduling tools in Adobe Workfront](deprecate-resource-scheduling.md).



You can configure various settings to customize how and what information displays in the scheduling timeline. 



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article::

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View access or higher to Projects, Tasks,&nbsp;and Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Contribute permissions or higher to projects, tasks, and issues</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Configure issues to display on the scheduling timeline {#configure-issues-to-display-on-the-scheduling-timeline}

You can configure issues to be displayed in addition to tasks on the scheduling timeline.   
When scheduling resources `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> in the Scheduling section for a team</MadCap:conditionalText>`, issues are displayed by default in addition to tasks. When scheduling resources for projects, only tasks are displayed by default.



1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
    
    
    * **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For an individual project**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Go to a project, click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For a team**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Teams</span>, select a team, click <span class="bold"> <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span> in the left panel, then select <span class="bold"> Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    
1. Click the `Settings` icon on the scheduling timeline.  

1. On the Resource Scheduling Settings dialog box, enable the  `Show Issues`&nbsp;option.  
   ![RS_scheduling_tab_all_settings__1_.png](assets/rs-scheduling-tab-all-settings--1--350x417.png)


1. Click `Return to Scheduling`.&nbsp;




## Configure completed work to display on the scheduling timeline {#configure-completed-work-to-display-on-the-scheduling-timeline}

You can configure the scheduling timeline to display work that has already been marked as Complete. By default, completed work is not displayed on the scheduling timeline.&nbsp;



1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
    
    
    * **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For an individual project**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Go to a project, click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For a team**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Teams</span>, select a team, click <span class="bold"> <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span> in the left panel, then select <span class="bold"> Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    
1. Click the `Settings` icon on the scheduling timeline.  

1. On the Resource Scheduling Settings dialog box, enable the `Show Completed Work`&nbsp;option.  
   ![RSS_show_completed_work_disabled__1_.png](assets/rss-show-completed-work-disabled--1--350x336.png)


1. Click `Return to Scheduling`.  
   Completed work is displayed with a checkmark in the upper-right corner of the work item.  





## Configure Project Names to display on the scheduling timeline&nbsp; {#configure-project-names-to-display-on-the-scheduling-timeline}

You can configure the project name to display on each task and issue on the scheduling timeline. This allows users viewing the scheduling timeline to quickly see the name of the project where the task or issue resides.


When you enable project names to display, each task and issue consumes more vertical space on the scheduling timeline, resulting in fewer tasks and issues displaying in a single view.


By default, project names are not displayed on tasks and issues on the scheduling timeline.


To display project names on tasks and issues on the scheduling timeline:



1.  Go to the scheduling timeline for multiple projects or for a team: 

    
    
    *  **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    *  **For a team**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Teams</span>, select a team, click <span class="bold"> <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span> in the left panel, then select <span class="bold"> Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    
  


1. Click the `Settings` icon on the scheduling timeline.  

1. On the Resource Scheduling Settings dialog box, enable the option,  `Show Project Names`.  
   ![RS_scheduling_tab_all_settings__2_.png](assets/rs-scheduling-tab-all-settings--2--350x348.png)


1. Click `Return to Scheduling`.  
   Each task and issue on the scheduling timeline displays the name of the project where the task or issue resides.  
   ![resourcescheduling_projectnames.png](assets/resourcescheduling-projectnames-350x200.png)






## Configure Projected Dates to display on the scheduling timeline {#configure-projected-dates-to-display-on-the-scheduling-timeline}

By default, Planned Dates are used on the scheduling timeline. Alternatively, you can configure the scheduling timeline to use Projected Dates.


Consider the following information about Planned and Projected Dates:



*  Planned Dates for tasks can be set manually, or they can be set automatically, depending on task constraint and duration type. For more information, see&nbsp;the articles [Task Constraint overview](task-constraint-overview.md)&nbsp;and&nbsp; [Overview of Task Duration and Duration Type](task-duration-and-duration-type.md)&nbsp;.


  Planned Dates for issues&nbsp;are manually set on issues by users. However, the system administrator can restrict users from adjusting Planned Dates for issues.

* Projected Dates for both tasks and issues are set&nbsp;automatically. For more information about the Projected Dates, see&nbsp;the articles [Overview of the Projected Completion Date for projects, tasks, and issues](project-projected-completion-date.md).




>[!NOTE]
>
>When using Projected Dates on the scheduling timeline, user allocation information cannot be displayed. For more information about user allocations, see the article [Manually assign unassigned tasks and issues in the Scheduling areas](manually-assign-items-scheduling-areas.md).


To configure the scheduling timeline to display tasks and issues according to Projected Dates:&nbsp;



1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
    
    
    * **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For an individual project**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Go to a project, click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For a team**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Teams</span>, select a team, click <span class="bold"> <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span> in the left panel, then select <span class="bold"> Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    
1.  Click the  `Settings`&nbsp;icon on the scheduling timeline.  

1. On the Resource Scheduling Settings dialog box, disable the  `Use Planned instead of Projected Dates`&nbsp;option.
1. Click `Return to Scheduling`.




## Configure how users are displayed on the scheduling timeline {#configure-how-users-are-displayed-on-the-scheduling-timeline}



>[!NOTE]
>
>This section applies only when scheduling resources for teams (from the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Scheduling section for a team</MadCap:conditionalText>`). When scheduling resources for multiple projects (from the Scheduling tab) or for a single project (from the Staffing tab), users cannot be displayed alphabetically; they are always organized by role.


When scheduling resources for a team, you can configure users to be displayed on the&nbsp;scheduling timeline either alphabetically or by role. By default, users are displayed alphabetically (roles are not displayed).



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click&nbsp;Teams. A team is selected by default. </MadCap:conditionalText>`
1. Click the `Settings` icon on the scheduling timeline.  

1. On the Settings dialog box, select whether to enable the `Group by Role` option.   
   When this option is disabled, users are displayed in alphabetical order, and roles are not shown on the scheduling timeline.  
   When this option is enabled, roles are displayed on the scheduling timeline, and users are grouped within their respective role. If a given user has multiple roles defined in the system, that user appears multiple times on the scheduling timeline, beneath each appropriate role.  
   ![RS_working_on_team_scheduling_full_settings__1_.png](assets/rs-working-on-team-scheduling-full-settings--1--350x348.png)


1. Click `Return to Scheduling`.




## Configure whether parent tasks are displayed on the scheduling timeline {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Parent Tasks display differently depending on which scheduling timeline you are accessing.&nbsp;



*  [Display parent tasks for multiple projects](#parents-in-scheduling-tab) 
*  [Display parent tasks for a project or a team](#parents-in-staffing-and-teams) 




### Display parent tasks for multiple projects {#display-parent-tasks-for-multiple-projects}

When scheduling resources for multiple projects in the Scheduling `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`, whether parent tasks display or not depends on the following settings:



* The Completion Mode of the Project.
* The Summary Completion Mode of the Project.
* The Show Parent Tasks setting on the Scheduling tab.


The following table outlines when the parent tasks display in the Scheduling tab, and when only the subtasks display.&nbsp;

For information about configuring the `Completion Mode`and the `Summary Completion Mode`fields for each project, see the section "Settings"&nbsp;in&nbsp;the article [Edit projects](edit-projects.md). 


You can manually configure the Show Parent Tasks setting in the Scheduling `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>` for multiple projects.&nbsp;


To configure the Show Parent Tasks setting:&nbsp;



1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>` 
1. Click the `Settings` icon on the scheduling timeline.  

1. In the Resource Scheduling Settings dialog box, select whether to enable the option,  `Show Parent Tasks.`  
   When this option is enabled, parent tasks from all projects are displayed according to the Summary Completion Mode and the Completion Mode settings of the projects, as outlined in the above table. This option is enabled by default.  
   ![RS_scheduling_tab_all_settings__3_.png](assets/rs-scheduling-tab-all-settings--3--350x348.png)


1. Click `Return to Scheduling`in the lower-left corner.




### Display parent tasks for a project or a team {#display-parent-tasks-for-a-project-or-a-team}

When scheduling resources in the Staffing `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section </MadCap:conditionalText>`of a project or in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Schedule section</MadCap:conditionalText>`, whether Parent Tasks display or not depends on the following settings:



* The Completion Mode of the Project.
* The Summary Completion Mode of the Project.


For information about configuring the `Completion Mode` and the  `Summary Completion Mode`fields for each project, see the section "Settings" in&nbsp;the article [Edit projects](edit-projects.md). 


The following table outlines when the Parent Tasks display in the Staffing `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section </MadCap:conditionalText>`of a project or in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Schedule section</MadCap:conditionalText>`, and when only the subtasks display.&nbsp;



## Configure whether daily Planned Hours are displayed on the scheduling timeline {#configure-whether-daily-planned-hours-are-displayed-on-the-scheduling-timeline}

To configure the scheduling timeline to display the daily totals for the Planned Hours for every user:&nbsp;



1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
    
    
    * **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For an individual project**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Go to a project, click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For a team**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Teams</span>, select a team, click <span class="bold"> <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span> in the left panel, then select <span class="bold"> Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    
1. Click the `Settings` icon on the scheduling timeline.  

1. In the Settings dialog box, enable the following options: 
    
    
    *   `Show Totals for Daily Planned Hours`: Shows the total of the daily Planned Hours for each user.
    * `Show Resource Allocation Highlighting`: Highlights the allocation of the user for tasks and issues, as well as highlights the days when the users are overallocated.  
      These options are disabled by default.  
      ![RS_all_settings__1_.png](assets/rs-all-settings--1--350x358.png)    
    
    
    
    
1. Click `Return to Scheduling`.  
   The total of Planned Hours allocated to the user display for each day.  
   The Planned Hours for the days when the user is overallocated are highlighted in red.  
   For more information about user allocations, see the article [Manually assign unassigned tasks and issues in the Scheduling areas](manually-assign-items-scheduling-areas.md).  





## Configure whether all&nbsp;user tasks are displayed on the scheduling timeline {#configure-whether-all-user-tasks-are-displayed-on-the-scheduling-timeline}



>[!NOTE]
>
>This option applies only when scheduling resources for individual projects (from the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Scheduling section of the project</MadCap:conditionalText>`). This option is not available when scheduling resources for multiple projects (from the Scheduling `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`) or for teams (from the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Scheduling section for a team</MadCap:conditionalText>`).





To configure whether all tasks assigned to each user (not just the tasks associated with the project you are viewing) are displayed on the scheduling timeline:



1. Go to the project where you want to configure the scheduling timeline to display all tasks assigned to each user.
1.  
   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel (it might be located under  <span class="bold">Show More</span>), then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>` 
1. Click the `Settings` icon on the scheduling timeline.  

1. In the Settings area, select whether to enable the option,  `Show All User Tasks`.  
   When this option is enabled, all tasks assigned to each user are displayed on the scheduling timeline, regardless of the project where the tasks are located.  
   This option is disabled by default.   
   ![RS_project_scheduling_area__1_.png](assets/rs-project-scheduling-area--1--350x340.png)


1. Click `Return to Scheduling`.


