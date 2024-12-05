---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Run a report
description: You can run any report that you have access to View.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
---

# Run a report

You can run any report that you have access to View.

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

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
   <td> <p>View access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a report</p></td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Run a report

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Reports]**.
 
1. Select from the following options:

   * **My Reports:** Reports that you have created.
   * **Shared With Me:** Reports that other users have shared with you.
   * **All Reports:** All reports in the system that you have access to.

1. Click the name of the report that you want to run.  
   Or  
   If the report was created using prompts, select the appropriate information from the drop-down menus, then click **Run Report**.  
   For more information about prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).  
   The contents of the report display with a timestamp in the upper-right corner of the report that includes the date, time, and time zone when the report was run from the context of the user who ran the report.

1. (Optional) Click the **Reload icon** ![Reload icon](assets/unshimmed-report-refresh-icon.png) to refresh the results in a report if the report has been displayed in your browser for a while.  

1. (Conditional) If the report uses filters or prompts, click **Show Filters and Prompts** to display a list of filters and prompts that are being used on the report you are viewing. If the report contains only filters or only prompts, **Show Filters** or **Show Prompts** appears instead.

   ![Show filters and prompts](assets/unshimmed-show-filters-and-prompts.png)

   Information displays below the report name on the left side of the page. For prompts, this is information about the prompt selections made at the time the report was run, as described in Step 3.

1. If you are using Custom Prompts, they do not display. Only the system prompts display. Custom Filters always display.

## View a cached report

Your report might be cached if it has been displayed in your browser for a while. You can force a cached report to reload when you perform any of the following actions:

* Edit the report settings and save the report.
* Change the View, Group, or Filter.
* Click the **Reload icon** ![Reload icon](assets/unshimmed-report-refresh-icon.png)
  This option is available in the upper-right corner of the page within the message box that indicates the time that the report was saved, or it is available in the upper-right corner of the dashboard that the report is placed on. For more information about reloading dashboards, see the section "Display Dashboards" in the article [Get started with dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Access any page of the report beyond the first page by navigating to the Summary, Matrix, or Chart tabs.
