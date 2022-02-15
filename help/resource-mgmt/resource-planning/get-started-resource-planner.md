---
filename: get-started-resource-planner
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
---



# *`Resource Planner`* overview {#resource-planner-overview}

You can estimate and budget the allocation of your resources to the projects they are assigned to and forecast their availability for future work using the *`Resource Planner`*. 


For a general overview of resource planning in *`Adobe Workfront`*, see the article [Get started with Resource Planning](get-started-resource-planning.md).


## *`Resource Planner`* overview  {#resource-planner-overview-1}

You can use the *`Resource Planner`* to easily understand the availability of users and job roles, as well as the planned time necessary to complete work on projects. You can then decide how to allocate your users and their job roles on the projects they are assigned to based on their available time. 


>[!IMPORTANT] {type="important"}
>
>
>You cannot use the *`Resource Planner`* to assign actual work (tasks and issues) to users. You can only estimate the amount of time needed for the users or job roles to complete a project, regardless of the tasks and issues they are assigned to.  >
>To assign actual work to users you must use the *`Workload Balancer`*. For more information about the *`Workload Balancer`*, see [Overview of the Workload Balancer](overview-workload-balancer.md).  


You can view information in the *`Resource Planner`* using three separate views. You can use each view to fulfill one of the following purposes: 



* To budget the time or cost of your resources for the work that needs to be accomplished using the Project and Role views. This is the main purpose of the *`Resource Planner`*.   
  For more information about budgeting in the *`Resource Planner`*, see the article [Resource Planner overview](#using2).

*  To view the following information using the User view: 
    
    
    * the availability of your users according to their schedule
    * the planned amount of time needed to complete the work according to the project plan. 
    * the amount of time that users have already logged on actual work items.
    
    
  For more information about viewing Available, Planned, and Actual Hours or FTE for users in the *`Resource Planner`*, see the article [View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view](view-hours-fte-user-view-resource-planner.md#using). 





## *`Resource Planner`* considerations {#resource-planner-considerations}




*  You can prioritize the projects you are working on, and budget your resource allocation according to their priority, to ensure that you have resources allocated to the most important projects first. 


  For information about prioritizing projects in the *`Resource Planner`*, see [Prioritize projects in the Resource Planner](prioritize-projects-resource-planner.md). 

*  You can display hours, FTE, and cost information from the tasks and issues of projects. 


  >[!NOTE]
  >
  >Tasks and issues do not display in the *`Resource Planner`*. However, the hours, FTE, and cost information from the resource allocations on the tasks displays in the *`Resource Planner`* as a total number for the project. 



*  The hour, FTE, and cost information from parent tasks is excluded from the projects that display in the *`Resource Planner`*. We recommend assigning resources only to children tasks if you want to manage those resources' time or cost in the *`Resource Planner`*.


  For information about parent tasks, see the following articles: 

    
    
    *  [Tasks overview](tasks-overview.md) 
    *  [Create subtasks](create-subtasks.md) 
    
    


  >[!TIP] {type="tip"}
  >
  >Parent tasks display a total of the hours and costs of the children tasks. Because of this, counting hours, FTE, and cost from the children tasks and the parent tasks would count these amounts twice. This is why the parent task information is excluded from the *`Resource Planner`*. 



*  You cannot manage the allocation of teams on the projects on which they have tasks or issues in the *`Resource Planner`*. 
*  You can budget resources for multiple projects at a time using the *`Resource Planner`*, or for a single project using the Resource Budgeting area of the Business Case. The information you budget for one project also displays in the *`Resource Planner`*. 


  For information about how you can budget resources for a single project, see the article [Budget resources in the Business Case](budget-resources-in-business-case.md).


  For information about how you can budget resources in the *`Resource Planner`* for multiple projects at a time, see the section "Budget resources in the *`Resource Planner`*" in the article [ [Budget resources in the Resource Planner using the Project and Role views](budget-resources-project-role-views-resource-planner.md)](budget-resources-project-role-views-resource-planner.md).





## Prerequisites for working in the *`Resource Planner`* {#prerequisites-for-working-in-the-resource-planner}

To successfully use the *`Resource Planner`* for budgeting your resources, you must first ensure that you, your projects, and your tasks meet a set of prerequisites. These prerequisites are mandatory to display the correct information in the *`Resource Planner`* and to accurately manage your resources. 




>[!IMPORTANT] {type="important"}
>
>If any of the following prerequisites are missing, you might find that some of the information about the allocation or the availability of the resources is missing or has a zero value.  
>For more information understanding why fields are missing data or have zero values, hover over the fields. 





![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)




>[!NOTE]
>
>The following prerequisites are required only when viewing the *`Resource Planner`* by project or by job role or when budgeting resources in the Business Case of a project.  
>For more information about the views in the *`Resource Planner`*, see the "Project/ Role/ User view" selection section in the article [Resource Planner overview](#).  



The following types of prerequisites are required for the correct functionality of the *`Resource Planner`* when viewing it by project or by role: 



* [User prerequisites](#user-prerequisites) 
* [Project prerequisites](#project-prerequisites) 
* [Tasks and issues prerequisites](#tasks-prerequisites) 
* [System-level prerequisites](#system-l) 




### User prerequisites {#user-prerequisites}

Ensure the following user setup exists before starting using the *`Resource Planner`*:



*  You have the correct access to budget resources.


  For information about the access needed to budget resources, see the article [Access needed to budget resources](access-needed-to-budget-resources.md).






*  Users who are assigned to tasks are added to the Resource Pools associated with the project.


  For information about adding users to Resource Pools, see the article [Work with Resource Pools](work-with-resource-pools.md).




  >[!NOTE]
  >
  >When users are not added to Resource Pools, the following scenarios may exist: 
  >
  >    
  >    
  >    * The users do not appear in the *`Resource Planner`* although they might be assigned to tasks on the projects. 
  >    * If the tasks they are associated with have Planned Hours, those hours do not appear for the project in the *`Resource Planner`*, unless the user is also associated with a job role on those tasks. 
  >    * If the users are associated with a job role on a task on the project, the Planned Hours display in the *`Resource Planner`* for the job role, but the job role cannot be budgeted. 
  >    
  >    





*  Users who are assigned to work and Resource Pools must have Schedules and Job Roles associated with their profile.


  For information about associating Schedules and Job Roles with users, see [Edit a user's profile](edit-a-users-profile.md).


  >[!NOTE]
  >
  >Users who are not associated with a Schedule but are in the Resource Pool of the project cannot be budgeted in the *`Resource Planner`*.



*  For accurate Available Hours information, ensure that the schedules associated with your users have the schedule exceptions and time off updated.


  >[!NOTE]
  >
  >If a user is not associated with a Schedule, the Default Schedule of your *`Workfront`* system is associated with the user by default, for the purposes of the *`Resource Planner`*. 


  For information about creating schedules, see the article [Create a schedule](create-schedules.md).  







*  If you want to budget your resources by Cost, you must associate Job Roles with Cost/Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.  
  For information about associating job roles with rates, see the article [Create and manage job roles](create-manage-job-roles.md).  
  For information about calculating Budgeted Labor Cost, see the article [Understand Budgeted Labor Cost and Budgeted Hours for projects](budgeted-labor-cost.md).  
  For information about calculating Budgeted Cost, see the article [Calculate Budgeted Cost](budgeted-cost.md).




### Project prerequisites {#project-prerequisites}

Ensure the following project setup exists before starting using the *`Resource Planner`*:



*  Your projects are associated with Resource Pools.  
  For more information about adding Resource Pools to projects, see the "Associate Resource Pools with projects and templates" section in the article [Work with Resource Pools](work-with-resource-pools.md).  


  >[!IMPORTANT] {type="important"}
  >
  >Projects without Resource Pools do not display Planned Hour or assignments information in the *`Resource Planner`*. 







### Tasks and issues prerequisites {#tasks-and-issues-prerequisites}

Although you cannot display tasks and issues in the *`Resource Planner`*, their information transfers to the projects that display in the *`Resource Planner`* . 


Ensure the following task and issue setup exists before starting budgeting resources in the *`Resource Planner`*:



*  The tasks or issues on the projects for which you are budgeting resources are assigned to one of these entities:  

    
    
    * `<li>Users in the Resource Pools of the project who are also associated with Job Roles</li>``<li><p>Job Roles</p></li>`
    
    
    


  >[!NOTE]
  >
  >Teams assigned to tasks or issues do not display in the *`Resource Planner`**. *The Planned Hours of tasks and issues assigned to job roles display in the *`Resource Planner`*, but these hours cannot be budgeted unless a user who is associated with the job role is listed in a Resource Pool associated with the project.



*  You should not assign parent tasks to users or roles.


  To display hour information in the *`Resource Planner`* for users or roles associated with parent tasks you must also assign them to the children tasks. The *`Resource Planner`* does not display information from parent tasks. 

* Tasks and issues have a value for Planned Hours which is greater than zero. 
* Tasks and issues have a value for their Duration which is greater than zero. 
* The Planned Dates of the issues are within the timeline of the project. 




### System-level prerequisites {#system-level-prerequisites}

You must understand how your instance of *`Workfront`* calculates user availability according to the Resource Management Preferences in your system. *`Workfront`* can calculate user availability using the user's schedule or the Default Schedule of your system.


![](assets/resource-management-preferences-section-in-setup-350x89.png)




Your *`Workfront administrator`* configures your Resource Management Preferences.


For more information, see [Configure Resource Management preferences](configure-resource-mgmt-preferences.md).



## Locate the *`Resource Planner`* {#locate-the-resource-planner}

You can locate the *`Resource Planner`* in two areas of *`Workfront`*, depending on whether you want to budget your resources for multiple projects, or for just one project.


For information about locating the *`Resource Planner`*, see [Locate the Resource Planner in Adobe Workfront](locate-resource-planner.md). 


## The areas of the *`Resource Planner`* {#the-areas-of-the-resource-planner}

You can view the following information or perform the following actions in the *`Resource Planner`*: 



*  Information about the resources assigned to your projects in the *`Resource Planner`* in a general timeline. 
*  Overallocation or underutilization of your resources in the *`Resource Planner`*. 
*  Budget your resources for work manually, or automatically. 


For more information about what areas display in the *`Resource Planner`* and how to configure what information displays in these areas, see the article [Resource Planner navigation overview](resource-planner-navigation.md).


## Limitations in displaying information in the *`Resource Planner`* {#limitations-in-displaying-information-in-the-resource-planner}

To improve performance, *`Workfront`* limits the amount of items you can display in the *`Resource Planner`*. 


For more information about these limitations, see the article [Resource Planner display limitations](resource-planner-display-limitations.md) . 


## Calculate FTE in the *`Resource Planner`* {#calculate-fte-in-the-resource-planner}

You can display availability, allocation, and planned values in the *`Resource Planner`* in Hours, FTE, or Cost.


For more information about changing the information you display in the *`Resource Planner`*, see the section [View information by Hour, FTE, or Cost](resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) in the article [Review resource availability and allocation using the Resource Planner](resource-availability-allocation-resource-planner.md).


For more information about how the Hours and FTE for users and roles are calculated in *`Workfront`*, see the article [Overview of calculating hours and FTE for users and roles in the Resource Planner](calculate-hours-fte-for-users-roles-resource-planner.md).


## Calculate Costs in the *`Resource Planner`* {#calculate-costs-in-the-resource-planner}

You must have View access to Financial Data and View Finance permissions on the projects to see the information by Cost in the *`Resource Planner`*.


Along with displaying availability, allocation, and planned values in the *`Resource Planner`* in Hours and FTE, you can also display them by Cost. 


>[!TIP] {type="tip"}
>
>You must associate your users and your job roles with Cost per Hour rates in order to display information by Costs in the *`Resource Planner`*.


For more information about associating Cost per Hour rates with job roles, see the article [Create and manage job roles](create-manage-job-roles.md).  
For more information about associating Cost per Hour rates with users, see the article [Edit a user's profile](edit-a-users-profile.md).


Consider the following when viewing information by Cost in the *`Resource Planner`*:



* The Cost of each type of hours (Planned, Available, Budgeted, Actual for Users, Roles, or the Projects) is calculated using a different Cost Rate.
* The Planned Cost is affected by the Cost Type of the tasks on the projects.
* When applying the User View to the *`Resource Planner`*, you cannot display the allocation and availability information by Cost. 


For more information about how Costs are calculated in the *`Resource Planner`* for users and roles, see the article [Calculate costs in the Resource Planner](calculate-costs-resource-planner.md).


## Filter information in the *`Resource Planner`* {#filter-information-in-the-resource-planner}

You can reduce the number of projects, roles, or users that display in the *`Resource Planner`* by creating a filter.   
For more information, see the article [Filter information in the Resource Planner](filter-resource-planner.md).
