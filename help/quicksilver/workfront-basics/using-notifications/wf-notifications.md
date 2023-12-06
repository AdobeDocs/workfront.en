---
content-type: overview;reference
navigation-topic: notifications
title: Notifications overview
description: Adobe Workfront sends email notifications, in-app notifications, and notifications on your mobile device.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
---
# Notifications overview

[!DNL Adobe Workfront] sends email notifications, in-app notifications, and notifications on your mobile device.

## Email notifications

[!DNL Workfront] sends email notifications to alert users about activity in Workfront, and provide useful information and links.

To change the preferences for your email notifications, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>If you want to receive email notifications from the Sandbox environment, you must enable emails from your user profile in that environment.

You can receive the following email notifications from [!DNL Workfront]:

* [Event notifications](#event-notifications)
* [Daily digest notifications](#daily-digest-notifications)
* [Notification of posted comments](#notification-of-posted-comments)
* [Automatic reminders](#automatic-reminders)
* [Reminder notifications](#reminder-notifications)
* [Boards notifications](#boards-notifications)
* [Other [!DNL Workfront] emails](#other-workfront-emails)

### Event notifications 

Event notifications usually triggered by certain predefined events, such as having a task assigned to you or getting a reply on a comment you made.

After event notifications are activated in your [!DNL Workfront] system by your [!DNL Workfront] administrator or group administrator, you can select which ones you would like to receive by editing your [!UICONTROL Notifications] preferences in your user profile. You can also choose whether you want to receive notifications as events happen, or if you want to receive events summarized in one daily digest email.

Depending on how the [!DNL Workfront] administrator has configured event notifications for your [!DNL Workfront] system (as described in [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)), you might see only a subset of these notifications in your settings.

The default status shows which notifications (daily, instant, or both) are enabled by default for new users when you create the new users.

For a full list of the event notifications, and information about how they are enabled and configured at the system level, group level, or user level, see [Event notifications available in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

For information about how to choose which event notifications you want to receive, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Event notifications are the only notifications that can be configured to be delivered in daily digest updates.

### Daily digest notifications 

For a complete list of what email notifications have been enabled for a daily digest email delivery as well as information about all the categories for email notifications, see [Event notifications](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] does not send any Daily digest notifications for the [!UICONTROL Miscellaneous] and [!DNL Goals] categories of events. You cannot disable the Daily notifications for these categories.

There are several things to be aware of when receiving daily digest notifications:

* Each [!UICONTROL notifications] section in your **[!UICONTROL My Settings]** panel generates its own daily digest email. You can have as many daily digest emails every day as notification settings that are enabled for daily digest emails.\
   For example, if you selected to receive a daily digest email for several actions under the **[!UICONTROL Information about Projects I] Own,** you receive one email notification listing all the events met for this area.

* Notifications in a daily digest email are grouped by various criteria. For example, in the case of **[!UICONTROL Information about Projects I Own]**, the events are grouped by the project name.

   For the **[!UICONTROL Communication]** category, the notifications are grouped by the object where the communication happened.

* The daily digest email lists events that happened for the actions in one particular area (like **Information about projects I Own**) within the 24 hours prior to the time chosen for delivery.
* The timezone for the time selected for daily digest delivery matches your timezone, as it is configured on your browser.
* The daily digest emails have the name of the section in the subject line, as well as the date on which they are delivered.
* At least one event must trigger a notification in order for the daily digest to be delivered. Daily digests are not sent if no events marked for daily digest emails are met.

### Notification of posted comments 

The notifications in the [!UICONTROL Communication] category alert you to comments that have been posted in the [!UICONTROL Update] stream of a specific item.

Daily digest emails for the [!UICONTROL Communication] category are selected for all notifications available.

The information is summarized for the object where the communication happened, and a total number of communication messages is displayed for each object.

For more information about configuring email notifications, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

For instructions on commenting on [!UICONTROL Communication] emails, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

To learn more about [!UICONTROL Communication] emails, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

For more information about enabling daily digest notifications, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatic reminders

Automatic reminders are enabled by your [!DNL Workfront] administrator to alert you of tasks and issues that are due, late, or near the planned completion date. For late notifications, the email is sent nightly until the task or issue is completed. After the administrator configures these, you cannot disable them. Also, you cannot change the content or the subject line of an email triggered by an automatic reminder.

They can be sent to one or more of the following:

* The users assigned to a task or issue
* The user's immediate manager
* The manager of the immediate manager

Automatic reminder emails are sent from the email address that your [!DNL Workfront] administrator selected to handle outgoing emails.

Depending which automatic reminder is activated, the following kinds of information are available in the automatic reminder email:

* The date when the task or issue was created
* Task or issue name
* The name of the project where the task or issue resides
* Description of task or issue
* A list of users assigned to the task or issue
* The name of the user who entered the task or issue
* The priority of the task or issue
* Date when the task or issue became overdue

For information about enabling automatic reminders, see [Set up automatic reminders](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Reminder notifications 

A [!DNL Workfront] administrator (or a user with a [!UICONTROL Planner] access level and administrative access to reminder notifications) can design reminder notifications about approaching deadlines and attach them to projects, tasks, issues, and timesheets. For more information about how you can get the required administrative access, see [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>If the deadline changes after a user receives a reminder notification for any of the objects mentioned above, the user doesn't receive another reminder notification.

Reminder notifications are sent from the email address that the [!DNL Workfront] administrator selected to handle outgoing emails.

For information about setting up and enabling reminder notifications, see [Set up reminder notifications](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### Boards notifications

[!DNL Adobe Workfront] [!UICONTROL Boards] sends you an email when you are added to a board and when a card is assigned to you.

You can select which emails you want to receive in your Boards preferences. For more information, see [Boards email notifications and preferences](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Other [!DNL Workfront] emails 

There are other emails you might receive from [!DNL Workfront] which cannot be configured. The following emails are automatically sent by [!DNL Workfront] when these conditions are met:

* Restore an item: When the [!DNL Workfront] administrator restores an object from the [!UICONTROL Recycle] Bin, an email is sent to the [!DNL Workfront] administrator.
* Failed to be restored: When the [!DNL Workfront] administrator attempts to restore an object from the Recycle Bin, and the restore fails, an email is sent to the [!DNL Workfront] administrator.

The following emails can only be configured at the user profile level. They cannot be enabled or disabled at the system level:

* Completion of personal task: when a personal task you assigned to someone else is completed, you will receive an email.
* Comment added to user: when someone comments on your user profile, you will receive an email.

## In-app notifications

You can receive notifications inside the [!DNL Workfront] web application, when certain events happen.

For more information about in-app notifications, see [View and manage in-app notifications](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Email notifications in the mobile email app

You can receive [!DNL Workfront] email notifications in your mobile email app, on your mobile device.

If you have the [!DNL Workfront] Mobile App installed on your phone, tapping the links in the email opens them in the [!DNL Workfront] Mobile App. This includes tapping any of the following action buttons:

* [!UICONTROL Work On It]
* [!UICONTROL Comment]
* [!UICONTROL Make Approval Decision]
* [!UICONTROL See All Notifications]
* [!UICONTROL Add]
* [!UICONTROL Get Started]
* [!UICONTROL See More Details]

For more information about the [!DNL Workfront] Mobile App, see [Use the [!DNL Adobe Workfront] mobile app](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
