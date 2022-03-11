---
filename: view-calculation-between-two-fields
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: View: display the result of a calculation between two fields in a column
description: You can use text mode in a column to display a calculation between two fields.
---

# View: display the result of a calculation between two fields in a column

You can use text mode in a column to display a calculation between two fields.

For example, if you want to find out the number of week days that elapsed between two dates, you can use text mode syntax and data expressions to calculate this difference.  
For example, you can calculate the week day difference between the Planned Completion Date and the Actual Completion Date of a task and display the result in a column.

You can use any other two dates in this calculation (Actual Start, Actual Completion, Projected Start, Projected Completion, etc).  
For more information about calculated data expressions, see [Calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Display the result of a calculation between two fields in a column

To add this column to a task view:

1. Go to a list of tasks.
1. From the `View` drop-down menu, click `New View`.

1. Click `Add Column`, then `Switch to Text Mode`.

1. Hover over the text mode area, and click `Click to edit text`.
1. Remove the text you find in the `Text Mode` box, and replace it with the following code:
   <pre>displayname=Week Day Difference<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (Optional) To aggregate the values displayed in the view in a grouping, follow the steps described in [Grouping: display the result of aggregating multiple calculated values in a grouping](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Click `Save`, then `Save View`.

