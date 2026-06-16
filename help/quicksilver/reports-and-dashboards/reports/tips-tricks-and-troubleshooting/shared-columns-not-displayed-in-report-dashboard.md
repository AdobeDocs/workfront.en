---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Data from shared columns not displayed in dashboard reports
description: Data from shared columns does not display when the report is placed in a multiple column dashboard layout, but it does display on a single column layout. Line breaks are also overridden.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Data from shared columns not displayed in dashboard reports

## Problem

Data from shared columns does not display when the report is placed in a multiple column dashboard layout, but it does display on a single column layout. Line breaks are also overridden.

## Cause

Only columns marked as 

```
shortview=true
```

are included in the dashboard view of the report when the dashboard layout has the left/right split or the left/middle/right split set up.

## Solution

Access the view used in the report and open text mode. (For more information, see [Edit a view using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Label all columns in the report, including the columns used in a shared/merged column, with 

```
shortview=true
```

. The report columns will then display properly in the dashboard.
