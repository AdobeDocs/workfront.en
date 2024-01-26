---
title: View the Resource capacity visualization in Enhanced analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: You can assess whether a team is over, under, or at capacity when viewing the Enhanced analytics resource capacity visualization chart in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
---
# View the Resource capacity visualization in Enhanced analytics

You can assess whether a team is over, under, or at capacity when viewing the Enhanced analytics resource capacity visualization chart in Adobe Workfront. 

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront plan</a>*</td> 
   <td> <p>Current: Business or higher</p>
   Or
   <p>New: Any</p>
    </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license*</td> 
   <td> <p>Current: Review or higher</p>
   Or
   <p>New: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>View access to Projects</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permission on a project</p>  </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Prerequisites

For prerequisites to using Enhanced Analytics, see the "Prerequisites" section in [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## Understand the Resource capacity chart

The Resource capacity chart shows whether a team is over, under, or at capacity. This calculation is based on:

* **Available capacity**: The total amount of hours a home team has available to work in the filtered period of time

  >[!NOTE]
  >
  >If you are looking at a future time period, the available capacity is calculated based on the team's capacity for the last 7 days. For this reason, any scheduled PTO is not taken into account.

* **Planned capacity**: The total amount of planned hours of work expected from the home team in the filtered period of time

This comparison of a home team's planned hours and actual scheduled hours can help you determine if you're not assigning enough work to the home team or if they may be experiencing burnout from a heavy workload.

![](assets/resource-capacity-350x110.png)

On the Resource capacity visualization, you can see the following details:

* **Planned capacity**: Inline with a home team name, the blue circle represents the number of planned hours assigned to the home team.

  ![](assets/resource-capacity-blue-circle.png)

* **Actual capacity**: Inline with a home team name, the vertical line represents the number of hours available for the home team.

  ![](assets/resource-capacity-vertical-line.png)

* **Over capacity**: When the horizontal line and the blue circle display to the right of the vertical line, the home team was assigned more work than they can complete in the number of available hours. This means that the team may be over capacity for the filtered time period. The remaining number of hours the team needs to complete displays to the right of the blue circle.

  ![](assets/resource-capacity-over-capacity.png)

* **Under capacity**: When the horizontal line and the blue circle display to the left of the vertical line, the home team has more available hours than the number of planned hours of work they were assigned. This means that the team may be under capacity for the filtered time period. The additional number of available hours for the home team to complete work displays to the left of the blue circle.

  ![](assets/resource-capacity-under-capacity.png)

Hovering over a row shows the exact number of hours for planned capacity and available capacity, as well as the number of hours the home team is over or under capacity.

Seeing this information helps you determine:

* If the home team was overallocated or underallocated.
* What the largest projects were that the home team was focused on.
* Which home teams are available for work.

To learn how to get the best data for this visualization, see [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## View the Resource capacity visualization

1. Click the Main Menu icon ![](assets/main-menu-icon-16x12.png), then select **Analytics**.
1. In the left panel, select **People**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Optional) To use a different date range, select new start and end dates from the date range filter.

   ![](assets/filters-select-date-range-350x344.png)

   For information on using the date range filter, see [Apply filters in Enhanced analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Conditional) If you haven't set your Team filter, add the Team filter and select each team that you want to see data for.

   For more information on adding filters in Enhanced analytics, see [Apply filters in Enhanced analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of Workfront.

1. (Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.

   All other visualizations update to the same date range and a timeframe filter is created.

   ![](assets/timeframe-filter-350x220.png)

1. Hover over the home team line to see how many hours are still available to be scheduled, the amount of hours planned for the home team to complete, and the total number of hours worked, which is labeled as over, under, or at capacity.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Optional) To export the visualization data, click the **Export icon** ![](assets/export.png) in the top-right corner of the visualization, then select the export format:

   * **Chart (PNG)** 
   * **Data Table (XSLX)**

1. Click a home team name to see more information in the Team capacity visualization.

   To learn more about the Team capacity visualization, see [View the Team capacity visualization in Enhanced analytics](../enhanced-analytics/team-capacity-overview.md).


