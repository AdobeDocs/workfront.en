---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Lock or Unlock a Project, Task, or Issue Preference for Subgroups
description: As a group administrator, you can configure and then lock a project, task, or issue preference if a Workfront administrator has unlocked it at the system level.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
---
# Lock or unlock a project, task, or issue preference for subgroups

As a group administrator, you can configure and then lock a project, task, or issue preference if a Workfront administrator has unlocked it at the system level.

Locking a project, task, or issue preference that you have configured at the level ensures that everyone in your group and in its subgroups is using the same setting for that preference. Though you can still reconfigure a preference that you lock for your group, group administrators can't reconfigure it for groups.

Conversely, unlocking a project, task, or issue preference allows group administrators more flexibility to manage the way their groups work with those items. When a preference is unlocked, group administrators can reconfigure it for  those subgroups.

This is parallel to the ability that a Workfront administrator has to lock or unlock a preference for everyone in the system.

For information about how a Workfront administrator can lock or unlock a preference for all groups in the system, see [Lock or unlock project preferences for all groups in the system](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Configuring an unlocked preference for a group doesn't affect that preference for any subgroups below the group.
>
>  However, when a new subgroup is created, it inherits the preference settings and locked or unlocked state of the group immediately above it.
>
>* If you move a group under a group that has a locked preference, the moved group inherits that preference and it is locked for the moved group. 
>* If you move a group under a group that has an unlocked preference, the moved group is not affected by that preference.
>
>  If the preference in the moved group is locked at the time of the move, it remains locked, but the group administrator can unlock it now because it is unlocked for the parent group.
>

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

+++

## Lock or unlock a group project, task, or issue preference

{{step-1-to-setup}}

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
