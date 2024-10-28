---
content-type: reference
product-area: reporting;projects
keywords: calculated,aggregates,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Grouping: Display the Result of Aggregating Multiple Calculated Values in a Grouping'
description: You can use text mode in a column to display a calculation between two fields in the view of a report or list. Each line displays the calculation for each object in the report or list.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
---
# Grouping: display the result of aggregating multiple calculated values in a grouping

<!--Audited: 10/2024-->

You can use text mode in a column to display a calculation between two fields in the view of a report or list. Each line displays the calculation for each object in the report or list.

For example, you can display the difference between Actual Hours and Planned Hours in a third column called Work Balance for each task in a task report. For more information about calculated data expressions, see [Overview of calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

You can display the aggregated value of multiple calculated view items in the same column in a grouping by adding a calculation to the `aggregator` line of the column that contains the calculated value. For example, you can aggregate (display the sum of) the amount of Work Balance hours of all the tasks in the grouping of the report or the list for the Work Balance column. This article describes how to do this.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
    <p>New:</p>
   <ul><li><p>Contributor to modify a filter </p></li>
   <li><p>Standard to modify a report</p></li> </ul>

   <p>Current:</p>
   <ul><li><p>Request to modify a filter </p></li>
   <li><p>Plan to modify a report</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Display the result of aggregating multiple calculated values in a grouping

1. Go to a task report, click **Report Actions** > **Edit**.
1. In the **Groupings** tab, click **Add grouping**, and start typing **Project Name** in the **Group by** field, then select **Project > Name** it when it displays in the list. 

1. In the **Columns(View)** tab, click **Add Column**, then start typing **Planned Hours** in the **Show in this column** field, then select it when it displays in the list.

   >[!TIP]
   >
   >Always start adding as much information using the Standard interface before you edit information in text mode. Add fields that are closest to or contain the most amount of information that for the calculation you are trying to make.

1. In the **Summarize this column by** field, select **Sum**. 
1. Click **Switch to Text Mode** in the column you added, then click **Edit Text Mode**. 
1. Replace the text in the box with the following text mode example:

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >In order to get the aggregated value in the grouping to display the aggregated difference between the Planned Hours and Actual Hours fields, input the same equation into the `aggregator.valuefield` line. The `aggregator.displayformat` used for the Planned Hours column converts minutes to hours. Because the Planned Hours field was used as a placeholder, this line doesn't need to be adjusted.
   >
   >
   >The `minutesAsHoursString` definition of the `aggregator.displayformat` line means there is no need to divide each field by 60 as done on the `valueexpression` for the results. In this `aggregator.valuefield=workRequired` becomes: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.
1. Click **Done**.
1. Click **Save+Close**.
