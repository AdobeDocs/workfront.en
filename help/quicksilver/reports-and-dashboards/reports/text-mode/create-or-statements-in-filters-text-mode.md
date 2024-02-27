---
product-area: reporting
navigation-topic: text-mode-reporting
title: Create "OR" statements in text mode filters
description: You can include multiple statements when you create a filter in lists and reports.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
---
# Create "OR" statements in text mode filters

You can include multiple statements when you create a filter in lists and reports.

For information about creating filters, see the following articles:

* [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Text Mode filter operators

For information about Adobe Workfront filter operators in the standard filter interface, see [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront has 2 filter operators that connect each filter statement:

* **AND**: When you join 2 filter statement by the AND&nbsp;operator you indicate that you want both filter statements to be met at the same time.

  By default, the statements in a filter are joined by the AND&nbsp;operator.

  When building an AND filter in the text mode interface, you don't need to use the AND operator. It is assumed.

  **Example:** To filter for tasks that have a Planned Completion Date of Today and a Percent Complete lower than 100% use the following text mode code:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OR**: When you join 2 filter statements by the OR operator you indicate that you want either statement to be met.

  >[!TIP]
  >
  >When changing your AND statements to OR statements, the number of the items in your report should increase.

  When building an OR&nbsp;filter using the text mode interface, you must use the OR operator.

  **Example:** To filter for tasks that have a Planned Completion Date of Today or a Percent Complete lower than 100% use the following text mode code:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OR:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre>

## Text Mode syntax for OR filters

The text mode syntax for an OR filter must contain the following:

* The OR operator followed by a colon, a number, and another colon at the beginning of each filter line that refers to the object in the OR statement.&nbsp;This includes the line that references the filter field or attribute and the line that references the filter modifier.

  Follow this pattern when building an OR filter:

  <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>OR:1:<field name in camel case>=<value></pre><pre>OR:1:<field name in camel case>_Mod=<modifier value></pre>

  >[!TIP]
  >
  >The OR operator is case sensitive and it is always uppercase.

  You may have multiple OR statements in a filter. In this case, every OR statement receives a number, in the order you want the statements applied.

  **Example:**  To filter for tasks that have a Planned Completion Date of Today OR a Percent Complete lower than 100% OR a Status of New use the following text mode code:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OR:1:status=NEW</pre><pre>OR:1:status_Mod=in</pre><pre>OR:2:percentComplete=100</pre><pre>OR:2:percentComplete_Mod=lt</pre>

* The name of the fields or the attributes you reference in a filter must be written in camel case. For information about camel case, see [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* When you refer to custom fields in an OR filter, you must insert DE: between the OR modifier syntax and the name of the custom field. You must spell the name of the custom field as it appears in the Workfront interface.

  **Example:** To filter for tasks that have a Status of New OR a Percent Complete lower than 100% OR a custom field called "Account Type" with a value of "Equal", use the following text mode code:

  <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>OR:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre><pre>OR:2:DE:Account Type=Capital</pre><pre>OR:2:DE:Account Type_Mod=in</pre>
