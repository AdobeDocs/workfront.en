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
