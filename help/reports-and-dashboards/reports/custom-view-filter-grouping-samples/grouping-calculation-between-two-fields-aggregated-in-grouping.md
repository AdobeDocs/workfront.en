---
filename: grouping-calculation-between-two-fields-aggregated-in-grouping
content-type: reference
product-area: reporting;projects
keywords: calculated,aggregates,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: Grouping: display the result of aggregating multiple calculated values in a grouping
description: You can use text mode in a column to display a calculation between two fields in the view of a report or list. Each line displays the calculation for each object in the report or list.
---

# Grouping: display the result of aggregating multiple calculated values in a grouping

You can use text mode in a column to display a calculation between two fields in the view of a report or list. Each line displays the calculation for each object in the report or list.

For example, you can display the difference between&nbsp;Actual Hours and Planned Hours in a third column called Work Balance for each task in a task report. For more information about calculated data expressions, see [Calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

You can display the aggregated value of multiple calculated view items in the same column in a grouping by adding a calculation to the 

```
aggregator.
```

line of the column that contains the calculated value. For example, you can aggregate (display the sum of) the amount of Work Balance hours of all the tasks in the grouping of the report or the list for the Work Balance column. This article describes how to do this.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Display the result of aggregating multiple calculated values in a grouping

<ol> 
 <li value="1"> <p>Go to a task report, click <span class="bold">Report Actions</span> >&nbsp;<span class="bold">Edit</span>.</p> </li> 
 <li value="2">In the <span class="bold">Groupings</span> tab, click <span class="bold">Add Grouping</span>, and start typing <span class="bold">Project Name</span> in the <span class="bold">Group your Report</span> > <span class="bold">First by</span> field, then select it when it displays in the list. </li> 
 <li value="3"> <p>In the <span class="bold">Columns(View)</span> tab, click <span class="bold">Add Column</span>, then start typing <span class="bold">Planned Hours</span> in the <span class="bold">Show in this column</span> field, then select it when it displays in the list.</p> <note type="tip">
   Always start adding as much information using the Standard interface before you edit information in text mode. Add fields that are closest to or contain the most amount of information that for the calculation you are trying to make. 
  </note> </li> 
 <li value="4">In the <span class="bold">Summarize this column by</span> field, select <span class="bold">Sum</span>, then click <span class="bold">Done</span>.</li> 
 <li value="5">Click <span class="bold">Switch to Text Mode</span> in the column you added. </li> 
 <li value="6">Hover over the text mode area, and click <span class="bold">Click to edit text</span>.</li> 
 <li value="7"> <p>Replace the <code>valuefield.</code> and the <code>aggregator.valuefield.</code> lines with the lines highlighted in the following text mode example: </p><pre>valueformat=compound<br>aggregator.displayformat=minutesAsHoursString<br><span style="font-weight: normal;">aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)</span><br>aggregator.function=SUM<br>aggregator.valueformat=val<br>aggregator.namekey=workrequired<br>linkedname=direct<br>textmode=true<br>valuefield=workRequired<br>namekey=workrequired<br>valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours")
viewalias=workrequired<br>displayname=Work Balance<br><br></pre> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>In order to get the aggregated value in the grouping to display the aggregated difference between the Planned Hours and Actual Hours fields, input the same equation into the <code>aggregator.valuefield</code> line. The <code>aggregator.displayformat</code> used for the Planned Hours column converts minutes to hours. Because the Planned Hours field was used as a placeholder, this line doesn’t need to be adjusted.</p> 
   <p>The <code>minutesAsHoursString</code> definition of the <code>aggregator.displayformat</code> line means there is no need to divide each field by 60 as done on the <code>valueexpression</code> for the results. In this <code>aggregator.valuefield=workRequired</code> becomes: <code>aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2</code>. </p> 
  </div> </li> 
 <li value="8">Click <span class="bold">Save+Close</span>.</li> 
</ol>

&nbsp;

