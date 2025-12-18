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