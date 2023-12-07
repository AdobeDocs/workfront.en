---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Condition operators in calculated custom expressions
description: You can use condition operators or modifiers when building calculated custom data in Adobe Workfront when using text mode.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
---
# Condition operators in calculated custom fields

You can use condition operators or modifiers when building calculated custom data in Adobe Workfront when using text mode.

For information about using text mode in&nbsp;Workfront, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Condition operators or modifiers help build a condition statement by connecting existing Workfront fields in statements and generating a new field. The most common use of condition operators is to build the condition of an "IF" statement.

You can use "IF" statements in Workfront to compare, format, and string together fields of data for both reporting and custom data purposes.

You can build "IF" statements for the following Workfront elements:

* Views
* Groupings
* Calculated custom fields

For more information about building "IF" statements, see ["IF" statements overview](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

The examples in this guide illustrate the use of condition operators in calculated custom fields. You can also use them in calculated custom columns or groupings as well, when following the correct syntax for calculated custom fields in reports.

For information about the difference in syntax between the calculated custom fields and calculated custom data in reports, see [Calculated custom fields vs. calculated columns](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Refer to the API Explorer to find the fields you want to reference in your calculated custom expressions. For information about the API Explorer, see [API Explorer](../../../wf-api/general/api-explorer.md).

You can use the following condition modifiers in Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Condition operator</th> 
   <th>Condition operator syntax</th> 
   <th>Condition operator definition</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Equal</td> 
   <td>= </td> 
   <td> <p>Use this operator to indicate that the condition is fulfilled when the first field of your statement is equal to the second field.</p> <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</pre> </td> 
  </tr> 
  <tr> 
   <td>Greater than </td> 
   <td>&gt; </td> 
   <td>Use this operator to indicate that the condition is fulfilled when the first field of your statement is greater than the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</pre></td> 
  </tr> 
  <tr> 
   <td>Greater than or equal to </td> 
   <td>&gt;= </td> 
   <td>Use this operator to indicate that the condition is fulfilled when the first field of your statement is either greater than or equal to the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</pre></td> 
  </tr> 
  <tr> 
   <td>Lesser than </td> 
   <td>&lt; </td> 
   <td>Use this operator to indicate that the condition is fulfilled when&nbsp; the first field of your statement is lesser than the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</pre></td> 
  </tr> 
  <tr> 
   <td>Lesser than or equal to </td> 
   <td>&lt;= </td> 
   <td>Use this operator to indicate that the condition is fulfilled when&nbsp; the first field of your statement is lesser than or equal to the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</pre></td> 
  </tr> 
  <tr> 
   <td>Does not </td> 
   <td>! </td> 
   <td> <p>Add this operator in front of any of the above operators to negate the operator. </p> <p>For example: </p> 
    <ul> 
     <li>Equals: = </li> 
     <li>Does not equal: != </li> 
    </ul> <p>Adding this operator in front of the following data expressions adds a negative statement to expressions: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>For information about these data expressions and for a complete list, see <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Overview of calculated data expressions</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Or </td> 
   <td>|| </td> 
   <td> <p>Use this operator to indicate that the condition is fulfilled when the expression&nbsp; finds either the first or the second value of your statement. </p> <p>For example, use the following statement in a calculated custom field to build an "IF" statement that marks projects in either the Current or Planning statuses as "Active": </p><pre>IF({status}="PLN"||{status}="CUR","Active","Not Active")</pre> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;And </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Use this operator to indicate that the condition is fulfilled when the expression&nbsp; finds an item that fulfills two conditions at the same time. </p> <p>For example, use the following statement in a calculated custom field to build an "IF" statement that finds projects that are in Current status and have a Condition of At Risk and marks them as "Mediation Needed." </p><pre>IF({status}="CUR"&&{condition}="AR","Mediation Needed",""))</pre> </td> 
  </tr> 
 </tbody> 
</table>
