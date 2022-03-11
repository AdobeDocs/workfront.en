---
filename: unlock-configuration-of-event-notifications-for-groups
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Unlock or lock configuration of event notifications for all groups
description: If you are an Adobe Workfront administrator, you can unlock or re-lock the ability for group administrators to configure an event notification for top-level groups they manage. Configuration of an event notification consists of activating or deactivating it.
---

# Unlock or lock configuration of event notifications for all groups

If you are an `Adobe Workfront administrator`, you can unlock or re-lock the ability for `group administrators` to configure an event notification for top-level groups they manage. Configuration of an event notification consists of activating or deactivating it.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for `Workfront administrators` (for any group).

When an administrator configures an event notification for a group, the configuration affects users for whom that group, or one of its subgroups, is their Home Group. In their user profiles, these users see the event notifications that are activated for their Home Group instead of the event notifications that are activated system-wide. For more information, see [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* A `Workfront administrator` can unlock and re-lock configuration for an event notification in both `Adobe Workfront Classic` and `the new Adobe Workfront experience`. But a `group administrator` can configure that event notification for a group only in `the new Adobe Workfront experience`. `Group administrators` using `Adobe Workfront Classic` can switch to `the new Adobe Workfront experience` to configure unlocked event notifications for a group, then switch back to `Adobe Workfront Classic` to see the changes in effect.
>
>* Subgroups inherit group-level event notification configurations from the top-level groups above them.
>

## Access requirements

You must have the following access to perform the steps in this article:

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
>When you re-lock a notification, all groups in the system inherit the notification exactly as you set it. This overrides any changes that `group administrators` might have made for their groups, so it’s a good idea to consult with them first.

<ol data-mc-continue="false"> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Email</span> > <span class="bold">Notifications</span>.</li> 
 <li value="3"> Make sure the <span class="bold">Event Notifications</span> tab is open.</li> 
 <li value="4"> <p>Click the icon to the right of the notification to switch it to the unlocked <img src="assets/lock-toggle-button.png"> or locked <img src="assets/unlock-toggle-button.png"> position.</p> <p>Or</p> <p>If you want to unlock or lock multiple notifications all at once, select them, then click the Unlock <img src="assets/unlock-icon-toolbar.png"> or Lock <img src="assets/lock-icon-locked-qs.png"> button that displays in the toolbar above the list.</p> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> (Optional) If you want to configure the event notification for a top-level group instead of leaving this task to the group’s administrator, you can do one of the following: Delete System Event Notifications in the search box above the list of notifications, search for and select the name of the top-level group to list its notifications, then activate or inactivate the unlocked notifications in the list that displays. Click Groups in the left menu, then click the name of the top-level group. Click Event Notifications in the left panel, then configure the unlocked event notification, as explained in View and configure event notifications for a group. 
</ol>

