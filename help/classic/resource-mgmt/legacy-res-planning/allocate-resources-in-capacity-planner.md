---
filename: allocate-resources-in-capacity-planner
product-area: resource-management
navigation-topic: legacy-resource-planning
title: Allocate resources in the Capacity Planner
description: You can manage your job role resource allocation using the Capacity Planner. For more information about the Capacity Planner, see Plan resources in the Capacity Planner.
---

# Allocate resources in the Capacity Planner

>[!IMPORTANT]
>
>Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the new Workfront experience as soon as possible.

>[!IMPORTANT]
>
>The information in this article refers to functionality that is currently deprecated and will be removed from Workfront. For information about the current functionality for managing resources in Workfront, see the [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md) section.

You can manage your job role resource allocation using the Capacity Planner. For more information about the Capacity Planner, see [Plan resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md).

>[!NOTE]
>
>The resource allocations estimated in the Capacity Planner are the Budgeted Hours, FTEs, or costs of your resources. The Planned Hours on the tasks in your projects are considered the scheduled resources on the projects.

You must have a Plan license with administrative access to Resource Pools to be able to use the Capacity Planner. For more information about administrative access, see [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

The Capacity Planner allows users to estimate the allocation of resources in the following ways:

* Manually, by entering the number of hours, FTEs, or the cost of each resource for the timeframe of the project.
* Automatically, by using one of the options inside the hammer icons of the Capacity Planner.

## Allocate resources in the Capacity Planner manually

Resource allocations for your projects should be populated from the Resource Estimates area at the project level when the project is associated with a Legacy Resource Pool, as part of the Business Case. For more information about defining Resource Estimates for a project, see [Estimate project resources by applying Legacy Resource Pools to the Business Case](../../manage-work/projects/define-a-business-case/apply-legacy-pools-to-business-case.md).

You can also estimate your resource allocations to projects in the Projects area of the Capacity Planner. For more information about estimating resources in the Capacity Planner, see the [Plan resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md) section in [Plan resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md).

## Allocate resources in the Capacity Planner automatically

You can estimate the allocation of your resources by using one of the options available in the hammer icon, inside the Projects area of the Capacity Planner.

The hammer icon is available for the following fields:

* All the projects in the Capacity Planner
* One project
* One job role

For more information about the icons and options in the Capacity Planner, see the [Plan resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md) section in [Plan resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md).

The following options allow you to automatically modify the estimates of your resource allocations in the Capacity Planner:

* [Set Budget to Schedule](#set-budget-to-schedule) 
* [Set to Net Remaining](#set-to-net-remaining) 
* [Set Best Fit](#set-best-fit) 
* [Move Schedule to Budget](#move-schedule-to-budget)

### Set Budget to Schedule {#set-budget-to-schedule}

By setting the budget to match the schedule you are estimating that the time needed to complete the work equals the Planned Hours of the tasks on the project. In this case, your Planned Hours are equal to the Budgeted Hours.

This activity should be done only if you know that project planning has been completed and an accurate number of Planned Hours has been assigned to all the tasks. Otherwise, you may replace initial estimates with values from the schedule that are less accurate. The project manager has the responsibility to update the initial estimates from the schedule.

![set_budget_to_schedule.png](assets/set-budget-to-schedule-350x52.png)

### Set to Net Remaining {#set-to-net-remaining}

By setting the budgeted resources to the net remaining, you are estimating that the time needed to complete the work equals the difference between the total availability of each resource and the amount of time already budgeted for other projects. If you are trying to use this option on a resource pool you created previously, this option changes your resource budgets to reflect this information.

**Set to Net Remaining** should only be used only in the following scenarios:

* if you have established the budget for all other Legacy Resource Pools
* if you have defined a new set of users as part of a pool and know that all unallocated resources also belong to this pool.

![set_to_net_remaining.png](assets/set-to-net-remaining-350x55.png)

### Set Best Fit {#set-best-fit}

By setting the budgeted resources to the **Best Fit**, you are asking Workfront to find the earliest available start time with the fewest over-allocations for each project. This is similar to the **Move Schedule to Budget** setting. This setting calculates the best fit for your projects based on the following criteria:

* the resource requirements for the projects.
* the priority of the projects (which is determined by the order in which the projects appear in the Capacity Planner).  
  For more information about the priority of projects in the Capacity Planner, see the [Prioritize projects in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md#establishing-project-priority) section in [Plan resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md).

* resource availability.

>[!NOTE]
>
>T his option will change the dates on your tasks. If the project has to complete by a certain time, this option might alert you that a best fit is not possible within the time frame of the project.

![set_to_best_fit.png](assets/set-to-best-fit-350x53.png)

### Move Schedule to Budget {#move-schedule-to-budget}

By moving the schedule to match your budget, you are asking Workfront to move the project timeline according to the first available time when all resources are available without any over-allocations. This is similar to **Set Best Fit**.

This setting calculates the best fit for your projects based on the following criteria:

* the resource requirements for the projects.
* the priority of the projects (which is determined by the order the projects appear in the Capacity Planner).  
  For more information about the priority of projects in the Capacity Planner, see the [Prioritize projects in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md#establishing-project-priority) section in [Plan resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/plan-resources-in-capacity-planner.md).

* resource availability.

Using this option will also shift the planned dates to earliest available resource estimates that best fit the needs of the project.

>[!NOTE]
>
>This option will change the dates on your tasks. If the project has to complete by a certain time, this option might alert you that a best fit is not possible within the timeframe of the project.

![move_schedule_to_budget.png](assets/move-schedule-to-budget-350x55.png)

