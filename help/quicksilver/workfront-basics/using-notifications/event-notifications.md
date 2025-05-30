---
content-type: overview
navigation-topic: notifications
title: Event notifications
description: Event notifications are emails triggered by various types of events on objects such as projects, tasks, or issues. They are sent when something occurs on the project that others need to know about. Depending on the event, users receive instant, daily, or both instant and daily email notifications about it.
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
---
# Event notifications

 <!-- Audited: 4/2025 -->

Event notifications are emails triggered by various types of events on objects such as projects, tasks, or issues. They are sent when something occurs on the project that others need to know about. Depending on the event, users receive instant, daily, or both instant and daily email notifications about it.

>[!NOTE]
>
>Event notifications are one of several types of [!DNL Adobe Workfront] notifications. For information about all [!DNL Workfront] notification types, see [Notifications overview](../../workfront-basics/using-notifications/wf-notifications.md).

## Configuring event notifications

Event notification emails can be configured at the following levels:

* **System level**: A [!DNL Workfront] administrator can activate and deactivate event notifications at the system level, as explained in [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   All groups inherit system notifications by default, but group administrators might be able to change some configurations on the group level if allowed by the [!DNL Workfront] administrator.

* **Group level**: A group administrator can configure an event notification for groups they manage after a [!DNL Workfront] administrator unlocks this ability for groups. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for [!DNL Workfront] administrators (for any group). For more information, see [View and configure event notifications for a group](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

* **User level**: All of the event notifications that are activated system-wide are listed in each user's [!UICONTROL Notifications] section on their individual profile. Users can activate and deactivate their individual event notifications there.

   [!DNL Workfront] administrators and users with access to edit other users can also activate and deactivate notifications in an individual user's profile.

   For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >User-level notifications also include [!DNL Workfront Goals] notifications. However, the [!DNL Workfront] administrator or the group administrator cannot configure notifications for [!DNL Workfront Goals]. Each use must configure their own [!DNL Workfront Goals] notifications in their profile. If you have access to edit users, you can also modify these notifications for others. For enabling [!DNL Workfront Goals] notifications for your profile or for other users that you have access to edit, see [Notifications: Goals](../../workfront-basics/using-notifications/notifications-goals.md).

   For more information about what notifications the [!DNL Workfront] administrator can configure, see [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). 

## Event notification content

An event notification email contains information about the event that took place and contains a link to [!DNL Workfront] where you can see the event in the system. For more information about receiving email notifications, see [Notifications overview](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] administrator can't change email notification content as it's configured by [!DNL Workfront], but they can change event notification email subject lines. For more information, see [Customize email subjects for event notifications](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

For a list all of the [!DNL Workfront] event notifications, along with a brief description of each event, and whether it is active or inactive by default, see [Event notification types](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
