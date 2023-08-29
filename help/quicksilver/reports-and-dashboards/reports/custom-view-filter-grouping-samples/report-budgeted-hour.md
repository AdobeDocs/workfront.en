---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Report: Budgeted Hour'
description: 'Report: Budgeted Hour'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
---
# Report: Budgeted Hour

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

When you want to share Budgeted Hour information with other users who do not have access to the Resource Planner, you can do so by building a Budgeted Hour report. You can then share the report with them.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>Budgeted Hours are updated every hour in the Adobe Workfront database. Refreshing the report does not necessarily refresh the hour information in it. You can view the time lapsed since the last update in the upper-right corner of every Budgeted Hour report. Refreshing the report refreshes the information in it only when there has been more than one hour since the last update.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Build a Budgeted Hour report

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner, then click&nbsp;**Reports**. 

1. Click&nbsp;**New Report > Budgeted Hour**.

   The default view is applied to the report.

1. (Optional) To make the report easier to read, click the **Budgeted Hours** column, then **Switch to Text Mode**, then change the 

   ```
   valuefield
   ```

   line to 

   ```
   valueexpreesion
   ```

   and enter the rounding expression.

   This rounds the number of Budgeted Hours to a number of decimals that you specify.

   For information about how to round a number in Workfront, see the article [Calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Optional)&nbsp;Click **Add Column** to add additional columns.
1. (Optional) To make the report easier to read, we recommend that you add a grouping to it. We suggest the following grouping:

   Click the **Groupings** tab, then do one or several of the following:

   1. Click&nbsp;**Add Grouping** and start typing "Project&nbsp;Name", then select it when it appears in the list.
   1. Click **Add Grouping** and start typing "Job&nbsp;Role Name", then select it when it appears in the list.
   1. Click **Add Grouping** and start typing **Allocation Date**, select it when it appears in the list, and then select the timeframe you want to group by from the **Group Dates by** field.

1. (Optional) Click&nbsp;**Filters** to add filters to the report.
1. (Optional)&nbsp;Click&nbsp;**Chart** to add a chart to the report.
1. Click&nbsp;**Save + Close**.

## Review the Budgeted Hour report

The following information is available in the Budgeted Hour report by default:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Project </td> 
   <td>This is the name of the project associated with the Budgeted Hour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Job&nbsp;Role</p> </td> 
   <td>This is the name of the job role associated with the Budgeted Hour. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">User</td> 
   <td>This is the name of the user associated with the Budgeted Hour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alloc. Date</td> 
   <td> <p>This is the Allocation Date. It is the first day (a Sunday) of the week for which you budgeted the hours.</p> <p>Tip:  <p>If a week spans for two months, this generates two rows in the report: one corresponding to the first day of the week (the Sunday of the week which is during the first month), and a second one corresponding with the first day of the second month (and which could be any day of the week.)</p> <p>For example, if you budget 8 hours for a user for the week of June 30 (Sunday) - July 6 (Saturday), the two rows show an Allocation Date of June 30, and July 1.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bud. Hours</td> 
   <td>These are the Budgeted Hours allocated to the User in the Resource Planner.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Bud. Hours</td> 
   <td>These are the Budgeted Hours allocated to the Job&nbsp;Role or the Project in the Resource Planner.</td> 
  </tr> 
 </tbody> 
</table>
