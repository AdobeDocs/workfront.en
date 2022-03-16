---
filename: task-progress-in-resource-grid
product-area: resource-management
navigation-topic: legacy-resource-planning
title: Display task progress on the Resource Grid
description: You can configure the Resource Grid to display the following visual indicators related to task progress:
---

# Display task progress on the Resource Grid

>[!IMPORTANT]
>
>The information in this article refers to functionality that is currently deprecated and will soon be removed from Workfront. For information about the current functionality for managing resources in Workfront, see the [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md) section.

## Overview of task progress

You can configure the Resource Grid to display the following visual indicators related to task progress:

* Hide planned work when tasks complete early.
* Highlight week blocks in pink when the task is going beyond its scheduled planned completion date.  
  The days after the Planned Completion Date are displayed in pink, and the pink continues to display through the projected completion date of the task. (While no hours are displayed for these days, the range will show.)  
  ![](assets/screen-shot-2013-11-05-at-8.22.03-am-350x58.png)  
  Without this option selected, users see the Resource Grid in its standard view:  
  ![](assets/screen-shot-2013-11-05-at-8.22.26-am-350x52.png)

* Bold the hours of any user who has a task with potential impact on the project.  
  Either the user has not recorded hours to the task, or the user has taken longer than was planned. The project manager can assess the schedule and make adjustments.

To configure the `Resource Grid` to display visual indicators related to task progress, see [Chart Options](../../resource-mgmt/legacy-res-planning/resource-grid-overview.md#chart-options).

## Overview of the icons in the Resource Grid

You can access the Resource Grid in the following locations:

* By going to the Legacy Resource Planning tab in the People area.
* By applying the Resource Grid View to a user report.  
  For more information about applying the Resource Grid View to a user report, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* From the Staffing tab of a project, when you view the Resource Grid for a specific project.

Depending where you are viewing the Resource Grid from, the icons may be slightly different.

The following icons are visible on both the Resource Grid accessible from the Legacy Resource Planning tab as well as on the Resource Grid View when applied to a user report:

| `Icon`  | `Name`  | `Function`  |
|---|---|---|
|  ![resource_grid_magnifing_glass.png](assets/resource-grid-magnifing-glass.png), ![resource_grid_zoom_in_2.png](assets/resource-grid-zoom-in-2.png)

|Zoom In |Changes the grid display by zooming in one level. |
|  ![resource_grid_zoom_out.png](assets/resource-grid-zoom-out.png), ![resource_grid__zoom_in_2.png](assets/resource-grid--zoom-in-2.png)

|Zoom Out |Changes the grid display by zooming out one level. |
|  ![resource_grid_open_expand.png](assets/resource-grid-open-expand.png), ![resource_grid_open_all_2.png](assets/resource-grid-open-all-2.png)

|Open (Expand) All |Opens the interface to display all users, their projects, and tasks. |
|  ![resource_grid_collapse_all.png](assets/resource-grid-collapse-all.png), ![resource_grid_collapse_all_2.png](assets/resource-grid-collapse-all-2.png)

|Close (Collapse) All | Closes or hides any user's open projects and tasks data.  |
|  ![resrouce_grid_preferences.png](assets/resrouce-grid-preferences.png), ![resource_grid_Preferences_2.png](assets/resource-grid-preferences-2.png)

|Preferences |Provides an interface to update the columns to be displayed in the user list, the Chart Options and the Date Range. |
|  ![resource_grid_fullscreen.png](assets/resource-grid-fullscreen.png), ![resource_grid_full_screen_2.png](assets/resource-grid-full-screen-2.png)

|Full Screen |Expands the Resource Grid to occupy the full width and height of the browser window.  |
|  ![resource_grid_export_to_excel.png](assets/resource-grid-export-to-excel.png), ![resource_grid_export_to_excel_2.png](assets/resource-grid-export-to-excel-2.png)

|Export to Excel |Exports the data displayed in the Resource Grid to a Microsoft Excel file.  |
|  ![resource_grid__view_mode.png](assets/resource-grid--view-mode.png)

|View Mode |Allows you to select whether all planned work should be displayed, or if remaining availability should be displayed in the grid view. |
|  ![resource_grid_data_type.png](assets/resource-grid-data-type.png)

|Data Type  |Allows you to select whether the data should display in Hours, FTE or Percent Allocation.  |
|  ![resource_grid_previous_3_months.png](assets/resource-grid-previous-3-months.png)

|Previous three months |Expands the Resource Grid data to include the previous three months of assignments. |
|  ![resource_grid_next_3_months.png](assets/resource-grid-next-3-months.png)

|Next three months |Expands the Resource Grid data to include the next three months of assignments. |
|  ![resource_grid_overage.png](assets/resource-grid-overage.png)

|Overage |Indicates that the user has at least one overage: they are allocated to more planned work than their schedule allows for.  |

## Overview of the Resource Grid colors

For more information about the Resource Grid colors, see [Overview of the colors in the Resource Grid](../../resource-mgmt/legacy-res-planning/colors-of-resource-grid.md).

## Overview of the Resource Grid timelines

The timeline shows the dates during which the user is allocated to a task or an issue. You can choose to see the Planned timeline, or the Projected timeline. For more information about choosing Planned vs Projected dates to display in the Resource Grid, see [View Planned or Projected work](../../resource-mgmt/legacy-res-planning/resource-grid-overview.md#viewing-planned-or-projected-work).

When there is an over allocation, the day of the allocation for that task or issue is displayed in red. Toggle between `Used Resources` and `Available Resources`. Using `Available Resources` displays over-allocations in red negative numbers.

![](assets/screen-shot-2014-777-15-at-9.34.46-am--1--350x187.png)

The Resource Grid truncates Planned Hours if a task is completed early. The user utilization page then displays the availability of the user for additional tasks or assignments. But keep in mind this does not change the timeline within a project or adjust your Work Breakdown Structure. You will have to make additional adjustments to your project schedule manually to indicate that tasks have completed earlier than planned.

## Timeline limitations for user allocation

There is a limitation of how many days display user allocation for the timeline of a task, issue, or project in the Resource Grid.  
If a task, issue, or project span more than 1,000 days, the `Resource Grid` shows allocation information only for 1,000 days starting from the planned start date of the task, issue, or project .  
All other days included in the timeline of the task, issue, or project in the `Resource Grid` appear as non-working days and therefore no allocation is calculated for those. 
