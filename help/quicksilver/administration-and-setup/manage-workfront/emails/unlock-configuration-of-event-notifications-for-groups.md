---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Unlock or lock configuration of event notifications for all groups
description: If you are an Adobe Workfront administrator, you can unlock or re-lock the ability for group administrators to configure an event notification for top-level groups they manage. Configuration of an event notification consists of activating or deactivating it.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
---
# Unlock or lock configuration of event notifications for all groups

If you are an Adobe Workfront administrator, you can unlock or re-lock the ability for group administrators to configure an event notification for top-level groups they manage. Configuration of an event notification consists of activating or deactivating it.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

When an administrator configures an event notification for a group, the configuration affects users for whom that group, or one of its subgroups, is their Home Group. In their user profiles, these users see the event notifications that are activated for their Home Group instead of the event notifications that are activated system-wide. For more information, see [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* A Workfront administrator can unlock and re-lock configuration for an event notification in both Adobe Workfront Classic and the new Adobe Workfront experience. But a group administrator can configure that event notification for a group only in the new Adobe Workfront experience. Group administrators using Adobe Workfront Classic can switch to the new Adobe Workfront experience to configure unlocked event notifications for a group, then switch back to Adobe Workfront Classic to see the changes in effect.
>* Subgroups inherit group-level event notification configurations from the top-level groups above them.
>

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Unlock or re-lock the ability to configure an event notification

>[!IMPORTANT]
>
>When you re-lock a notification, all groups in the system inherit the notification exactly as you set it. This overrides any changes that group administrators might have made for their groups, so it's a good idea to consult with them first.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Email** > **Notifications**.

1. Make sure the **Event Notifications** tab is open.
1. Click the icon to the right of the notification to switch it to the locked ![Lock icon](assets/lock-toggle-button.png) or unlocked ![Unlock icon](assets/unlock-toggle-button.png) position.

   Or

   If you want to unlock or lock multiple notifications all at once, select them, then click the Unlock ![Unlock icon](assets/unlock-icon-toolbar.png) or Lock ![Lock icon](assets/lock-icon-locked-qs.png) button that displays in the toolbar above the list.

1. Click **Save**.
1. (Optional) If you want to configure the event notification for a top-level group instead of leaving this task to the group's administrator, you can do one of the following:

   * Delete **System Event Notifications** in the search box above the list of notifications, search for and select the name of the top-level group to list its notifications, then activate or inactivate the unlocked notifications in the list that displays.
   * Click **Groups** in the left menu, then click the name of the top-level group. Click **Event Notifications** in the left panel, then configure the unlocked event notification, as explained in [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
