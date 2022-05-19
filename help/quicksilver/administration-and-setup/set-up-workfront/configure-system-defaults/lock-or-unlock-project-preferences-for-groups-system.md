---
filename: lock-or-unlock-project-preferences-for-groups-system
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Lock or unlock project preferences for all groups in the system
description: Groups in your organization might need a project preference configured differently for their unique workf lows. You can unlock the preference for all groups throughout the organization so that they can configure it on their own.
---

# Lock or unlock project preferences for all groups in the system

Groups in your organization might need a project preference configured differently for their unique workf lows. You can unlock the preference for all groups throughout the organization so that they can configure it on their own.

When a preference is unlocked and the group administrator modifies it, the projects associated with the group acquire the configuration for that preference from the group-level setting instead of from the system-level setting.

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
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
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## About locked and unlocked preferences

Locking a project, task, or issue preference that you have configured at the```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level">  system</MadCap:conditionalText>``` level ensures that everyone```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level">  throughout the system</MadCap:conditionalText>``` is using the same setting for that preference. Though you can still reconfigure a preference that you lock, group administrators can't reconfigure it for ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level"> their</MadCap:conditionalText>``` groups.

Conversely, unlocking a project, task, or issue preference allows group administrators more flexibility to manage the way their groups work with those items. When a preference is unlocked, group administrators can reconfigure it for ```<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level"> their groups</MadCap:conditionalText>```.

For instructions on locking or unlocking a system-level project, task, or issue preference, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>After a Workfront administrator unlocks a preference at the system level, any group administrator can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a Workfront administrator has to configure and lock a preference for everyone in the system. For more information, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) and [Lock or unlock a project, task, or issue preference for subgroups](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Unlock a project preference so that groups can configure it

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Project Preferences**, then click **Projects**.

1. Do any of the following:

   * If you want group administrators to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
   * If you want all groups to use your configuration for a preference, make sure that it is locked (this is the default).   
   
     >[!IMPORTANT]
     >
     >We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that group administrators might have made.

1. Click **Save**.

