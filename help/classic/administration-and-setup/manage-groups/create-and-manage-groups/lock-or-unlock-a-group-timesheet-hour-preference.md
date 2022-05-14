---
filename: lock-or-unlock-a-group-timesheet-hour-preference
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Lock or unlock a group timesheet and hour preference
description: If you are a group administrator, you can configure and then lock a timesheet and hour preference for your group after a Workfront administrator unlocks it at the system level.
---

# Lock or unlock a group timesheet and hour preference

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

If you are a group administrator, you can configure and then lock a timesheet and hour preference for your group after a Workfront administrator unlocks it at the system level.

Locking an Adobe Workfront preference```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  at the group level</MadCap:conditionalText>``` ensures that everyone```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  in your group and in its subgroups</MadCap:conditionalText>``` is using the same setting for that preference. Though you can still reconfigure a preference that you lock, group administrators can’t do so for ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> lower subgroups</MadCap:conditionalText>```.

Conversely, unlocking a preference```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  at the group level</MadCap:conditionalText>``` allows ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> sub</MadCap:conditionalText>```group administrators more flexibility to manage the way their groups work with those items. When a ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> group </MadCap:conditionalText>```preference is unlocked, group administrators```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  of lower subgroups</MadCap:conditionalText>``` can reconfigure it for ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> those subgroups</MadCap:conditionalText>```.

This is parallel to the ability that a Workfront administrator has to lock or unlock a preference for everyone in the system.

For information about how a Workfront administrator can lock or unlock a timesheet and hour preference for all groups in the system, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

For information about configuring a timesheet and hour preference for a group, see [Configure timesheet and hour preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Configuring an unlocked preference for a group doesn’t affect that preference for any subgroups below the group.
>
>  However, when a new subgroup is created, it inherits the preference settings and locked or unlocked state of the group immediately above it.
>
>* If you move a group under a group that has a locked preference, the moved group inherits that preference and it is locked for the moved group. 
>* If you move a group under a group that has an unlocked preference, the moved group is not affected by that preference.
>
>  If the preference in the moved group is locked at the time of the move, it remains locked, but the group administrator can unlock it now because it is unlocked for the parent group.
>

## Access requirements

You must have the following to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## Lock or unlock a group timesheet and hour preference

>[!NOTE]
>
>If you are a group administrator, you can lock a group timesheet or hour preference only in the new Adobe Workfront experience. 
>
>Or you can ask a Workfront administrator to lock the group preference for you from the main Timesheets & Hours Preferences area in Setup, as explained in the Tip below. This can be done in Workfront Classic.

>[!TIP]
>
>If you are a Workfront administrator, you can bypass steps 1-4 by going to Setup > Timesheet &&nbsp;Hours > Preferences, then searching for the group’s name in the box at the top of the page.

1. In the left panel, click **Groups**.
1. Click the name of the group where you want to lock or unlock a timesheets and hours preference.
1. In the left panel, click **Timesheets and Hour****s Preferences**.

1. On the page that appears, do any of the following:

   * If you want administrators of groups below your group to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
   * If you want all groups below yours to use your configuration for a preference, make sure that it is locked ![](assets/lock-toggle-button.png) (this is the default).

     >[!IMPORTANT]
     >
     >It's important to communicate with the administrators and users in groups below yours to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by any subgroups below. And if the preference has been unlocked for any period of time, your configuration replaces those that group administrators in lower subgroups might have made.

1. Click **Save**.

