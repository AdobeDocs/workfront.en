---
filename: report-on-budgeted-hours
product-area: resource-management;reporting
navigation-topic: resource-planning
title: Report on Resource Planner Budgeted Hours
description: You can budget resources on your projects by using the Resource Planner. For information about budgeting your resources using the Resource Planner, see the article Budget resources in the Resource Planner using the Project and Role views.
---

# Report on Resource Planner Budgeted Hours

You can budget resources on your projects by using the Resource Planner. For information about budgeting your resources using the Resource Planner, see the article [Budget resources in the Resource Planner using the Project and Role views](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Budgeting resources means that you define (or budget) a certain number of hours that the resources on a project need to complete their work on the project. To share the budgeted hour information that you enter in the Resource Planner with other users who might not have access to the Resource Planner, you can build a Budgdted Hour report. For information, see [Report: Budgeted Hour](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

<!--
When you want to share Budgeted Hour information with other users who do not have access to the Resource Planner, you can do so by building a Budgeted Hour report. You can then share the report with them.
-->

>[!IMPORTANT]
>
><!-->
>Budgeted Hours are updated every hour in the Adobe Workfront database. Refreshing the report does not necessarily refresh the hour information in it. You can view the time lapsed since the last update in the upper-right corner of every Budgeted Hour report. Refreshing the report refreshes the information in it only when there has been more than one hour since the last update.>
>-->
><!-->
>-->

  <!--
  Build a Budgeted Hour report
  -->

  <!--
  Review the Budgeted Hour report
  -->

<!--
Build a Budgeted Hour report
-->

   <!--
   Click the Main Menu in the upper-right corner, then click Reports.
   -->

1. 

   <!--
   Click New Report> Budgeted Hour.
   -->

   <!--
   The default view is applied to the report.
   -->

1. 

   <!--
   (Optional) To make the report easier to read, click the Budgeted Hours column, then Switch to Text Mode, then change the valuefield line to valueexpreesion and enter the rounding expression. This rounds the number of Budgeted Hours to a number of decimals that you specify.
   -->

   <!--
   For information about how to round a number in Workfront, see the article Condition operators in calculated custom expressions.
   -->

   <!--
   (Optional) Click Add Column to add additional columns.
   -->

1. 

   <!--
   (Optional) To make the report easier to read, we recommend that you add a grouping to it. We suggest the following grouping:
   -->

   <!--
   Click the Groupings tab, then do one or several of the following:
   -->

     <!--  
     Click Add Grouping and start typing "Project Name", then select it when it appears in the list.  
     -->

     <!--  
     Click Add Grouping and start typing "Job Role Name", then select it when it appears in the list.  
     -->  
  
  1. 
  
     <!--  
     Click Add Grouping and start typing Allocation Date, select it when it appears in the list, and then select the timeframe you want to group by from the Group Dates by field.  
     -->

   <!--
   (Optional) Click Filters to add filters to the report.
   -->

   <!--
   (Optional) Click Chart to add a chart to the report.
   -->

   <!--
   Click Save + Close.
   -->

<!--
Review the Budgeted Hour report
-->

<!--
The following information is available in the Budgeted Hour report by default:
-->

<!--
Project This is the name of the project associated with the Budgeted Hour. Job Role This is the name of the job role associated with the Budgeted Hour. User This is the name of the user associated with the Budgeted Hour. Alloc. Date This is the Allocation Date. It is the first day (a Sunday) of the week for which you budgeted the hours. Tip: If a week spans for two months, this generates two rows in the report: one corresponding to the first day of the week (the Sunday of the week which is during the first month), and a second one corresponding with the first day of the second month (and which could be any day of the week.) For example, if you budget 8 hours for a user for the week of June 30 (Sunday) - July 6 (Saturday), the two rows show an Allocation Date of June 30, and July 1. Bud. Hours These are the Budgeted Hours allocated to the User in the Resource Planner. Pln. Bud. Hours These are the Budgeted Hours allocated to the Job Role or the Project in the Resource Planner.
-->

