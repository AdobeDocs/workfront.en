---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Edit report settings
description: You can edit the settings of a report to define how it displays for other users, or what kind of information can users prompt for before they run the report.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
---
# Edit report settings

You can edit the settings of a report to define how it displays for other users, or what kind of information can users prompt for before they run the report.

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
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## How-to steps

1. Start creating a report by going to the **Main menu** > **Reports**, then select the object of your report.

   Or

   Open an existing report, then click **Report Actions** > **Edit**.

1. Click **Report Settings** in the upper-right corner of the report builder.
1. Configure the following report settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Report Title</td> 
      <td>Specify a title for the report.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Specify a statement describing the purpose and uses of the report.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Run this report with the Access Rights of</td> 
      <td>Select the user whose access rights you want this report to use when displaying for other users. For more information about running a report with the access rights of another user, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">When the Report loads, show the</td> 
      <td>Select the default tab that is displayed for all users when the report loads.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">When the report loads on a dashboard, show ... items</td> 
      <td>Specify the number of items that are displayed for all users when the report loads on a dashboard. The default is 15 items and the maximum number of items is 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Show the Resource Grid view on the Details tab</td> 
      <td> <p>(User Report Only) Select this option to display the Resource Grid on the Details tab of the report.</p> <p>Note:  When applying the Resource Grid view to a user report, the report only shows projects that are in the Current status. If you want to see projects in any other status, you can use the User Utilization Tab in the People area of the Global Navigation Bar, and apply the Resource Grid View there. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Show a special view on the Details tab</td> 
      <td>(Project Report Only) Specify the type of view users will see when they access this information on the Details tab. For example, you can select a Milestone or Gantt view.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Show this report in a Gantt view by default</td> 
      <td>(Project Report and Task Report Only) Select this option to have the Gantt view automatically enabled when users view the Details tab in this report.<br>For more information about viewing the Gantt chart in project reports and task reports, see the section "View task information in the project list Gantt Chart" in the article <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">View information in the Gantt Chart </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow View to be changed on the report</td> 
      <td>Select this option to allow users to change the View when running the report.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow Group to be changed on the report</td> 
      <td>Select this option to allow users to change the Group when running the report.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow Filter to be changed on the report</td> 
      <td>Select this option to allow users to change the Filter when running the report.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Report Prompts** to set up any prompts for the report.  
   For more information about adding prompts to a report, see the article [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Click**Done,** then click **Save + Close**.

## Additional information

See also:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Get started with reports in Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md) 
* [Use Adobe Workfront built-in reports](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md) 
* [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
