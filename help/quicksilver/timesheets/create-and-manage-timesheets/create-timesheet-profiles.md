---
filename: create-timesheet-profiles
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Create, edit, and assign timesheet profiles
description: You can create, edit, and assign timesheet profiles that generate recurring timesheets for your users without any further intervention from you. This saves you time and ensures that the following are consistent between users - EDIT ME.
---

# Create, edit, and assign timesheet profiles

You can create, edit, and assign timesheet profiles that generate recurring timesheets for your users without any further intervention from you. This saves you time and ensures that the following are consistent between users:

* Timesheet time frame
* Approvers
* General hour types

For more information about creating a timesheet manually, see [Create a single-use timesheet](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

##  

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>You must have administrative access to Timesheets. </p> <p>For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p>  <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create or edit a timesheet profile

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>To enable timesheet profile changes in current timesheets, you have to delete the existing timesheets and then generate new ones. For instructions, see [Delete timesheets in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) and [Manually generate timesheets](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. If you are creating or editing a timesheet profile for use throughout the system, click **Timesheet & Hours**.

   Or

   If you creating or editing a timesheet profile for a group, click **Groups**, then click the group's name.

1. Click **Timesheet Profiles**.
1. To create a new timesheet profile, click **New Profile**.

   Or

   To edit an existing timesheet profile, select the timesheet profile you want to edit, then click **Edit**.

   The new or existing timesheet profile displays.

1. On the**Set Details** tab, type a **Name** and **Description** for the timesheet profile and supply the following information:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
        <ul> 
         <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
        </ul> 
        <ul> 
         <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group’s administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p> <p>Note: When users outside the group are attaching timesheet profiles to other user, they won’t be able to see or attach this timesheet profile.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p> <p>Note:  If you configure a timesheet profile to create timesheets on a Friday, users are not able to record hours on Friday, Saturday, and Sunday, for the current week.</p> <p>Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet&nbsp;starts when the time frame of the first one ends.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approvers</strong> </td> 
      <td> <p> <p>Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
        <ul> 
         <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
         <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
         <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit hours</strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. If Restrict timesheet editing to owners and admins is enabled in Timesheet &amp; Hours &gt; Preferences, you can't enable this setting. </p> <p>Note: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md" class="MCXref xref">Submit a timesheet for approval</a> and<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md" class="MCXref xref">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by&nbsp;selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect&nbsp;all hour types to generate the timesheet without a section for general hours.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click the **Assign People** tab to associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams. Begin typing the name of the user, group, or team, then click it when it appears in the drop-down list.

   If you are a group administrator, you can assign the timesheet profile to groups you administer, but not to teams. For more information, see [Limitations for a group administrator assigning a timesheet profile](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in this article.

   >[!NOTE]
   >
   >
   >   
   >   
   >   * You can also associate a user with a timesheet profile by editing the user profile. For more information, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >   * When you add a group, only the group name appears on the Assign People tab, not the list of group members. If you want to see the group members listed here, click Save Changes, then click the name of the timesheet profile you just created.
   >   * When you finish these steps, the timesheet profile generates timesheets only for the assigned users or group members who don’t have existing timesheets for the current period.
   >   
   >

1. Click **Save Changes** .

   The first time the timesheet profile generates timesheets, 2 timesheets are created for each user. After that, each time it generates new timesheets, onhe timesheet is created per user.

## Limitations for a group administrator assigning a timesheet profile {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

If you are a group administrator and the administrative access option Timesheets & hours is disabled in your access level, you can create timesheet profiles, but you can assign them only to:

* Groups you administer 
* Individual users you have access to edit who are in a group you administer

For these groups and users, you won’t have access to the timesheets that the timesheet profile generates.

Further, if the option User Admin (Group Users) is also disabled in your access level, you can assign the timesheet profile to a group you administer, but it affects only the users in the group that you have access to edit. If the group contains users that you don’t have access to edit, they are not assigned the timesheet profile along with the rest of the group.

For information about the option Timesheets & hours in your access level, see [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

For information about the option User Admin (Group Users) in your access level, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Multiple recurring timesheet profiles

You can have more than one timesheet profile for your organization if there are:

* Unique pay periods for different sets of users
* Unique approvers for different sets of users
* Unique general hours requirements for different sets of users

One user cannot be associated with more than one timesheet profile at a time.&nbsp;
