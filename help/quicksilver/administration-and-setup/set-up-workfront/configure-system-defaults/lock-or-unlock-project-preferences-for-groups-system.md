---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Lock or Unlock Project Preferences for All Groups in the System
description: Groups in your organization might need a project preference configured differently for their unique workflows. You can unlock the preference for all groups throughout the organization so that they can configure it on their own.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
---
# Lock or unlock project preferences for all groups in the system

Groups in your organization might need a project preference configured differently for their unique workflows. You can unlock the preference for all groups throughout the organization so that they can configure it on their own.

When a preference is unlocked and the group administrator modifies it, the projects associated with the group acquire the configuration for that preference from the group-level setting instead of from the system-level setting.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## About locked and unlocked preferences

Locking a project, task, or issue preference that you have configured at the system level ensures that everyone is using the same setting for that preference. Though you can still reconfigure a preference that you lock, group administrators can't reconfigure it for their groups.

Conversely, unlocking a project, task, or issue preference allows group administrators more flexibility to manage the way their groups work with those items. When a preference is unlocked, group administrators can reconfigure it for their groups.

If a field does not have a lock/unlock toggle, then it cannot be unlocked for group administrators to configure settings at the group level. Configuration is only available at the system level.

For instructions on locking or unlocking a system-level project, task, or issue preference, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>After a [!DNL Workfront] administrator unlocks a preference at the system level, any group administrator can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a [!DNL Workfront] administrator has to configure and lock a preference for everyone in the system. For more information, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) and [Lock or unlock a project, task, or issue preference for subgroups](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Unlock a project preference so that groups can configure it

{{step-1-to-setup}}

1. Click **[!UICONTROL Project Preferences]**, then click **[!UICONTROL Projects]**.

1. Do any of the following:

   * If you want group administrators to be able to configure a preference for their groups, unlock it ![Unlock toggle](assets/unlock-toggle-button.png).
   * If you want all groups to use your configuration for a preference, make sure that it is locked (this is the default).

      >[!IMPORTANT]
      >
      >We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that group administrators might have made.

1. Click **[!UICONTROL Save]**.
