---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Create a Single-use Timesheet
description: You can manually create a single-use timesheet if you want a timesheet that is not recurring. When the end date of the timesheet is reached and you need more timesheets are needed, you must create new ones.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
---
# Create a single-use timesheet

<!--Audited: 6/2025-->

You can manually create a single-use timesheet if you want a timesheet that is not recurring. When the end date of the timesheet is reached and you need more timesheets are needed, you must create new ones.

For information about creating a timesheet profile that generates recurring timesheets for your users without any further intervention from you (recommended), see [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

For information about manually generating timesheets for all users in the system that are associated with a timesheet profile, see [Manually generate timesheets](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md). 

>[!NOTE]
>
>* Single-use timesheets cannot be created for groups.
>* When creating a single-use timesheet, you cannot select specific general hour types to include in your timesheet. All general hour types that are activated in your system display in timesheets created manually. 
>
>If you want to select only certain general hour types to display in your timesheets, use a timesheet profile. For more information about timesheet profiles, see [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td><p>Administrative access to Timesheets</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a single-use timesheet

{{step1-to-timesheets}}

   The **All** filter is selected by default. This displays all timesheets you have access to view.

   ![Timesheets list with one timesheet selected](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Do one of the following to update the filter in the list of timesheets:

   * Select **My Timesheet Approvals** in the upper-right corner of the page to view only timesheets that you approve

     Or

     Select **My Timesheets** to view only your timesheets.

     This applies the My Timesheet Approvals or the My Timesheet filters to the list of timesheets.

     ![My timesheets filter buttons on the Timesheets list page](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Click the **Filter** icon ![Filter icon](assets/filter-nwepng.png) to apply a different filter, or create a new one. For information about creating or updating filters, see [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >The My Timesheet Approvals and My Timesheets options do not display at the top of the timesheet list or in the list of filters if your Workfront administrator or a group administrator removed the My Timesheet Approvals and the My Timesheets filters from either the List Controls in the Setup area or from your Layout Template. For more information see the following articles:
   > 
   >   * [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) 
   

1. (Optional) Click the **Search** icon ![Search icon](assets/search-icon.png) to type a keyword and search for a specific timesheet. For example, you can search for a timesheet time frame of owner name. 

1. (Optional) Click the **View** ![View icon](assets/view-icon.png) or **Grouping** ![Grouping icon](assets/grouping.png) icons to apply a different view or grouping or to create a new one.

   For information about creating filters, views, or groupings, see the following articles:

   * [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
   * [Create or edit views in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 
   * [Create groupings in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Click **New Timesheet** at the top of the list of timesheets.
   
   Specify the following information:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Create timesheet for</strong> </td> 
      <td>Start entering the name of the user, a job role, or a team for whom you are creating the timesheet, and click them when they display in the list.</td> 
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
      <td>Approvers are users who approve the timesheet for the users associated with the timesheet. Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.<br>Start entering the names of the timesheet approvers and click them when they appear in the list.<br>You can have multiple approvers on a timesheet. In this case, after one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Can edit time</strong> </td> 

      <td> <p>Select this option if you want to allow approvers to edit hours on the timesheet.</p> 
      
      This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.

      The following scenarios exist: 

      <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
   <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
   <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
   <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
   <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
   <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
   <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
   </ul>

   <p><b>NOTE</b>

      Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p>
          
      </td> 
      </tr> 
           
     <tr> 

      <td role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
      <td>You can choose to hide the Overtime box on the timesheet. This option is disabled by default.</td> 
      </tr> 
      </tbody> 
   </table>

1. Click **Create timesheet**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## When tasks and issues appear on users' timesheets

A task or issue assigned to a user automatically appears on the timesheet of a user if the task or issue meets any of the following criteria:

* The user has logged hours on the task or issue
* The planned dates of the task or issue fall within the dates of timesheet
* The task or issue has an Actual Start Date (The task or issue status is In Progress)
* The task or issue is pinned to the timesheet
* The Planned Completion date falls within the date range of the timesheet and the status is In Progress

If the **Pre-Populate timesheets with ...** preferences (located in the Timesheets & Hour preferences) are deselected, the timesheet shows issues and tasks which have a status of In Progress. For more information about the Timesheets & Hour Preferences, see [Configure timesheet and hour preferences](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
