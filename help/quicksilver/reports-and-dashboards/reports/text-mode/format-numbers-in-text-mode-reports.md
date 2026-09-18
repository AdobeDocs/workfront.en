---
product-area: reporting
navigation-topic: text-mode-reporting
title: Format numbers, currency and percentage values in text mode reports
description: Numeric values including currency can be configured to display in a variety of formats in reports and lists in Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/z96Rvp54iQcZxVWJ4Evoe1Qasl-VrEZ-IrVy11n9cDc
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
# Format numbers, currency and percentage values in text mode reports

<!-- Audited: 1/2025 -->

Numeric values including currency can be configured to display in a variety of formats in reports and lists in Adobe Workfront.

To modify the format of a numeric value, you must edit the **valueformat** line of your column.

For example, if you wanted to display the Budget column as $1000, the value format line would look like:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

For more information about applying conditional formatting in Workfront reports and lists using text mode, see [Use conditional formatting in Text Mode](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

You can format numbers using the following values for the `valueformat` line of your column:

| Example | `valueformat=` |
|---|---|
| 1234 |`doubleAsString`<br>or<br>`int` |
| 1,234 |`doubleAsInt` |
| $1,234 |`currencyStringCurrencyRounded` |
| 1234.56 |`doubleAsDouble` |
| $1,234.56 |`currencyStringCurrency` |
| 12% |`doubleAsPercentRounded` |
| 12.34% |`doubleAsPercent` |
| (1,234.56) |`doubleAsFinancial` |
| (1,234) |`doubleAsFinancialRounded` |

