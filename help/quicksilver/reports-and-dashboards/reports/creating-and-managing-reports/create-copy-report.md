---
product-area: reporting;user-management
keywords: save,new,report,copy
navigation-topic: create-and-manage-reports
title: Create a copy of a report
description: You can create a copy of any report that you have access to. You can either create an exact copy of a custom report or you can save a new version of a default report. After you copy a report, you become the owner of the copied report and it displays in the My Reports section.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
---
# Create a copy of a report

<!-- Audited: 11/2024 -->

You can create a copy of any report that you have access to. You can either create an exact copy of a custom report or you can save a new version of a default report. After you copy a report, you become the owner of the copied report and it displays in the My Reports section.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

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
   <td> 
      <p>New:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Current:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions*</td> 
   <td><p>View permissions to a report</p></td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Create an exact copy of a report

If you want to make a copy of a custom report, do the following:

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Reports]**.

1. Click **All Reports**, then open a report.

1. Click **Report Actions**, then **Copy**.

   >[!TIP]
   >
   >If the report is a default report, the Copy option does not appear in the Report Actions menu.  
   >For information on how to create a copy of a default report, see [Create a new version of a report](#create-a-new-version-of-a-report).

   ![Copy report](assets/unshimmed-report-actions-copy.png)

   A copy of the original report is created with the default name of _[Name of the original report] (Copy)_. For example, a copy of the report "Q4 Completed Tasks" would be named "Q4 Completed Tasks (Copy)".

1. (Optional) To rename the report, click **Report Actions** then **Edit**. Type a new name in the text box in the top left corner, then click **Save + Close** when finished.

1. (Optional) To share the new version of the report with other users, click **Report Actions**, then **Sharing**.

   >[!NOTE]
   >
   >The sharing information does not transfer to the copied report from the original version.  
   >For information on how to see who the previous report was shared with, see [Create a report on reporting activities](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Optional) If you have Manage permissions to the original report and the original report is no longer needed, you can delete it to remove unnecessary duplicated reports in Workfront.

   To delete the original report, do the following:

   1. Navigate to the report.

   1. Click **Report Actions**, then **Delete**.
   
   1. Click **Yes, Delete it** to confirm that you want to delete the report.

## Create a new version of a report {#create-a-new-version-of-a-report}

If you want to create a copy of a default report, do the following:

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Reports**, then **All Reports**. 
1. Click the name of a default report to open it.
1. Click **Report Actions**, then **Edit**.

   ![Edit report](assets/unshimmed-report-actions-default-report.png)

1. Make any modifications you need to in the following tabs of the report:

   * **Columns (View)**: For more information about customizing views, see the article [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Groupings**: For more information about customizing groupings, see the article [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filters**: For more information about customizing filters, see the article [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Chart**: For more information about customizing a report chart, see the article [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. In the upper-right corner, click **Report Settings**.
1. In the **Report Title** field, give the report a new name.
1. Click **Done**.
1. Click **Save as New Report**.

   ![Save as new report](assets/unshimmed-save-as-new-report.png)

1. (Optional) To share the new version of the report with other users, click **Report Actions**, then **Sharing**.
