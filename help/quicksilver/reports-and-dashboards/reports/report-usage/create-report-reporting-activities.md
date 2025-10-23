---
product-area: reporting
keywords: change,owner,shared,report,share,run,user,access,rights,entered,last,viewed,date,reporting,activities
navigation-topic: report-usage
title: Create a report on reporting activities
description: When you create a report about reports, you can identify specific report information, which can include if reports are assigned to deactivated users, if reports are set to run with access rights of a deactivated user, if users are accessing a report you plan to delete, and so forth.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
---
# Create a report on reporting activities

When you create a report about reports, you can identify specific report information, which can include if reports are assigned to deactivated users, if reports are set to run with access rights of a deactivated user, if users are accessing a report you plan to delete, and so forth.

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard</p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars</p> <p>Edit access to Filters, Views, Groupings</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create the report about existing reports {#create-the-report-about-existing-reports}

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.
1. Click **Reports**, then **New Report**.
1. In the **New Report** drop-down men, select **Report** to create a report on existing reports.

1. In the **Columns (View)** tab, add the columns you want in your report.  
   Some of the following fields may be useful:  

   | Field |Description |
   |---|---|
   | **Run As User: Name** |This is the user specified in the **Run this report with the Access Rights of:** field on the report. If this user is deactivated, a report does not display for anyone the report is shared with. |
   | **Shared With** |These are all the entities that the report is shared with. |
   | **Entered By** |This is the owner of the report. |
   | **Last Viewed Date** |This is the date and time the report was last viewed by a user. |

   {style="table-layout:auto"}

1. (Optional) To limit your list of reports to specific deactivated users:

   1. Select the **Filters** tab, then click **Add a Filter Rule**.
   
   1. Add the filter **Run As User ID** > **Equal**.
   
   1. Type the name of the deactivated user you want to add to the filter, then click the name when it displays in the list.
   1. Repeat Step C until you have selected all deactivated users you want to include in the report.

1. (Optional) To limit your list of reports to scheduled reports:

   1. Select the **Filters** tab, then click **Add a Filter Rule**.
   
   1. Add the filter **Scheduled Report ID** > **Is Not Blank**.

1. Click **Save + Close**, then type a name for the report, and click **Save Report**.

   Your report information displays.

1. (Optional) Export this report to Excel and save it on your computer.  
   For information on exporting a report, see [Export data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Update information about a report

After creating your report, you can update your reports as needed.

1. Go to the report you want to update.
1. Depending on the action you want to take, do one of the following:

   * Update the **Run this report with the Access Rights of:** field to an active user: For more information, see [Run and deliver a report with the access rights of another user](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).
   
   * Create a copy of the report: For more information, see [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Delete a report:&nbsp;For more information, see the [Create an exact copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) section of the article [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   
   * Share a report:&nbsp;For more information, see [Share a report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Conditional) If you copy the original reports, use the information from the report you created in [Create the report about existing reports](#create-the-report-about-existing-reports) to share the new copies with the same entities as the original reports.
