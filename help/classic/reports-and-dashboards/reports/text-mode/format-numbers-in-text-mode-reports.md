---
filename: format-numbers-in-text-mode-reports
product-area: reporting
navigation-topic: text-mode-reporting
title: Format numbers, currency and percentage values in text mode reports
description: Numeric values including currency can be configured to display in a variety of formats in reports and lists in Adobe Workfront.
---

# Format numbers, currency and percentage values in text mode reports

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Numeric values including currency can be configured to display in a variety of formats in reports and lists in&nbsp;Adobe Workfront.

To modify the format of a numeric value, you must edit the&nbsp;**valueformat**&nbsp;line of your column.

For example, if you wanted to display the Budget column as $1000, the value format line would look like:
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>For more information about applying conditional formatting in Workfront reports and lists using text mode, see [Use conditional formatting in Text Mode](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

You can format numbers&nbsp;using the following values for the&nbsp;

```
valueformat
```

&nbsp;line of your column:

| **Example** |*

```
valueformat=
```

* |
|---|---|
| 1234 |<pre>doubleAsString</pre> or <pre>int</pre> |
| 1,234 |<pre>doubleAsInt</pre> |
| $1,234 |<pre>currencyStringCurrencyRounded</pre> |
| 1234.56 |<pre>doubleAsDouble</pre> |
| $1,234.56 |<pre>currencyStringCurrency</pre> |
| 12% |<pre>doubleAsPercentRounded</pre> |
| 12.34% |<pre>doubleAsPercent</pre> |
| (1,234.56) |<pre>doubleAsFinancial</pre> |
| (1,234) |<pre>doubleAsFiancialRounded</pre> |

