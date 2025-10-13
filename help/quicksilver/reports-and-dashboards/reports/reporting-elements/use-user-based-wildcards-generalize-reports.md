---
product-area: reporting
navigation-topic: reporting-elements
title: Use user-based wildcards to generalize reports
description: You can generalize a report by using wildcards instead of specific information when building certain reporting elements.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
---
# Use user-based wildcards to generalize reports

<!-- Audited: 11/2024 -->

You can generalize a report by using wildcards instead of specific information when building certain reporting elements. For example, if you want to create a report that shows the tasks assigned to a specific user, you can use the user's name in the Assigned To field of the filter. However, if you want to create a report that shows tasks assigned to the logged in user, regardless of who that user is, you can use a wildcard that indicates that when someone views the report it displays information pertaining only to them. This way, you build the report once but because you use a wildcard in the filter it produces different results every time someone else reads it.

You can use user-based wildcards when building the following reporting elements:

* Filters
* Custom prompts
* Views when adding rules for columns

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to Reports, Dashboards, Calendars to edit reporting elements in a report</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
    <td> <p>Manage permissions to a report to edit reporting elements in a report</p> <p>Manage permissions to a view or filter to edit them</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

You must create a report before you can add a wildcard variable to it.

For instructions on creating reports, see [Create a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## How-to steps

To insert a user-based wildcard in a report:

1. Go to a report for which you want to insert a user-based wildcard.
1. Click **Report Actions**, then **Edit**.

1. Click the **Filters** tab.
1. Click **Add a Filter Rule**.
1. Start typing the name of the field that you want to filter by.  
   You must type fields that reference the user object or information about users.
1. Select **Equal** in the drop-down menu for the filter variable.

   >[!TIP]
   >
   >You must always select the **Equal** filter variable when working with wildcards in Adobe Workfront.

1. In the **Start typing name ...** box, type: `$$USER.ID` or `$$USER.name` if you want the report to display information about the user who logs in, based on their name. You can insert other wildcards that refer to the logged-in user's Group, Team, Company, or other information.

   For a complete list of user-based wildcards, see [Wildcard filter variables overview](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Click **Save + Close**.

## Additional information

See also:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Wildcard filter variables overview](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md) 
* [Create or edit filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
* [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) 
* [Use conditional formatting in views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
