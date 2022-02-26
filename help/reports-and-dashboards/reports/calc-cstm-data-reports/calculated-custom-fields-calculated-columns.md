---
filename: calculated-custom-fields-calculated-columns
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Calculated custom fields vs. calculated columns
description: To aggregate several fields in Adobe Workfront and display that aggregate value in a new field, you can do the following:
---

# Calculated custom fields vs. calculated columns

To aggregate several fields in *Adobe Workfront* and display that aggregate value in a new field, you can do the following:

* A calculated custom field in a Custom Form  
  For more information about adding a calculated custom field to a Custom Form, see the section [Add a calculated field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) in the article [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* A calculated column in a View  
  For more information about using calculations in a View, see the section [Use Text Mode in views](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) in the article [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Although you use text mode to build both calculated fields and calculated columns, the syntax for building them differs. Refer to the articles listed above to learn how to build calculated fields and calculated columns. For information about the different syntax used in calculated data expressions such as calculated custom fields and columns, see the [You can use the same calculations in both calculated fields as well as a calculated column. However, depending on what your purpose for these calculations is you might want to consider building one versus the other.](#syntax) section in this article.

You can use the same calculations in both calculated fields as well as a calculated column. However, depending on what your purpose for these calculations is you might want to consider building one versus the other.

## The syntax of calculated custom fields vs the syntax of calculated custom columns

Although the data expressions used are the same, the syntax for building a calculated custom field is different than that of building a calculated custom column.

For example:

<ul> 
 <li> <p>To add a calculated data expression to a custom field on a task form for the Project Name, you use the following text: </p> <p><code>Project.Name</code> </p> </li> 
 <li> <p>To add a calculated data expression to a custom column on a task report for the Project Name, you use the following text:</p> <p><em><code>valuefield=project:name</code></em> </p> <p>Or<br></p> <p><code>valueexpression={project}.{name}</code> </p> <note type="tip">
   The same syntax applies to all text-mode reporting elements where calculated expressions are used: views, filters, groupings, prompts. 
  </note> </li> 
</ul>

The differences between the two syntaxes are: 

<table cellspacing="3"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Calculated custom field</td> 
   <td>Calculated custom reporting element</td> 
  </tr> 
  <tr> 
   <td> <p>Use the name of the fields as they appear in&nbsp;the <em>Workfront</em> interface.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Example of field name used in a calculated custom field:&nbsp;<code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Use the name of the objects or fields as they appear in the <em>Workfront</em> database. The names of objects and fields are spelled in lower case or camel case, if they are compound names. </p> <p>For an inventory of all&nbsp;<em>Workfront</em> objects and fields as they appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Example of field name used in a calculated custom reporting element:&nbsp;<code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Do not enclose field names in parentheses or curly brackets.</td> 
   <td> <p>Do not enclose field names in brackets or parentheses when using them in a <code>valuefield </code>line.</p> <p>Enclose field names in curly brackets when using them in a <code>valueexpression</code> line.</p> </td> 
  </tr> 
  <tr> 
   <td>Separate the fields by periods.</td> 
   <td> <p>Separate the fields by colons when using them in a <code>valuefield </code>line</p> <p>Separate the fields by periods when using them in a <code>valueexpression </code>line. </p> </td> 
  </tr> 
 </tbody> 
</table>

For more information about the syntax you must use in a calculated custom column, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## When to use calculated custom fields

* When you want to group the aggregated results in a report or you want to show this information in a chart
* When you want to aggregate the data beyond the aggregation that is calculated in the field
* When you are not concerned about the timeliness of the data, as data is not updated and it might change over time

## Actions that trigger the update of a calculated custom field

<ul> <draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">On an object’s main page, clicking the More icon <img src="assets/more-icon.png">, then clicking <span class="bold">Recalculate Expressions</span></li>
 </draft-comment>
 <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">On an object’s main page, clicking the More icon <img src="assets/more-icon.png">, then clicking <span class="bold">Recalculate Expressions</span></li> 
 <li>Bulk editing multiple objects when <span class="bold">Recalculate Custom Expressions</span> is enabled</li> 
 <li>Editing a custom form when <span class="bold">Update previous calculations</span> is enabled for the calculated custom field</li> 
</ul>

## When to use Calculated Columns in a View

<ul> 
 <li> <p>When you want real-time data to be available on a report.</p> <p>Calculated views are always fresh because the calculation is made when the report is run or the view is applied.</p> </li> 
 <li>When you have no plans to group by aggregated results nor use this information in a chart.</li> 
 <li>When you do not plan to aggregate the data beyond the aggregation that is calculated in the column (data can be aggregated only once).</li> 
 <li> <p>When you want the calculation to include a reference to the current date using the $$TODAY or $$NOW wildcards.</p> <note type="tip">
   Do not use this reference in calculated custom fields because they only recalculate when the attached object is edited. These types of calculations become outdated.
  </note> </li> 
</ul>

## Examples of calculated custom fields and columns

For examples of calculated custom fields, see [Calculated custom data in reports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

For examples of calculated custom columns in views see the following articles:

* [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md) 
* [Custom View, Filter, and Grouping samples](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

