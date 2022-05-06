---
filename: plan-resources-in-capacity-planner
product-area: resource-management
navigation-topic: legacy-resource-planning
title: Plan resources in the Capacity Planner
description: The Capacity Planner is a Workfront tool for planning resources for your projects inside a Legacy Resource Pool, according to their availability. You cannot use the Capacity Planner outside a Legacy Resource Pool.
---

# Plan resources in the Capacity Planner

>[!IMPORTANT]
>
>Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the new Workfront experience as soon as possible.

>[!IMPORTANT]
>
>The information in this article refers to functionality that is currently deprecated and will be removed from Workfront. For information about the current functionality for managing resources in Workfront, see the [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md) section.

The Capacity Planner is a Workfront tool for planning resources for your projects inside a Legacy Resource Pool, according to their availability. You cannot use the Capacity Planner outside a Legacy Resource Pool.

>[!NOTE]
>
>The Capacity Planner shows an overall allocation of job roles inside of a Legacy Resource Pool to a specific project. It does not show the allocation of the job role at the task level, nor does it show the allocation of users fulfilling those roles at the task level. You must refer to the project plan to understand what tasks each job role is assigned to and what users are assigned to each task.

You must have a Plan license with administrative access to Resource Pools to be able to use the Capacity Planner. For more information about administrative access, see [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Prerequisites for using the Capacity Planner {#prerequisites-for-using-the-capacity-planner}

You can use the Capacity Planner to prioritize future projects based on resource availability. Within a Legacy Resource Pool, you can use the Capacity Planner to compare actual job role assignments on the project to the allocated availability of each job role for a specific time frame.

Before you can start using the Capacity Planner, the following requirements must be met:

* Active users are assigned to at least one job role.
* Active users have a valid value for their FTE field.  
  For more information about editing the job role and the FTE value for users, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Job roles must be placed in a Legacy Resource Pool.  
  For more information about defining Legacy Resource Pools, see [Work with Legacy Resource Pools](../../resource-mgmt/legacy-res-planning/work-with-legacy-resource-pools.md).

* Job roles must be budgeted in the Resource Pools area of the Resource Budget Manager.  
  For more information about budgeting job roles in the Resource Budget Manager, see [Budget Legacy Resource Pools in the Resource Budget Manager](../../resource-mgmt/legacy-res-planning/budget-legacy-pools-in-budget-manager.md).

* Tasks should be assigned to job roles and should have a valid value for Planned Hours and Duration. 
* Projects must be associated with a Legacy Resource Pool and they must have their Resource Estimates defined in the Business Case. Using Resource Estimates, as the project manager, you should estimate how many hours you would need for each job role assigned to tasks to complete their assignments.

  >[!NOTE]
  >
  >The number of estimated hours needed for a resource to complete tasks on a project can be different than the number of Planned Hours on the tasks.

  For more information about defining Resource Estimates for a project, see [Estimate project resources by applying Legacy Resource Pools to the Business Case](../../manage-work/projects/define-a-business-case/apply-legacy-pools-to-business-case.md).

## Access the Capacity Planner {#access-the-capacity-planner}

1. Go to the **People** area in your Global Navigation Bar.
1. Select the **Legacy** **Resource Planning** tab.

1. Select the **Legacy** **Resource Pools** sub-tab

1. Click a **Legacy** **Resource Pool** to select it.

1. Select the **Capacity Planner** tab.  
   This displays the Capacity Planner only for the selected Legacy Resource Pool.

## Overview of the areas of the Capacity Planner

The Capacity Planner consists of 3 areas:

* [Available Resources](#available-resources) 
* [Projects](#projects) 
* [Net Remaining resources](#net-remaining-resources)   
  ![capacity_planner_areas.png](assets/capacity-planner-areas-350x211.png)

### Available Resources {#available-resources}

The Available Resources area of the Capacity Planner shows the total number of job role resources available in your Legacy Resource Pool.

The Available Resources area is not editable. The available number of job roles comes from the Resource Pools area of the Resource Budget Manager. Using the Resource Budget Manager, you can budget the number of hours (or FTEs or cost) that the job roles are available to work.  
For more information about budgeting the availability of job roles in the Resource Budget Manager, see [Budget Legacy Resource Pools in the Resource Budget Manager](../../resource-mgmt/legacy-res-planning/budget-legacy-pools-in-budget-manager.md).

>[!NOTE]
>
>If the Available Resources numbers are zero, you must contact the Resource Manager of your Workfront instance so that they can ensure that all the prerequisites for the Capacity Planner are in place. For more information about the prerequisites needed to use the Capacity Planner, see [Prerequisites for using the Capacity Planner](#prerequisites-for-using-the-capacity-planner) [Prerequisites for using the Capacity Planner](#prerequisites-for-using-the-capacity-planner).

### Projects {#projects}

* [Overview of the Projects area](#overview-of-the-projects-area) 
* [Add projects to the Capacity Planner](#add-projects-to-the-capacity-planner) 
* [Estimate resources in the Capacity Planner](#estimate-resources-in-the-capacity-planner) 
* [Prioritize projects in the Capacity Planner](#prioritize-projects-in-the-capacity-planner)

#### **Overview of the Projects area** {#overview-of-the-projects-area}

The Projects area of the Capacity Planner displays projects you are currently managing for resource management purposes. The projects which are associated with this Legacy Resource Pool are not automatically added to this area. They will have to be added manually. This area of the Capacity Planner is editable. Projects can manually be added or removed from this section and you can manually adjust the allocation of resources to the projects.

You can expand each project to see the allocation of resources for each job role assigned to tasks on the project. The allocation of resources should come from the Resource Estimates completed at the project level, or you can manually update it here. If you update the estimation of resources in the Capacity Planner, the project-level Resource Estimates updates, as well.

The resource estimates in the Capacity Planner and the Resource Estimates of the project represent the estimated budgeted time that the project or resource manager assumes that it would be needed to complete the work on the project.

>[!NOTE]
>
>The allocation of the resources in the Capacity Planner is different than the Planned Hours of the tasks on the project. You can display the Planned Hours associated with your resources, but this value is not editable in the Capacity Planner. However, the resource estimates (the estimated budgeted time) allocated to resources is manually editable in this area.  
>![planned_data_on_capacity_planner.png](assets/planned-data-on-capacity-planner-350x50.png)

#### **Add projects to the Capacity Planner** {#add-projects-to-the-capacity-planner}

You can add projects to the Capacity Planner, even if they are not associated with the Legacy Resource Pool. Adding them to the Capacity Planner in this area will automatically associate them with the Legacy Resource Pool.

To add projects to the Capacity Planner:

1. Access the **Capacity Planner** tab inside a **Legacy** **Resource Pool**.  
   For more information about accessing the Capacity Planner, see [Access the Capacity Planner](#access-the-capacity-planner).

1. To add more projects in the **Projects** area of the **Capacity Planner**, click **Add Projects**.  
   ![](assets/add-projects-capacity-planner.png)

1. In the **Add Project** dialog box, consider specifying the following:

   * **Portfolio**: Select a portfolio to display only the projects associated with it.
   * **Show projects without a Resource Pool**: Select this field, if you want to see projects that are not associated with this Legacy Resource Pool.
   * **Status**: Select the status of the projects that you want to display in the Capacity Planner.
   * **Date Range**: Select the date range for which you want to manage the resource allocation for the projects in this Legacy Resource Pool.

     >[!NOTE]
     >
     >Allocation data displays for 1095 days (or 3 years) in the Legacy Resource Estimates area of the Business Case.

     ![add__project_in_the_capacity_planner.png](assets/add--project-in-the-capacity-planner-350x186.png)

1. As projects start populating the top half of the **Add Project** box, select multiple projects by keeping the "shift" key pressed and clicking a project at a time to select it.
1. Drag and drop the selected projects in the **Projects to Add** area of the **Add Project** dialog box. 

1. Click **OK**.  
   Your projects are appearing in the **Projects** area of the Capacity Planner now.   
   Each line displays one project.

#### **Estimate resources in the Capacity Planner** {#estimate-resources-in-the-capacity-planner}

When you are modifying the resource allocations of each job role in the Capacity Planner, you are changing the resource estimates values for your job roles for a specific project. The Planned Hours associated with the job roles do not change.

To edit the allocation of resources in the Capacity Planner:

1. Access the **Capacity Planner** tab inside a **Legacy** **Resource Pool**.  
   For more information about accessing the Capacity Planner, see [Access the Capacity Planner](#access-the-capacity-planner).

1. In the **Projects** area of the **Capacity Planner**, the projects associated with this Legacy Resource Pool appear after they have been added.

1. Click the icon to the left of the project name, to expand the project.  
   The job roles associated with the project are listed under the project name. 
1. Start typing a value in Hours, FTE, or Cost, for each job role, for each day of the project timeline, to estimate how much time (in hours or FTE) or cost is needed for a specific job role to complete the project.  
   When adding projects, the current total availability of each job role should change and some resources will appear over-allocated. Over-allocations of resources will appear in red.
1. (Optional) Manually modify allocations in the **Projects** area to avoid over-allocations.  
   For more information about allocating resources in the Capacity Planner, see [Allocate resources in the Capacity Planner](../../resource-mgmt/legacy-res-planning/allocate-resources-in-capacity-planner.md).

1. Click **Save**.

#### **Prioritize projects in the Capacity Planner** {#prioritize-projects-in-the-capacity-planner}

Projects located in the **Projects** section of the Capacity Planner receive a priority according to their position in the list.

Capacity Planning priority is unrelated to the ```priority``` setting found on the **Project Details** tab. The Priority field on the Project Details tab is a visual flag that you manually specify to understand how important a project should be. In the Capacity Planner, the project at the top of the list gets assigned resources first, the next project gets assigned resources second, and any projects left on the list receive the resources that remain available.  
![](assets/capacity-planner-350x186.png)

You can change the priority of any project by dragging and dropping it to the desired position in the list.

There is a project priority given to projects that belong to a Portfolio. Inside the Portfolio Optimizer, you can establish what projects are more important to be completed first, by simply placing them in the correct order. For more information about prioritizing projects in the Portfolio Optimizer, see [Prioritize projects in the Portfolio Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

To view the priority a project has in the Portfolio Optimizer in the Capacity Planner:

1. Go to the **Capacity Planner** of a Legacy Resource Pool.
1. Click the **Properties** icon.  
   ![](assets/properties-icon.png)  
   The Preferences dialog box displays. 

1. Select the **Field Data** tab in the Preferences dialog box.
1. Select the **Priority** field in the **Unused** column, then click the arrow pointing right, to move it to the **Used** column.  
   ![](assets/screen-shot-2013-09-19-at-1.03.32-pm-350x242.png)

1. Click **OK**.  
   You can see the priority given to a project in the Portfolio Optimizer in the Priority column you added to the Capacity Planner.  
   If you click the **Priority** column, you can sort your projects the same way they are displayed in the ```Portfolio Optimizer. This ensures that you prioritize your resource allocation according to the same priority by which the portfolio manager expects the project to be completed.```

### Net Remaining resources {#net-remaining-resources}

The Net Remaining Resources area of the Capacity Planner displays the remaining number of resources in the Legacy Resource Pool after allocations have been made to projects.

The Net Remaining Resources area is not editable. Workfront calculates the difference between the total number of resources available for the Legacy Resource Pool (as budgeted in the Resource Budget Manager and displayed in the Available Resources area of the Capacity Planner) and the allocation of resources coming from the projects associated with the Legacy Resource Pool. This calculated number is displayed in the Net Remaining Resources area of the Capacity Planner.

Over-allocated job roles appear in red. Modify the resource allocations for your projects in the Projects area of the Capacity Planner to eliminate the over-allocations.

## Overview of the Capacity Planner navigation

The following icons and options are visible in the Capacity Planner:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Icon</strong> </th> 
   <th><strong>Name</strong> </th> 
   <th><strong>Function</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/undo-redo-change-capacity-planner.png" alt="undo_redo_change_capacity_planner.png"> </td> 
   <td>Undo/ Redo icons</td> 
   <td>Allow you to cancel or redo the changes you made to the Capacity Planner before saving.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/properties-icon.png" alt="properties_icon.png"> </td> 
   <td>Preferences Icon</td> 
   <td>Provides an interface to update the columns in the Projects area and the Date Range. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export-to-excel-icon.png" alt="export_to_excel_icon.png"> </td> 
   <td>Export to Excel</td> 
   <td>Exports the data displayed in the Capacity Planner to a Microsoft Excel file. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/capacity-planner-show-by-drop-down-field.png" alt="capacity_planner_show_by_drop_down_field.png"> </td> 
   <td> <p>Show by:</p> 
    <ul> 
     <li>FTE</li> 
     <li>Hours</li> 
     <li>Cost</li> 
    </ul> <p> </p> </td> 
   <td>Select whether your resources should be estimated using number of FTEs, Hours, or Cost. You must have rates associated with job roles in order to display resource estimates by Cost. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip2.png" alt="mceclip2.png"> </td> 
   <td> <p>View by:</p> 
    <ul> 
     <li>Week</li> 
     <li>Month</li> 
    </ul> </td> 
   <td>Select whether you want to view the timeline of the projects by weekly or monthly allocations. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip3.png" alt="mceclip3.png">, <img src="assets/mceclip4.png" alt="mceclip4.png"></td> 
   <td>Full screen/ End full screen</td> 
   <td>See the Capacity Planner in full screen mode, or end the full screen mode and return to the default view.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip5.png" alt="mceclip5.png"> </td> 
   <td>Add projects icon</td> 
   <td>Use this to add projects to the Capacity Planner, in the Projects area. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/budgeting-in-capacity-planner-350x314.png" alt="budgeting_in_capacity_planner.png" style="width: 350;height: 314;"> </td> 
   <td>Hammer icon for All Projects</td> 
   <td> <p>Allows you to expand or collapse all the projects in the Projects area of the Capacity Planner with one click. </p> <p>You can also automatically manage all the resources from all the projects in this Legacy Resource Pool with one click. For more information about allocating resources to projects automatically, see <a href="../../resource-mgmt/legacy-res-planning/allocate-resources-in-capacity-planner.md" class="MCXref xref">Allocate resources in the Capacity Planner </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/capciaty-planner-budgeting.png" alt="capciaty_planner_budgeting.png"> </td> 
   <td>Hammer icon for one project</td> 
   <td> <p>Allows you to automatically manage all the resources associated with one project with one click. For more information about allocating resources to projects automatically, see <a href="../../resource-mgmt/legacy-res-planning/allocate-resources-in-capacity-planner.md" class="MCXref xref">Allocate resources in the Capacity Planner </a>. </p> <p>It also allows you to:</p> 
    <ul> 
     <li>add new roles to the project</li> 
     <li>remove project from the Capacity Planner</li> 
     <li>edit some of the information on the project </li> 
     <li>Go to the project page</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip8.png" alt="mceclip8.png"></td> 
   <td>Hammer icon for the job role</td> 
   <td> <p>Allows you to automatically manage your resource. For more information about allocating resources to projects automatically, see <a href="../../resource-mgmt/legacy-res-planning/allocate-resources-in-capacity-planner.md" class="MCXref xref">Allocate resources in the Capacity Planner </a>. </p> <p>You can also remove the job role from the project from here, if it is not associated with a task. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip9.png" alt="mceclip9.png"></td> 
   <td> Planned Hours</td> 
   <td>Display the Planned Hours associated with the tasks assigned to the job roles on each project. This field is not editable in the Capacity Planner.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip10.png" alt="mceclip10.png"> </td> 
   <td> Projected Hours</td> 
   <td> <p>Display the Projected Hours associated with the tasks assigned to the job roles on each project. This field is not editable in the Capacity Planner. </p> <p> <p>Note:  The Projected Hours take into account the real timeline of the project, and they are different than the Planned Hours of the tasks. Projected Hours are a calculation that Workfront makes using the Planned Hours of the tasks and the amount of hours that the task is delayed to determine when the task is most likely going to be completed.<br>For example, a task might have 10 Planned Hours, but it is 3 hours behind in starting. The Projected Hours are 13 hours in this case (10 Planned Hours + 3 Hours delay).</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip11.png" alt="mceclip11.png"> </td> 
   <td>Table icon</td> 
   <td> <p>Display the Net Remaining Resources in a table format.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/mceclip12.png" alt="mceclip12.png"> </td> 
   <td>Chart icon</td> 
   <td>Display the Net Remaining Resources in a chart format.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/legend-for-cap-planner.png" alt="legend_for_cap_planner.png"> </td> 
   <td> Show legend icon</td> 
   <td> <p>This explains the colors used in the Capacity Planner for the following fields:</p> 
    <ul> 
     <li>Planned Dates</li> 
     <li>Budgeted Allocations</li> 
     <li>Budgeted Outside Current Date Range</li> 
     <li>Exclude from Calculation</li> 
     <li>Planned Schedule</li> 
     <li>Projected Schedule</li> 
     <li>Overage</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

