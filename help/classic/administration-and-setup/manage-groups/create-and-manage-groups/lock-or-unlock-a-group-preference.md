---
filename: lock-or-unlock-a-group-preference
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Lock or unlock a project, task, or issue preference for subgroups
description: As a group administrator, you can configure and then lock a project, task, or issue preference if a Workfront administrator has unlocked it at the system level.
---

# Lock or unlock a project, task, or issue preference for subgroups

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

As a group administrator, you can configure and then lock a project, task, or issue preference if a Workfront administrator has unlocked it at the system level.

Locking a project, task, or issue preference that you have configured at the```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  group</MadCap:conditionalText>``` level ensures that everyone```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  in your group and in its subgroups</MadCap:conditionalText>``` is using the same setting for that preference. Though you can still reconfigure a preference that you lock```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  for your group</MadCap:conditionalText>```, group administrators can’t reconfigure it for ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> sub</MadCap:conditionalText>```groups```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  on lower levels</MadCap:conditionalText>```.

Conversely, unlocking a ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> group’s </MadCap:conditionalText>```project, task, or issue preference allows ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> sub</MadCap:conditionalText>```group administrators more flexibility to manage the way their groups work with those items. When a ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> group </MadCap:conditionalText>```preference is unlocked, group administrators```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  of lower subgroups</MadCap:conditionalText>``` can reconfigure it for ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> those subgroups</MadCap:conditionalText>```.

This is parallel to the ability that a Workfront administrator has to lock or unlock a preference for everyone in the system.

For information about how a Workfront administrator can lock or unlock a preference for all groups in the system, see [Lock or unlock project preferences for all groups in the system](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

<table cellspacing="0"> 
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

## Lock or unlock a group project, task, or issue preference

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. In the left panel, click **Groups**.
1. Click the name of the group where you want to lock or unlock a project preference.
1. In the left panel, click **Project Preferences** or **Tasks & Issues Preferences**.

1. On the page that appears, do any of the following for a preference that is unlocked at the system level or for a group above your group:

   * If you want administrators of groups below your group to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
   * If you want all groups below yours to use your configuration for a preference, make sure that it is locked ![](assets/lock-toggle-button.png).

     >[!IMPORTANT]
     >
     >It's important to communicate with the administrators and users in groups below yours to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by any subgroups below. And if the preference has been unlocked for any period of time, your configuration replaces those that group administrators in lower subgroups might have made.

1. Click **Save**.

