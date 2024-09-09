---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Workload Balancer Overview
description: After project managers plan the work on projects by creating tasks and after resource managers allocate job role resources to projects in the Resource Planner, project owners and team managers can use the Workload Balancer to assign work items to users.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
---
# Workload Balancer overview

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

After project managers plan the work on projects by creating tasks and after resource managers allocate job role resources to projects in the Resource Planner, project owners and team managers can use the Workload Balancer to assign work items to users.

>[!IMPORTANT]
>
>You can use the Workload Balancer to assign actual work (tasks and issues) to users. 
>
>You must use the Resource Planner and not the Workload Balancer to estimate job role allocations for your projects, at a high level. For more information about the Resource Planner, see [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

This article describes the general purpose for the Workload Balancer and some of the best practices for how you can set up your projects and resources to successfully use it.

To review video tutorials of the Workload Balancer, go to the [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html) page. In the left menu, select **Manage resources** > **Workload Balancer** and choose a tutorial.

## Locate the Workload Balancer

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

We recommend using the Workload Balancer in the following areas for scheduling resources: 

* At the system level, in the Resourcing area.
* At the project level, in the Workload Balancer section of a project. 
* At the team level, in the Workload Balancer section of a team. 

For more information about locating the Workload Balancer, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Benefits of the Workload Balancer

Consider the following benefits when using the Workload Balancer:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Access a clear visual mapping of resource overallocation and underutilization which is transparent to all stakeholders. 
* As a people manager, you can protect your people from burnout and empower them to do their best work with better focus, quality, and engagement. You can ensure their full utilization, break silos, and enable alignment of work across teams. 
* When you assign work at the task or issue level you don't have visibility into how busy a user might be. When you use the Workload Balancer, you can view which users have availability in their workload to complete the task or issue on time. This includes their time off and schedule exceptions details.

  For more information, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  You can also assign work items in bulk which makes it easier to distribute many work items at one time, across multiple projects. For more information, see [Assign work in bulk using the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md). 

* Executives can make timely staffing decisions through transparency into how people in their organization are utilized. 
* Team members benefit from better collaboration, as they can all view what their coworkers are working on at any given time. For information about the access needed to view or manage resources in the Workload Balancer, see [Access needed to manage resources in the Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Share it with anyone that does not have access to the Resourcing area by embedding a link to it in a custom tab. For information, see [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualize and manage people's workloads and demand in one view at the global, project, or team level, depending on your role. When managing projects, this includes not only resource allocation for the project, but also visualizing the allocation of resources from the Adobe Workfront Scenario Planner. People managers use the Workfront Scenario Planner to manage job skills across the organization. The Scenario Planner is only available in the new Adobe Workfront experience.

  >[!NOTE]
  >
  >  The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../scenario-planner/scenario-planner-overview.md).


## Best practices for using the Workload Balancer

We recommend the following best practices for planning projects, configuring users, and using filters before starting scheduling your resources using the Workload Balancer.

* [Best practices for displaying information in the Workload Balancer](#best-practices-for-displaying-information-in-the-workload-balancer) 
* [Best practices for setting up users](#best-practices-for-setting-up-users) 
* [Best practices for setting up tasks and issues](#best-practices-for-setting-up-tasks-and-issues)

### Best practices for displaying information in the Workload Balancer {#best-practices-for-displaying-information-in-the-workload-balancer}

We recommend that you use filters so you can display only the information that is pertinent to you for both unassigned and assigned work items.

For information about creating and using filters in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Best practices for setting up users

* As the user who schedules work for others, you must have the correct access and permissions to schedule resources for work.

  For information about the access needed to manage the workload of your resources in the Workload Balancer, see [Access needed to manage resources in the Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md). 

* The users whose workload you want to manage must meet the following criteria so that the information about their availability and skills is accurate:

   * Have Schedules and Job Roles associated with their profile.
     
     For more information about associating Schedules and Job Roles with users, see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * If a user is not associated with a Schedule, the Default Schedule of your Workfront system is associated with the user by default, for the purposes of resource management. 
   * Have Schedule Exceptions updated in their schedules.  
     
     For more information about creating schedules, see [Create a schedule](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
   
   * Have their Time Off calendar updated in their profile.   
     
     For information about updating a user's Time Off calendar, see [Configure personal time off](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* The Workfront administrator must determine how Workfront calculates user availability. They can decide whether Workfront uses the System Default Schedule, or the user's schedule to calculate the time that the user is available to work by adjusting the Resource Management preferences in the Setup area of Workfront. 
  
  For more information, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Best practices for setting up tasks and issues {#best-practices-for-setting-up-tasks-and-issues}

Ensure the following task and issue setup exists before starting assigning work to users in the Workload Balancer:

* Parent tasks are not assigned to users or roles. Parent tasks do not display in the Workload Balancer. 
* Tasks and issues have a value for Planned Hours which is greater than zero. 

* Tasks and issues have a value for their Duration which is greater than zero. 
* The Planned Dates of the issues are within the timeline of the project.

## Before you start to use the Workload Balancer

* Review the following articles before you start using the Workload Balancer: 

    * This article walks you through how to navigate the Workload Balancer to perform these actions: [Navigate the Workload Balancer](../workload-balancer/navigate-the-workload-balancer.md). 

  * The following articles walk you through how you assign work and manage user allocations:
  
    * [Overview of assigning work in the Workload Balancer](../workload-balancer/assign-work-in-workload-balancer.md).
    * [Manage user allocations in the Workload Balancer](../workload-balancer/manage-user-allocations-workload-balancer.md). 

* The Workload Balancer can be found several different areas of Workfront. For information about where you can find the Workload Balancer, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Access needed to use the Workload Balancer

You must have the correct Workfront access and permissions to specific projects to be able to view and use the Workload Balancer in Workfront. For information about the access needed to use the Workload Balancer, see the article [Access needed to manage resources in the Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
