---
filename: format-dates-in-text-mode-reports
product-area: reporting
navigation-topic: text-mode-reporting
title: Format dates in text mode reports
description: Dates can be configured to display in a variety of formats in reports and lists in Adobe Workfront. To establish a date format, you must modify the valueformat line of the text mode code in the column.
---

# Format dates in text mode reports

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Dates can be configured to display in a variety of formats in reports and lists in Adobe Workfront. To establish a date format, you must modify the 

```
valueformat
```

line of the text mode code in the column.
<pre>valueformat=&nbsp;[new date format]</pre>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate&nbsp;</pre>If you wanted to show the Planned Completion Date as *Mth, DD, Year*, the code would look like:
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>For more information about applying conditional formatting in Workfront reports and lists using text mode, see [Use conditional formatting in Text Mode](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

You can format dates using the following 

```
valueformat
```

&nbsp;text mode values:

| **Format** |Example&nbsp; |***valueformat=*** |
|---|---|---|
| MM/DD/YY |10/11/18 |<pre>atDate</pre> |
| MM/DD/YY Time |10/11/18 12:00pm |<pre>longAtDate</pre> |
| MM/DD/YY |10/11/18 |<pre>shortAtDate</pre> |
| Mth, DD, YR |Oct, 11, 2018 |<pre>mediumAtDate</pre> |
| DW, Mth, Day, YR |Mon, Oct, 11, 2018 |<pre>partialAtDate</pre> |
| DW, Mth, Day, YR Time |Mon, Oct, 11, 2018 12:00 pm |<pre>fullAtDate</pre> |

