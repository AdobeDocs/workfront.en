---
filename: get-started-resource-management
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
---



# Get started with Resource Management  {#get-started-with-resource-management}

Resource Management allows you to configure your system to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget. 


## Overview of Resource Management in *`Adobe Workfront`* {#overview-of-resource-management-in-adobe-workfront}

Resource Management refers to all the activities performed by the *`Adobe Workfront administrator`*, the resource manager, and the Project Owner for the forecasting and scheduling of resources to the work that these resources are assigned to taking into account their availability. 


*`Workfront`* has several sets of tools used to manage resources. Although some of these tools overlap, each one has an individual scope. Currently, you can use the following Resource Management tools in *`Workfront`*, depending on which stage of resource management you are in: 



*  To plan how resources are allocated at a higher level, before the actual work on projects begins, use the following tool`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> s</MadCap:conditionalText>`: 

    
    
    *  `The *`Resource Planner`*`: You can use the *`Resource Planner`* in the first stage of resource management to budget project time for your resources according to their scheduled availability. During the planning of resources phase, you can organize users in&nbsp;Resource Pools and assign multiple Resource Pools to a project. *  
      *For more information about Resource Planning, see the section [Resource Planning in Adobe Workfront](_resource-planning-overview.md).
    *  `**The ** *`Scenario Planner`*: This is a higher-level planning of resources that allows you to manage them across multiple initiatives and to use the best scenario for making the most out of their availability and your budget.` `This is available only in *`the new Adobe Workfront experience`* and requires an additional license. For information about the *`Workfront Scenario Planner`*, see` [The Adobe Workfront Scenario Planner overview](scenario-planner-overview.md). 
    
    






*  To schedule or assign resources to actual work (tasks and issues), use the following tools: 

    
    
    * `The Workload Balancer`(recommended): This is a lower-level stage of resource management, where you can assign your resources to the actual work (tasks and issues) that they must complete, based on the amount of hours needed to complete them and their availability. Using the *`Workload Balancer`* you can assign to users actual work that is currently unassigned or assigned to job roles.
    
    
      For information about the Workfront Balancer, see the section [The Workload Balancer](_workload-balancer.md). 
    
    *  `Scheduling` (deprecated): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This is a lower-level view of resource management, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  
      For more information about resource scheduling, see the section [Resource Scheduling](_resource-scheduling-overview.md). 
    
    
      >[!NOTE]
      >
      >We are no longer developing the Resource Scheduling tools and they will soon be removed from *`Adobe Workfront`*. We recommend that you use the *`Workload Balancer`* for scheduling your resources. 
      >
      >
      >For information about scheduling resources using the new *`Workload Balancer`*, see the section [The Workload Balancer](_workload-balancer.md).
      >
      >
      >For more information about the timeline for removing the Resource Scheduling tools and replacing them with the *`Workload Balancer`*, see [Deprecation of Resource Scheduling tools in Adobe Workfront](deprecate-resource-scheduling.md).

    
    
    
    
    






*  To analyze budgeted, planned, and actual allocations across multiple projects, use the following tool: 

    
    
    *  `Utilization Report`: Use this report to view the utilization of resources for projects. You can compare budgeted, planned, and actual allocations for your projects and their impact on the cost and revenue of the projects. For information about the Utilization&nbsp;Report, see [View resource utilization information](view-utilization-information.md).
    
    





## The components of the Resource Management process {#the-components-of-the-resource-management-process}



>[!NOTE]
>
>Resource Management is never a stagnant process in *`Workfront`*. As the schedules of your projects, the availability of your users, or their roles change, you must continually adjust the information about your resources, their assignments, and their allocations to projects, tasks, and issues. 


The process of managing resources in  *`Workfront`* includes the following stages: 



* `Configuration`: As a resource manager or Project Owner, you or your *`Workfront administrator`* must configure certain fields and objects in your *`Workfront`* instance before managing your resources. For more information about the prerequisites necessary to start managing resources in *`Workfront`*, see the [Prerequisites for accurate resource management](#prerequisites) section in this article.   
  In addition to having projects with work items, you must configure the following items in *`Workfront`*:  

    
    
    * Users  
      For more information about creating users, see the article [Add users](add-users.md).
    
    * Job Roles  
      For more information about creating job roles, see the article [Create and manage job roles](create-manage-job-roles.md).
    
    * Schedules  
      For more information about creating schedules, see the article [Create a schedule](create-schedules.md).
    
    * Project Preferences
    
    
      >[!TIP] {type="tip"}
      >
      >Only a system administrator can modify Project Preferences.
    
    
      For more information about defining Project Preferences, see the article [Configure system-wide project preferences](set-project-preferences.md).
    
    * Resource Pools  
      For more information about creating Resource Pools, see the article [Work with Resource Pools](work-with-resource-pools.md).
    
    
    

*  `Resource allocation`: As a resource manager, or a Project Owner, you can define allocation of resources for your projects as well as assign work. For this step, you can manage the allocation of your resources at the project level using the *`Resource Planner`*. Then, you can assign work items (tasks and issues) to users based on their job roles using the resource scheduling tools. 


  For more information about resource planning, see the following sections:

*  `<li> <a href="_resource-planning-overview.md" class="MCXref xref" xrefformat="{para}">Resource Planning in Adobe Workfront</a></li>` `<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><a href="_scenario-planning.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner</a> </p> </li>` 

* For more information about resource scheduling, see the section [Resource Scheduling](_resource-scheduling-overview.md).
* `Analysis`: As a resource manager, Project Owner, or people manager, review the Utilization&nbsp;Report to understand how the budgeted and planned allocations of your resources compare to the actual ones. Review information by hours, cost, or revenue. For information about the Utilization report, see [View resource utilization information](view-utilization-information.md). 





## Access needed to view and manage resources using the Resource Management tools in *`Workfront`* {#access-needed-to-view-and-manage-resources-using-the-resource-management-tools-in-workfront}

The following users have access to the Resource Management tools in *`Workfront`*:


You must be one of the following users and have the following access and permissions to access Resource Planning and Scheduling tools:



*  The system administrator.
*  A user with a Plan license 


  In addition to having a *`Plan`* license, you must have the following to use specific resource management tools:

    
    
    *  Edit access to Resource Management to use the Scheduling tool
    * Edit access to Financial Data to display Cost information in the Planner
    * View access to&nbsp;Financial&nbsp;Data to view Cost and&nbsp;Revenue information in the Utilization Report
    
    

* Manage permissions on the projects you want to manage resources for.
*  Designated as a Resource Manager for projects to use the Scheduling tool. 


  >[!TIP] {type="tip"}
  >
  >This is not required for using the *`Resource Planner`* and the *`Workload Balancer`*. 





For information about the access needed to budget resources, see the article [Access needed to budget resources](access-needed-to-budget-resources.md).


For information about the access needed to manage resources in the *`Workload Balancer`*, see [Access needed to manage resources in the Workload Balancer](access-needed-manage-resources-balancer.md).


##  Prerequisites for accurate resource management  {#prerequisites-for-accurate-resource-management}

You must meet a set of requirements before you can efficiently use the resource management tools in *`Workfront`*. 


For information about what the requirements are for each tool see the following:



* The section "Prerequisites for working in the *`Resource Planner`*" in the article [Resource Planner overview](get-started-resource-planner.md)

* The section "Prerequisites" in the article [Get started with Resource Scheduling](get-started-resource-scheduling.md)
* [Access needed to manage resources in the Workload Balancer](access-needed-manage-resources-balancer.md) 



