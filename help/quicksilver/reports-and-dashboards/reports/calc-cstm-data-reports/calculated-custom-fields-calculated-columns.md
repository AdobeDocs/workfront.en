---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Calculated custom fields vs. calculated columns
description: To aggregate several fields in Adobe Workfront and display that aggregate value in a new field, you can create a calculated custom field in a custom form or a calculated column in a view.
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
---
# Calculated custom fields vs. calculated columns

To aggregate several fields in Adobe Workfront and display that aggregate value in a new field, you can create the following:

* A calculated custom field in a custom form  
  For more information about adding a calculated custom field to a custom form, see the section [Add a calculated field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#add-a-calculated-field-to-a-custom-form) in the article [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* A calculated column in a view  
  For more information about using calculations in a view, see the section [Use Text Mode in views](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) in the article [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Although you use text mode to build both calculated fields and calculated columns, the syntax for building them differs. Refer to the articles listed above to learn how to build calculated fields and calculated columns. For information about the different syntax used in calculated data expressions such as calculated custom fields and columns, see the section [Syntax of calculated custom fields vs. calculated custom columns](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in this article.

You can use the same calculations in both calculated fields as well as a calculated column. However, depending on what your purpose is for these calculations, you might want to consider building one versus the other.

## Syntax of calculated custom fields vs. calculated custom columns

Although the functions that you use are the same, the syntax for building an expression in a calculated custom field can be different than it is for  building a calculated custom column.

For example:

* In a custom field, on a custom form for tasks, you would use the following to generate the name of the parent project of the task where the custom form is attached:

  `{project}.{name}`

* In a custom column in a report, you would use the following to add a Project Name custom column on a task report:

  `valuefield=project:name`

  Or

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >The same syntax applies to all text-mode reporting elements where calculated expressions are used: views, filters, groupings, and prompts.

The differences between the two syntaxes are: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Calculated custom field</strong></td>
   <td><strong>Calculated custom reporting element</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Use the name of the fields as they appear in the Workfront interface.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Example of field name used in a calculated custom field: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Use the name of the objects or fields as they appear in the Workfront database. The names of objects and fields are spelled in lower case or camel case, if they are compound names. </p> <p>For an inventory of all Workfront objects and fields as they appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Example of field name used in a calculated custom reporting element: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Enclose field names in parentheses or curly brackets</td> 
   <td> <p>Do not enclose field names in brackets or parentheses when using them in a <code>valuefield </code>line.</p> <p>Enclose field names in curly brackets when using them in a <code>valueexpression</code> line.</p> </td> 
  </tr> 
  <tr> 
   <td>Separate the fields by periods</td> 
   <td> <p>Separate the fields by colons when using them in a <code>valuefield</code>line.</p> <p>Separate the fields by periods when using them in a <code>valueexpression</code>line.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more information about the syntax you must use in a calculated custom column, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## When to use calculated custom fields

* When you want to group the aggregated results in a report or you want to show this information in a chart
* When you want to aggregate the data beyond the aggregation that is calculated in the field
* When you are not concerned about the timeliness of the data, as data is not updated and it might change over time

## Actions that trigger the update of a calculated custom field

* On an object's main page, clicking the More icon ![](assets/more-icon.png), then clicking **Recalculate Expressions**

* Bulk editing multiple objects when **Recalculate Custom Expressions** is enabled
* Editing a custom form when **Update previous calculations** is enabled for the calculated custom field

## When to use calculated columns in a view

* When you want real-time data to be available on a report.

  Calculated views are always fresh because the calculation is made when the report is run or the view is applied.

* When you have no plans to group by aggregated results nor use this information in a chart.
* When you do not plan to aggregate the data beyond the aggregation that is calculated in the column (data can be aggregated only once).
* When you want the calculation to include a reference to the current date using the $$TODAY or $$NOW wildcards.

  >[!TIP]
  >
  >Do not use this reference in calculated custom fields because they only recalculate when the attached object is edited. These types of calculations become outdated.

## Examples of calculated custom fields and columns

For examples of calculated custom fields, see [Calculated custom data in reports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

For examples of calculated custom columns in views, see the following articles:

* [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md) 
* [Custom view, filter, and grouping samples: article index](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
