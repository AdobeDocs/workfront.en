---
filename: event-notifications
content-type: overview
navigation-topic: notifications
title: Event notifications
description: Event notifications are emails triggered by various types of events on objects such as projects, tasks, or issues. They are sent when something occurs on the project that others need to know about. Depending on the event, users receive instant, daily, or both instant and daily email notifications about it.
---

# Event notifications

Event notifications are emails triggered by various types of events on objects such as projects, tasks, or issues. They are sent when something occurs on the project that others need to know about. Depending on the event, users receive instant, daily, or both instant and daily email notifications about it.

>[!NOTE]
>
>Event notifications are one of several types of `Adobe Workfront` notifications. For information about all `Workfront` notification types, see [Adobe Workfront notifications](../../workfront-basics/using-notifications/wf-notifications.md).

## Configuring event notifications

Event notification emails can be configured at the following levels listed below. Configuration of an event notification consists of activating or deactivating it.

<ul> 
 <li> <p><span class="bold">System level</span>: A <span>Workfront administrator</span> can activate and deactivate event notifications at the system level, as explained in <a href="../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref" xrefformat="{para}">Configure event notifications for everyone in the system</a>.</p> <p>All groups inherit system notifications by default, but <span>group administrators</span> might be able to change some configurations on the group level, if allowed by the <span>Workfront administrator</span>, as explained in the next bullet item below.</p> </li> 
 <li> <p><span class="bold">Group level</span>: A <span>group administrator</span> can configure an event notification for groups they manage after a <span>Workfront administrator</span> unlocks this ability for groups. (missing or bad snippet) For more information, see <a href="view-and-configure-event-notifications-group.md" class="MCXref xref" xrefformat="{para}">View and configure event notifications for a group</a>.</p> <note type="note">
   This functionality is available initially only to customers on Cluster 4 as part of a phased roll-out. It will become available for other clusters shortly thereafter. This article will be updated as this occurs.
  </note> </li> 
 <li> <p><span class="bold">User level</span>: All of the event notifications that are activated system-wide are listed in each user's Notifications section on their individual profile. Users can activate and deactivate their individual event notifications there.</p> <p><span>Workfront administrators</span> and users with access to edit other users can also activate and deactivate notifications in the profile of individual users.</p> <p>For more information, see <a href="../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md" class="MCXref xref" xrefformat="{para}">Activate or deactivate your own event notifications</a>.</p> <note type="note">
   User-level notifications also include 
   <span>Workfront Goals</span> notifications. However, the 
   <span>Workfront administrator</span> or the 
   <span>group administrator</span> cannot configure notifications for 
   <span>Workfront Goals</span>. Each use must configure their own 
   <span>Workfront Goals</span> notifications in their profile. If you have access to edit users you can also modify these notifications for others. For enabling 
   <span>Workfront Goals</span> notifications for your profile or for other users that you have access to edit, see
   <a href="../../workfront-basics/using-notifications/notifications-goals.md" class="MCXref xref" xrefformat="{para}">Notifications: Goals</a>.
  </note> <p>For more information about what notifications the <span>Workfront administrator</span>can configure, see <a href="../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref" xrefformat="{para}">Configure event notifications for everyone in the system</a>. <span>Workfront Goals</span>are available only in<span>The new Adobe Workfront experience</span>.</p> </li> 
</ul>

## Event notification content

An event notification email contains information about the event that took place and contains a link to `Workfront` where you can see the event in the system. For more information about receiving email notifications, see [Adobe Workfront notifications](../../workfront-basics/using-notifications/wf-notifications.md).

A `Workfront administrator` cannot change the content of the email notifications, as they are configured by `Workfront`. However, they can change the subject lines of event notifications emails. For more information, see [Customize email subjects for event notifications](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

For a list all of the `Workfront` event notifications, along with a brief description of each event, and whether it is active or inactive by default, see [Event notifications available in Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
