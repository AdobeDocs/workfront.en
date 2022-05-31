---
filename: create-tmshts
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Create a single-use timesheet
description: You can manually create a single-use timesheet if you want a timesheet that is not recurring. When the end date of the timesheet is reached and you need more timesheets are needed, you must create new ones.
---

# Create a single-use timesheet

You can manually create a single-use&nbsp;timesheet if you want a timesheet that is not recurring.&nbsp;When the end date of the timesheet is reached and you need more timesheets are needed, you must create new ones.

For information about creating a timesheet profile that generates recurring timesheets for your users without any further intervention from you (recommended), see [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Single-use timesheets cannot be created for groups. >
>  <!--
>  <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Making sure with Lilit that this is correct</span>>
>  -->
>* When creating a single-use timesheet, you cannot specify&nbsp;specific general hour types to include in your timesheet. All general hour types that are activated in your system display in timesheets created manually. 
>
>  If you want to select only certain general hour types to display in your timesheets, use a timesheet profile.&nbsp;For more information about timesheet profiles, see [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

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
   <td> <p>You must have administrative access to Timesheets. </p> <p>For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create a single-use timesheet

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Timesheets**. The **All** filter is selected by default. This displays all timesheets you have access to view.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

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
   >   * [Edit list controls: filters, views, and groupings](../../administration-and-setup/manage-workfront/configure-reports/edit-list-controls-filters-views-groupings.md) 
   >   * [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) 
   >   
   >

1. (Optional) Click the **View** ![](assets/view-icon.png) or **Grouping** ![](assets/grouping.png) icons to apply a different view or grouping or to create a new one.

   For information about creating filters, views, or groupings, see the following articles:

   * [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
   * [Create or edit views in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 
   * [Create groupings in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Click **New Timesheet** at the top of the list of timesheets.
1. Specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Create timesheet for</strong> </td> 
      <td>Start entering the name of the user for whom you are creating the timesheet, and click it when it appears&nbsp;in the list.</td> 
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
      <td>Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.<br>Start entering the names of the timesheet approvers and click them when they appear&nbsp;in the list.<br>You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time</strong> </td> 
      <td> <p>Select this option if you want to allow approvers to edit hours on the timesheet.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
      <td>You can choose to hide the Overtime box on the timesheet. This option is disabled by default.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Create timesheet**.

## When tasks and issues appear on users' timesheets

A task or issue assigned to a user automatically appears on the timesheet of a user if the task or issue meets any of the following criteria:

* The user&nbsp;has logged hours on the task or issue
* The planned dates of the task or issue fall within the dates of timesheet
* The task or issue has an Actual Start Date (The task or issue status is In Progress)
* The task or issue is pinned to the timesheet
* The Planned Completion date falls within the date range of the timesheet and the status is In Progress

If the **Pre-Populate timesheets with ...** preferences (located in the Timesheets & Hour preferences) are&nbsp;deselected, the timesheet shows issues and tasks which have a status of In Progress. For more information about the Timesheets & Hour Preferences, see [Configure timesheet and hour preferences](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
