---
product-area: reporting
navigation-topic: text-mode-reporting
title: Format dates in text mode reports
description: Dates can be configured to display in a variety of formats in reports and lists in Adobe Workfront. To establish a date format, you must modify the valueformat line of the text mode code in the column.
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-8gB8XDwLQTBCUsrex-PIAyxcF-rSPsoM2Gvw2EhTaU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
---
# Format dates in text mode reports

<!-- Audited: 1/2025 -->

Dates can be configured to display in a variety of formats in reports and lists in Adobe Workfront. To establish a date format, you must modify the `valueformat` line of the text mode code in the column.

`valueformat= [new date format]` For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

If you wanted to show the Planned Completion Date as *Mth, DD, Year*, the code would look like:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

For more information about applying conditional formatting in Workfront reports and lists using text mode, see [Use conditional formatting in Text Mode](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

You can format dates using the following `valueformat` text mode values:

| **Format** |Example&nbsp; |***valueformat=*** |
|---|---|---|
| MM/DD/YY |10/11/18 |`atDate` |
| MM/DD/YY Time |10/11/18 12:00pm |`longAtDate` |
| MM/DD/YY |10/11/18 |`shortAtDate` |
| Mth, DD, YR |Oct, 11, 2018 |`mediumAtDate` |
| DW, Mth, Day, YR |Mon, Oct, 11, 2018 |`partialAtDate` |
| DW, Mth, Day, YR Time |Mon, Oct, 11, 2018 12:00 pm |`fullAtDate` |
