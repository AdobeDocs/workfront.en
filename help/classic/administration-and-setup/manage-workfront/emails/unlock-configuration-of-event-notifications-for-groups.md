---
filename: unlock-configuration-of-event-notifications-for-groups
user-type: administrator
product-area: system-administration
keywords: unlock,event,notifications,groups,email,group
navigation-topic: emails-administration
title: Unlock or lock configuration of event notifications for all groups
description: If you are an Adobe Workfront administrator, you can unlock or re-lock the ability for group administrators to configure an event notification for top-level groups they manage. Configuration of an event notification consists of activating or deactivating it.
---

# Unlock or lock configuration of event notifications for all groups

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

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
   <td> <p>Plan</p> </td> 
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
>When you re-lock a notification, all groups in the system inherit the notification exactly as you set it. This overrides any changes that group administrators might have made for their groups, so it’s a good idea to consult with them first.

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. Click **Email** > **Notifications**.

1. Make sure the **Event Notifications** tab is open.
1. Click the icon to the right of the notification to switch it to the unlocked ![](assets/lock-toggle-button.png) or locked ![](assets/unlock-toggle-button.png) position.

   Or

   If you want to unlock or lock multiple notifications all at once, select them, then click the Unlock ![](assets/unlock-icon-toolbar.png) or Lock ![](assets/lock-icon-locked-qs.png) button that displays in the toolbar above the list.

1. Click **Save**.
1. (Optional) If you want to configure the event notification for a top-level group instead of leaving this task to the group’s administrator, do the following:

   1. Delete **System Event Notifications** in the box near the upper-right corner.
   1. Start typing the name of the group in the box, then click it’s name when it appears.
   1. In the list that displays, configure the unlocked notifications, as explained in [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

