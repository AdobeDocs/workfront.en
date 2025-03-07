---
title: View the Flight plan visualization in Enhanced analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: The Flight plan visualization shows how many projects (within the applied filter criteria) were in flight, what condition changes happened throughout the life of these projects, and how closely these projects adhered to their planned completion deadlines.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
---
# View the Flight plan visualization in Enhanced analytics

>[!IMPORTANT]
>
>Enhanced Analytics will be removed from Workfront the week of May 26th. Workfront Data Connect is a new, alternative solution and can be used to replicate any Enhanced Analytics visualizations you currently use. <br>See the [Enhanced Analytics deprecation](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) guide for more information.


The Flight plan visualization shows how many projects (within the applied filter criteria) were in flight, what condition changes happened throughout the life of these projects, and how closely these projects adhered to their planned completion deadlines.

![Flight plan](assets/flight-plan-350x132.png)

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>Business or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to the project</p> <p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

For prerequisites to using Enhanced Analytics, see the "Prerequisites" section in [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## Understand the Flight plan visualization

In the actual duration of a project, you can see only the following project conditions:

* On Target
* At Risk
* In Trouble

To learn about project conditions, see [Overview of Project Condition and Condition Type](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

The Flight plan visualization shows the following project details:

* **Planned duration**: The horizontal blue line represents the planned length of the project, with the triangles at either end of the line indicating the start date and end date.

  ![Planned duration](assets/planned-duration-line-350x37.png)

* **Actual duration**: The thick, colored line below the planned duration represents the actual length of the project. The color of the line changes depending on the condition of the project at that particular time in the life of the project.

  ![Actual duration](assets/actual-duration-line.png)

* **Actual condition**: The thick, colored line also shows the condition of a project at different moments in time. The color of the line changes depending on the condition of the project:

   * **Green**: On Target
   * **Orange**: At Risk
   * **Red**: In&nbsp;Trouble

  ![Actual condition](assets/actual-condition-color.png)

By hovering over a project row in the Flight Plan visualization, you can see information about the project's planned timeframe, the current project condition, and—if applicable—the custom condition. To get a more in-depth view of what may have affected the duration or condition, you can look at the other visualizations in the Enhanced analytics area.

Seeing this information helps you determine:

* What events extend a project past the original planned completion date.
* When a project starts to run into issues.
* How many projects are open over the same time period.
* How many projects are active.
* Which projects need extra attention or support.

For information on how to get the best data for this visualization, see [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## View the Flight plan visualization

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon-16x12.png), then select **Analytics**.
1. (Optional) To use a different date range, select new start and end dates from the date range filter.

   ![Select date range](assets/filters-select-date-range-350x344.png)

   For information on using the date range filter, see [Apply filters in Enhanced analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Conditional) If you need to limit the project data set, select and apply the filters that you want to use.

   For more information on adding filters in Enhanced analytics, see [Apply filters in Enhanced analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of Workfront.

1. (Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.

   All other visualizations update to the same date range and a timeframe filter is created.

   ![Timeframe filter](assets/timeframe-filter-350x220.png)

1. (Optional) To change how the projects are sorted, click the **Sort by** menu in the upper-right corner of the Flight plan visualization, then select a new sorting option:

   * **A - Z** 
   * **Z - A** 
   * **Planned completion date** 
   * **Planned start date**

   All other visualizations on the page update to match your sorting selection.

1. (Conditional) If there are more than 50 projects in your data set, use the arrows in the bottom-left corner of the visualization to navigate from one group of 50 projects to the next.

   All other visualizations on the page update to match your page selection.

   ![Pagination](assets/pagination-350x118.png)

1. Hover over the project bar graph to see the blue date line, as well as the following details:

   * Planned timeline
   * Current condition
   * Custom condition (if applicable)

   ![Project bar graph](assets/project-bar-graph-350x143.png)

1. (Optional) To export the visualization data, click the **Export** icon ![Export icon](assets/export.png) in the top-right corner of the visualization, then select the export format:

   * **Chart (PNG)** 
   * **Data Table (XSLX)**

1. To see more project information, click a project on the visualization to open the Burndown and Tasks in flight visualizations.

   These visualizations can help you gain deeper insight into what caused the project to get off track. They also make it easy to check in on an in-progress project.  
   For more information on the Burndown visualization, see [View the Burndown visualization in Enhanced analytics](../enhanced-analytics/burndown-overview.md). For more information on the Tasks in flight visualization, see [View the Tasks in flight visualization in Enhanced analytics](../enhanced-analytics/tasks-in-flight-overview.md).

