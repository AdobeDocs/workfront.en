---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF statements overview
description: You can use "IF" statements in general programming languages. In Adobe Workfront, "IF" statements allow you to compare, format, and string together fields of data for both reporting and custom data purposes. Also, thinking mathematically about "IF" statements leads to a better conceptual understanding since variables for expressions are commonly used.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
---
# "IF" statements overview

You can use "IF" statements in general programming languages. In Adobe Workfront, "IF" statements allow you to compare, format, and string together fields of data for both reporting and custom data purposes. Also, thinking mathematically about "IF" statements leads to a better conceptual understanding since variables for expressions are commonly used.

## Recommendations for "IF" statements

Consider the following before creating an "IF" statement:

* We recommend a basic understanding of any general programming language, but we do not require it, for this guide.
* We require an advanced understanding of the Workfront text mode syntax. This helps with grasping the terminology of the Workfront API and with understanding the syntax of custom data in these specific formats.

  For information about the Workfront API, see [API basics](../../../wf-api/general/api-basics.md).

  For information about using text mode, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* You can build "IF" statements for the following Workfront elements:

   * Views
   * Groupings
   * Calculated custom fields

* You cannot build "IF" statements for filters. This results in a "Whoops" error in Workfront.
* The Support Team does not help with building custom data. You can contact the Support Team after you build the custom fields or columns and you are not seeing the desired results. For help building an expression, please contact your Account Executive to inquire about our consulting options.
* We recommend writing these expressions in a text editor first, such as Sublime or Visual Studio Code, because this helps you see data more clearly than would appear in Workfront.

## Components of an "IF" statement

You can build "IF" statements in Workfront using the following format:  
<pre>IF(Condition,True Expression,False Expression)</pre>The components of an "IF" statement are: 

* **IF**= This is the Workfront calculated data expression for "function." Similar to the SUM and PROD expressions, this first tells the system to understand the function as an "IF" statement. Always use capital letters for "IF" in this statement.  
  For a list of all calculated data expressions, see [Overview of calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condition**= This is the condition that the Workfront variable must meet and it is the foundation for this equation. Everything that can be later specified in the equation depends on the condition. You can use a number of references, comparisons or mathematical expressions to start an equation. Some examples of conditions are:

   * A date is greater than another date on a specified object.
   * A status equals one of the available statuses on a specified object.
   * Percent complete of a task is lesser than or greater than a certain percentage. 

* **Condition Operator** = this is the operator that helps you build the condition of your "IF" statement. For example, "is equal to" or "is greater than" are condition operators. For a list of condition operators that you can use in statements, see [Condition operators in calculated custom expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md). 

* **True****Expression**= This is the "True" variable, which tells the equation which indicator to display once the criteria of the condition are met (true indicators).

* **False Expression**= This is the "False" variable, which tells the equation which indicator to display when the criteria of the condition are not met (false indicators).

In the following example, the original statement format is used to write a simple data expression for an "IF" statement. The expression compares two different date fields in Workfront followed by a True/False result as a data string:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

In everyday speech, this statement would mean: If the Projected Completion Date of my object is "Greater Than" the Planned Completion Date of my same object, then display the words "Off Track" in this field. If not, display the words "On Track."

## Build calculated fields in custom forms or custom columns using "IF" statements

You can build "IF" statements in a calculated field either in a custom form, or in a custom column.

There is a difference in the syntax you use in a calculated custom form vs a calculated custom column. Refer to the following examples:

* [Single "IF" statements](#single-if-statements) 
* [Multiple "IF" statements](#multiple-if-statements)

### Single "IF" statements {#single-if-statements}

The following are examples of a calculated custom field and its corresponding column using an "IF" statement:

* Calculated custom field:

When building a custom field, use the following syntax for an "IF" statement:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Calculated custom column:

When building a custom column, you should use the following syntax for the "IF" statement in the value expression line:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Multiple "IF" statements {#multiple-if-statements}

You can put together multiple "IF" statements with the following statement to build a more complex and dynamic expression:  

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression))</pre>Notice, there is now no false statement for the first "IF". Instead, we replaced it with the start of a second "IF".

The following are examples of a calculated custom field and its corresponding custom column using multiple "IF" statements:

* Calculated custom field:  
  
  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Calculated custom column:  
 
 ```
 valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
 ```

In this example, the same thing has been accomplished by putting two different criteria variables together.  
You can further explore these options by rebuilding these examples in your own environment.

The best way to learn this is by experimenting with various fields and scenarios. Also, become familiar with the API Explorer, which reveals the field names that can be used. For information on the API Explorer, see [API Explorer](../../../wf-api/general/api-explorer.md).

For more information about Workfront syntax of calculated data expressions, see [Overview of calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
