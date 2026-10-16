---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Export a list of timesheets
description: As a people manager or timesheet approver, you might need to download a list of timesheets to quickly view information about the timesheets of the people you are responsible for. You can do this by exporting a list of timesheets.
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Export a list of timesheets

<!--Audited: 8/2024-->

As a people manager or timesheet approver, you might need to download a list of timesheets to quickly view information about the timesheets of the people you are responsible for. You can do this by exporting a list of timesheets.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td> <p>Light or higher </p>
   <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Access level configuration</td> 
   <td> <p>View or higher access to Tasks and Issues</p> </td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Export a list of timesheets

{{step1-to-timesheets}}

   All timesheets that you have access to view are displayed by default.

   ![Timesheets list](assets/list-of-all-timesheets.png)

1. (Optional) Do one of the following to update the filter in the list of timesheets:

   * Select **My Timesheet Approvals** in the upper-right corner of the page to view only timesheets that you approve,

     Or

     Select **My Timesheets** to view only your timesheets.

     This applies the **My Timesheet Approvals** or the **My Timesheet** filters to the list of timesheets.

   * Click the **Filter** icon ![Filter icon](assets/filter-nwepng.png) to apply a filter or create a new filter. For information about creating or updating filters, see [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >The My Timesheet Approvals and My Timesheets options do not display at the top of the timesheet list or in the list of filters if your Workfront administrator or a group administrator removed those filters from either the List Controls in the Setup area or from your Layout Template. For more information, see [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Optional) Click the **View** ![View icon](assets/view-icon.png) or **Grouping** ![Grouping icon](assets/grouping.png) icons to apply a view or grouping or to create a new one.

   For information about creating filters, views, or groupings, see the following articles:

   * [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
   * [Create or edit views in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 
   * [Create groupings in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Select the timesheets that you want to export, then click the **Export** ![Export icon](assets/export-38x15.png) icon.

   ![Click the Export icon](assets/export-timesheets.png)

1. Select the type of file that you want to export the list of timesheets to from the following options:

   * PDF Ladscape
   * PDF Portrait
   * PDF Other Sizes
   * Excel
   * Excel (xlsx)
   * Tab Delimited

   A list of timesheets is downloaded to your computer in the selected format and includes the following timesheet information:

   * Date Range
   * Owner name
   * Total Hours
   * Overtime amount
   * Approvers names
   * Status
