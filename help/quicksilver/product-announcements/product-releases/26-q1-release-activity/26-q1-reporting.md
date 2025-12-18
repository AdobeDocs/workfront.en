---
title: First Quarter 2026 Reporting enhancements
description: First Quarter 2026 Reporting enhancements
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog

---
# First Quarter 2026 Reporting enhancements

This page describes Reporting enhancements made with the First Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the First Quarter 2026 release cycle, see [First Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

<!--

## Currency updates in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have made the following updates for currency fields:

* When multiple currencies are defined in Workfront, you can now choose a default currency for the dashboard during creation. 

* When creating a report, you can lock a currency field. This ensures that the dashboard-level currency preference does not affect the display of these values.

* When viewing a dashboard, users can toggle between any defined currencies in Workfront. These changes apply to the entire dashboard with the exception of locked currency fields.

-->

<!--

## Quick search table results in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have added a quick search to Table reports. This search works across all pages, so you can find data even if it's not currently visible.

-->

## New Show total option for Pie Charts

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have introduced a new Show total option that converts pie charts into donut charts. This feature allows users to display a central value that represents the total of all segments in the chart.

* For count aggregation types, the center value displayed is a count of all segments of the chart. 
* For sum aggregation types, the center value displayed is the aggregated total of the numeric or currency value. 
* For average, max, and min aggregation types, the center value displays the average, maximum, or minimum value accordingly. 

Users also have the option to show or hide a label for the total and provide a custom label value.

For more information, see [Build a chart report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## New configuration options for Pie Charts in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have introduced two new configuration options for Pie Charts: 

* Hide segment labels: You can now choose to hide segment labels on a Pie Chart if they are too long and impact chart readability. 
* Hide and reposition chart legend: You can now choose to hide a Pie Chart legend. You can also set the position of the legend to the right (default), left, top, or bottom of the chart.

For more information, see [Build a chart report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## Canvas Dashboards grouping count improvements

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We've updated the grouping bar in Canvas Dashboards to display the record count for the current page and the overall record count for the grouping across all pages.

For example, the grouping bar will show "3 of 7" or "83 of 21032" to provide a clear view of the data distribution within the grouping.

Previously, the grouping bar did not provide this detailed count information, making it challenging to understand the total number of records within a grouping when navigating through multiple pages.

## New Reference Line feature in Reports in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

You can now define a Reference line in Bar, Column, and Line charts to set a target or threshold four your series-based reports. 

Note: The Reference line is not dynamic and multiple reference lines cannot be applied. We are exploring future enhancements, but there are no immediate plans in place.

For more information, see [Build a chart report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## Customize axis labels on Chart reports in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

You can now customize the axis labels on Chart reports. This new feature allows you to input a replacement axis label to display instead of the default object and field path. Additionally, you can choose to hide the axis labels entirely.

For more information, see [Build a chart report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## Duplicate a report in a Canvas Dashboard

>[!NOTE]
>
>Preview release: October 23, 2025
>Production for all customers: October 23, 2025
>[!BADGE Off schedule]{type=Neutral}

You can now duplicate a KPI, table, or chart report in a Canvas Dashboard after it's been created. Once duplicated, you can edit the report as needed before saving.

## Removing field options from report filters

>[!NOTE]
>
>Preview: November 6, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

We have removed the following field options that were previously available when applying a filter to a report:

* Other Groups IDs
* Other Roles IDs
* Other Teams IDs

These were removed due to issues associated with the Not Equal and Is Blank operators. If you have an existing filter that uses one of these fields, it will continue to work as expected. Alternatively, you can continue using these fields in <code>textmode</code>, but it's recommended to avoid using the Not Equal or Is Blank operators when doing so.

The following field options are available as alternatives:

* Other Groups: ID
* Other Roles: ID
* Other Teams: ID

## Improved display of grouping count in Canvas Dashboards

>[!NOTE]
>
>Preview: November 6, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

When a table report has multiple pages of results and the table is configured with groupings, the table now displays both the record amount for the current page and the overall record count for all pages. For example, if your table report has 7 groupings and the first page shows 3, the table will display 3 of 7.


## New guardrails to improve loading times in Canvas Dashboards

>[!NOTE]
>
>Preview: November 6, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

To avoid loading time delays and improve overall performance in Canvas Dashboards, we have applied limits on how many dashboard components can be added to a dashboard:

* Reports per dashboard: 25 limit
* Groupings on table views: 5 limit
* Distance from the report's base object: 10 limit
* Columns on a table view: 25 limit
* Dashboard-level filter prompts: 10 limit




