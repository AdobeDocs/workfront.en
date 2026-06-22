---
title: Third Quarter 2026 Reporting enhancements
description: Third Quarter 2026 Reporting enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Third Quarter 2026 Reporting enhancements

This page describes Reporting enhancements made with the Third Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Third Quarter 2026 release cycle, see [Third Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Add multiple Power BI IP address ranges to the Data Connect allowlist at once

>[!NOTE]
>
>Preview: N/A
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Workfront administrators connecting Microsoft Power BI to Workfront Data Connect can now add an entire region's set of Azure IP address ranges to the allowlist in a single step. On the **IP Allowlist** tab in **Data Connect**, the **New IP address** button now includes an **Add Power BI IP address blocks** option that opens a dialog where you can paste Power BI service tag entries from Microsoft's published Azure IP Ranges and Service Tags JSON file.

This replaces the previous workflow of adding each Power BI CIDR block one at a time, which was time-consuming for regions that publish dozens of address prefixes.

For more information, see [Establish a connection to Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).


## Sort the Canvas Dashboards list

>[!NOTE]
>
>Preview: June 11, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>Canvas Dashboards is currently in beta.

You can now sort the Canvas Dashboards list by any of the following columns: **Name**, **Description**, **Created by**, or **Create date**. Click a column header to sort the list by that column, then click the same header again to reverse the sort direction. By default, the list is sorted by **Name** from A to Z. Your sort order is preserved when you switch between tabs in the Canvas Dashboards list.

For more information, see [Use Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Changes to Actual Hours in custom formulas

>[!NOTE]
>
>Preview: June 1, 2026
>Production fast release: June 1, 2026
>Production for everyone: June 1, 2026

In 2025, a new Actual Hours field was added to the Workfront database as `actualWorkRequiredDouble`, and the existing Actual Hours field (`actualWorkRequired` in the database) was renamed Legacy Actual Hours. See the [release note](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md) for more information.

In June 2026, existing custom formulas using `actualWorkRequired` (Legacy Actual Hours) were migrated to use `actualWorkRequiredDouble` (Actual Hours) instead. `actualWorkRequired` can no longer be used in calculations and formulas.

Also, it is strongly recommended to use `actualWorkRequiredDouble` in all reports.

When replacing the field, note that `actualWorkRequired` stores values in minutes, whereas `actualWorkRequiredDouble` stores values in hours with decimal precision.

For more information on Actual Hours, see [View Actual Hours](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

## Custom currency data fields in Canvas Dashboard reports

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Canvas Dashboard reports now support custom currency data fields as columns, filters, groupings, and aggregations, including when multiple exchange rates are configured in System Setup. When a custom currency data field is shown as a column or aggregation, values convert to the currency selected in the dashboard's exchange rate toggle, unless the field is locked at the report level.

Reports that previously failed with a "restricted field" message after a second exchange rate currency was added now render. Planning currency fields remain restricted when multiple exchange rates are defined.

For more information, see [Use currency fields in Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Improved data accuracy in Canvas dashboard reports

>[!NOTE]
>
>Preview: May 14, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026
>
>Canvas Dashboards is currently in beta.

Canvas dashboards now structure report queries to prevent duplicate rows when filters or fields cross related records, so counts, sums, and other aggregates return accurate values.

Previously, a join between related records could repeat parent records once for each related record. For example, in a project report filtered to tasks assigned to a specific user, each project repeated once for every matching task. A KPI that summed project budget could show $6,000 instead of the correct $1,250.

There are no changes to the Canvas dashboard interface. Existing reports automatically return accurate data after this release.
