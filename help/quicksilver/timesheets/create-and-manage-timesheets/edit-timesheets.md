---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Edit timesheet information
description: As a user with administrative access to Timesheets, you can edit information on existing timesheets in Adobe Workfront . For example, you can edit the Owner, the Approvers, or the time frame of the timesheet.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
---
# Edit timesheet information

As a user with administrative access to Timesheets, you can edit information on existing timesheets in Adobe Workfront . For example, you can edit the Owner, the Approvers, or the time frame of the timesheet.

You can edit information on a single timesheet, or you can edit multiple timesheets in bulk.

>[!IMPORTANT]
>
>If users are associated with Timesheet Profiles and the timesheets are automatically generated, the changes you make to existing timesheets do not reflect on timesheets that will be generated for future dates. All timesheets generated automatically have the settings established in the Timesheet Profiles. For more information, see [Create timesheet profiles](../create-and-manage-timesheets/create-timesheet-profiles.md)


## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must have administrative access to Timesheets. </p> <p>For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Edit timesheets

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Timesheets**.

   The **All** filter is selected by default which displays all the timesheets that you have access to view.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Click the **search** icon ![](assets/search-icon.png) and type a keyword and search for a specific timesheet. For example, you can search for a timesheet time frame or owner name. 

1. (Optional) Do one of the following to update the filter in the list of timesheets:

   * Select **My Timesheet Approvals** in the upper-right corner of the page to view only timesheets that you approve

     Or

     Select **My Timesheets** to view only your timesheets.

     This applies the My Timesheet Approvals or the My&nbsp;Timesheet filters to the list of timesheets.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Click the Filter icon ![](assets/filter-nwepng.png) to apply a different filter, or create a new one. For information about creating or updating filters, see [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >The My Timesheet Approvals and My&nbsp;Timesheets options do not display at the top of the timesheet list or in the list of filters if your Workfront administrator or a group administrator removed the My&nbsp;Timesheet Approvals and the My&nbsp;Timesheets filters from either the List Controls in the Setup area or from your Layout Template.&nbsp;For more information see the following articles:
   >
   >   
   >   
   >   * [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) 
   >   
   >

1. (Optional) Click the**View** ![](assets/view-icon.png) or **Grouping** ![](assets/grouping.png) icons to apply a different view or grouping or to create a new one.

   For information about creating filters, views, or groupings, see the following articles:

   * [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
   * [Create or edit views in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 
   * [Create groupings in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Select one or several timesheets, then click the **Edit** icon ![](assets/edit-icon.png) at the top of the timesheet list. 
1. View or specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Owner</strong> </td> 
      <td> <p>This is the name of the user for which the timesheet was created.&nbsp;You cannot edit this field. </p> <p>The field does not display when you select multiple timesheets. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Start Date</strong> </td> 
      <td>This is the start date of the timesheet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>End Date</strong> </td> 
      <td> This is the end date of the timesheet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approvers</strong> </td> 
      <td> <p>Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. Only users with administrative access to Timesheets can be set as approvers. </p> <p>For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Start entering the names of the timesheet approvers and select them when they appear&nbsp;in the list.</p> <p>You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time</strong> </td> 
      <td> <p>Select this option if you want to allow approvers to edit hours on the timesheet.</p> <p>This option is not available when you select multiple timesheets. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
      <td> <p>You can choose to hide the Overtime box on the timesheet.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click Save.
