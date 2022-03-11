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
>  <!-->
>  Making sure with Lilit that this is correct>
>  -->
>* When creating a single-use timesheet, you cannot specify&nbsp;specific general hour types to include in your timesheet. All general hour types that are activated in your system display in timesheets created manually. 
>
>  If you want to select only certain general hour types to display in your timesheets, use a timesheet profile.&nbsp;For more information about timesheet profiles, see [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must have administrative access to timesheets. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Create a single-use timesheet

To create a single-use timesheet:

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront. Click Timesheets. Click All Timesheets in the left panel. 
 <li value="4"> Click <span class="bold">New Timesheet</span>.</li> 
 <li value="5"> <p>Specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Create timesheet for</span> </td> 
     <td>Start entering the name of the user for whom you are creating the timesheet, and click it when it appears&nbsp;in the list.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Start Date</span> </td> 
     <td>This is the start date of the timesheet.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">End Date</span> </td> 
     <td> This is the end date of the timesheet.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Approvers</span> </td> 
     <td>Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.<br>Start entering the names of the timesheet approvers and click them when they appear&nbsp;in the list.<br>You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <span class="bold">Closed</span> and it disappears from the timesheet approvals list of all the remaining approvers.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Can edit time</span> </td> 
     <td> <li> Select this option if you want to allow approvers to edit hours on the timesheet.&nbsp;</li> </td> 
    </tr> Overtime You can choose to hide the Overtime box on the timesheet. This option is disabled by default. 
   </tbody> 
  </table> </li> 
 <li value="6">Click <span class="bold">Create Timesheet</span>.</li> 
</ol>

## When tasks and issues appear on users' timesheets

A task or issue assigned to a user automatically appears on the timesheet of a user if the task or issue meets any of the following criteria:

* The user&nbsp;has logged hours on the task or issue
* The planned dates of the task or issue fall within the dates of timesheet
* The task or issue has an Actual Start Date (The task or issue status is In Progress)
* The task or issue is pinned to the timesheet
* The Planned Completion date falls within the date range of the timesheet and the status is In Progress

If the "Pre-populate timesheets..." preferences (located in the Timesheets & Hour preferences) are&nbsp;deselected, the timesheet shows issues and tasks which have a status of In Progress. For more information about the Timesheets & Hour preferences, see [Configure timesheet and hour preferences](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)
