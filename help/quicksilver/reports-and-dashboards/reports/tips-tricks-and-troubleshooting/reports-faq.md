---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Reports FAQs
description: Reports FAQs
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
---
# Reports FAQs

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

The following are frequently asked questions about reports.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Why does my custom calculation for an hour difference not show the correct result in a column?

On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  
My calculation is:
<pre>valueexpression=SUB(workRequired,actualWorkRequired)</pre>

### Answer

Fields using hours in Workfront are stored in minutes. When using the field in a calculation the result will be in minutes. To obtain the result in hours, you must divide the result of the calculation by 60.

The correct calculation is:  

<pre>valueexpression=SUB(workRequired,actualWorkRequired)/60</pre>

## Why is the value of each of my chart elements in a report not displayed on the chart?

### Answer

If you have more than 50 chart elements in a report chart, the value of each element does not display in the chart.

When you have less than 50 elements in a chart, the value of each element displays in the chart. Consider adding a filter or modifying the groupings in the report to limit the amount of items you display in each element of the chart.

## Why is my report returning too many results to display the chart?

When I run a report that has a chart, I see the error message "Whoa there... This report returned A LOT of data which makes the chart unreadable. Consider narrowing your results by adding a filter or changing the groupings in your chart."

### Answer

This error means that your chart contains up to 618 distinct results—for example, more than 618 bars in a bar chart. To resolve the display issue, you need to refine the results by modifying your current filter and grouping selections.

For information on modifying filters and groupings, see the articles [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) and [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Why do I see my tasks (or issues) when I access the same report (or calendar) as my coworker and they see their tasks instead?

### Answer

The report or calendar might have a wildcard filter variable which points to the user who is logged in. In this case, the report shows information based on the user who is logged in. Adjust the filter to remove the wildcard that points to the logged-in user.  
![](assets/qs--user.id-filter-variable-350x79.png)

For a complete list of user-based Wildcard filter variables overview, see [Wildcard filter variables overview](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Why does the data in my report seem incomplete?

### Answer

This can happen in most cases if you have a limited access that prevents you from seeing items in the system. Additionally, the items that you want to see are not shared with you.

The creator of the report can edit the report to run it with the access rights of a system administrator, or any Plan user who has access to see the data.

For more information, see [Run and deliver a report with the access rights of another user](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## How do I report on tasks (or issues) that I am assigned to, whether I am the Owner on them or not?

### Answer

To see all tasks or issues assigned to you, whether you are the Owner (or Primary Assignee) or not, use the following filter in a task or issue report:

1. Access a task or issue report.
1. On the **Filters** tab, click **Add a Filter Rule**.

1. In the **Start typing field name ...** field, start typing **Assignment Users Name**, then select it when it appears in the list.

   >[!NOTE]
   >
   >Do not use the **Assigned To Name** field, as this filters only for the tasks and issues for which you are the Primary Assignee, or Owner.

1. Select the **Equal** modifier.
1. Start typing *$$USER.ID* in the textbox and select it from the drop-down list that appears.  
   This ensures that you see all tasks and issues that are assigned to the logged in user. You can replace the wildcard with a specific user name.  
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Click **Save + Close**.

## Why are the Add Issues/Add Tasks links not appearing at the bottom of my Issues and Tasks lists on a project?

### Answer

First, ensure that you have the correct access and permissions to add issues and tasks to a project. In this case, you should see the **Add Issues** and **Add Tasks** links at the bottom of the **Issues** and **Tasks** lists.

However, there are a few things that may prevent these links from displaying:

* If you have the quick filter applied to these lists, the links do not display. Remove the quick filter and the links should display so you can add issues and tasks to your projects.  
  For information about the quick filter, see [Get started with lists in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* If you have a **Grouping** applied to these lists, the links do not display. Remove the **Grouping** and the links should display so you can add issues and tasks to your projects.  
  For information about creating Groupings, see [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* If you have a **View** applied to these lists that has a currency selected other than the default currency for the project, the links do not display. Change the **View** to **Project's Original Currency** and the links should display so you can add issues and tasks to your projects.  
  For more information on changing the currency in your View, see [Create financial data reports with unique exchange rates](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## Does the information in my report or dashboard refresh automatically?

### Answer

Information in reports or dashboards does not refresh automatically.

Information can be manually refreshed in a cached report.  
For more information about refreshing a cached report, see [Run a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Information can be manually refreshed in a cached dashboard.  
For more information about refreshing a cached dashboard, see the section [Display dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) in the article [Get started with dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Can I change the owner of a report?

### Answer

You can't change the owner of a report. However, the user who created the report can allow other users to edit the report. The way you can allow users to edit a report depends on the type of user you are.

* System administrators can allow users with a Plan license to edit reports by configuring the Edit option in the Reports row to include the access to Create a report.  
  For more information, see [Grant access to reports, dashboards, and calendars](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Any end users with access to create and share reports can allow others to edit individual reports by sharing them and giving other users Manage permissions to them.  
  For more information, see [Share a report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

If you have permissions to view or manage a report, you can also make a copy of the report, which you will then be the owner of by default. To learn more about copying a report, see [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Why can't I access a report owned by a deactivated user?

### Answer

Sometimes, the owner of the report is also the user specified in the **Run this report with the Access Rights of:** field on the report. If the **Run this report with the Access Rights of:** user is deactivated, the report no longer displays for users who have the report shared with them.&nbsp;When this happens, you can make the report accessible again by leaving the **Run this Report with the Access Rights of:** blank or entering an active user in the field.

To learn more about the **Run this Report with the Access Rights of:** field, see [Run and deliver a report with the access rights of another user](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). For information on identifying all reports owned by deactivated users, see [Create a report on reporting activities](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## How do I access a dashboard that contains a report owned by a deleted user?

### Answer

When you delete a user, you can still access any reports that they created, however, any dashboards that included the report are deleted as well. This means that you can no longer access the following:

* A dashboard that contains the report
* A custom section that contains a dashboard of the report

To learn more about the implications of deleting a user, see [Delete users](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

If you have View access to the report, you can do the following:

1. Create a copy of the report.  
   To learn how to create a copy of a report, see [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Update the dashboard to include the copied report.  
   To learn how to edit a dashboard, see [Edit a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
