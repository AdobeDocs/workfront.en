---
filename: wf-notifications
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront notifications
description: Adobe Workfront sends email notifications, in-app notifications, and notifications on your mobile device.
---

# Adobe Workfront notifications

Adobe Workfront sends email notifications, in-app notifications, and notifications on your mobile device.

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

## Email notifications

Workfront sends out a number of email notifications to alert users about activity in Workfront and provide useful information and links.

>[!NOTE]
>
>If you want to receive email notifications from the Sandbox environment, you must enable emails from your user profile in that environment.

You can receive the following email notifications from Workfront:

* [Event notifications](#understanding-instant-and-daily-digest-notifications) 
* [Daily digest notifications](#daily) 
* [Notification of posted comments](#notifica) 
* [Automatic reminders](#automatic-reminders) 
* [Reminder notifications](#reminder-notifications) 
* [Other Workfront emails](#other) 
* [Email notifications from Workfront Goals](#workfront-align)

### Event notifications

Event notifications are predefined in Workfront. They are usually triggered by certain events.

After the event notifications are activated by your Workfront administrator or group administrator, you can select which ones you would like to receive by editing your Notifications preferences in your user profile. You can also choose whether you want to receive notifications as events happen, or if you want to receive events summarized in one daily digest email.

Depending on how the Workfront administrator has configured event notifications for your Workfront system (as described in [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)), you might see only a subset of these notifications in your settings.

The default status shows which notifications (daily, instant, or both) are enabled by default for new users when you create the new users.

For a full list of the event notifications, and information about how they are enabled and configured at the system level, group level, or user level, see [Event notifications available in Adobe Workfront](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

For information about how to choose which event notifications you want to receive, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Event notifications are the only notifications that can be configured to be delivered in daily digest updates.

### Daily digest notifications

For a complete list of what email notifications have been enabled for a daily digest email delivery as well as information about all the categories for email notifications, see [Event notifications](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>Workfront does not send any Daily digest notifications for the Miscellaneous category  of events. You cannot disable the Daily notifications for this category .

There are several things to be aware of when receiving daily digest notifications:

* Each notifications section in your **My Settings** panel generates its own daily digest email. You can have as many daily digest emails every day as notification settings that are enabled&nbsp;for daily digest emails.  
  For example, if you selected to receive a daily digest email for several actions under the **Information about Projects I Own,**you receive one email notification listing all the events met for this area. 

* Notifications in a daily digest email are grouped by various criteria. For example, in the case of **Information about Projects I Own**, the events are grouped by the project name.

  For the **Communication** category, the notifications are grouped by the object where the communication happened.

* The daily digest email lists events that happened for the actions&nbsp;in one particular area (like **Information about projects I Own**) within the 24 hours prior to the time chosen for delivery.
* The timezone for the time selected for daily digest delivery matches&nbsp;your timezone, as it is configured on your browser.
* The daily digest emails have the name of the section in the subject line, as well as the date on which they are delivered.
* At least one event must trigger a notification&nbsp;in order for the daily digest to be delivered. Daily digests are not sent if no events marked for daily digest emails are met.

### Notification of posted comments

The notifications in the Communication category alert you to comments that have been posted in the Update stream of a specific item.

Daily digest emails for the Communication category are selected for all notifications available.

The information is summarized for the object where the communication happened, and a total number of communication messages is displayed for each object.

For more information about configuring email notifications, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

For instructions on commenting on Communication emails, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

To learn more about Communication emails, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

For more information about enabling daily digest notifications, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatic reminders

Automatic reminders are enabled by your Workfront administrator to alert you of tasks and issues that are due, late, or near the planned completion date. For late notifications, the email is sent nightly until the task or issue is completed. After the administrator configures these, you cannot disable them. Also, you cannot change the content or the subject line of an email triggered by an automatic reminder.

They can be sent to one or more of the following:

* The users assigned to a task or issue
* The user's immediate manager
* The manager of the immediate manager

Automatic reminder emails are sent from the email address that your Workfront administrator selected to handle outgoing emails.

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

A Workfront administrator (or a user with a Planner access level and administrative access to reminder notifications) can design reminder notifications about approaching deadlines and attach them to projects, tasks, issues, and timesheets. For more information about how you can get the required administrative access, see [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>If the deadline changes after a user receives a reminder notification for any of the objects mentioned above, the user doesn’t receive another reminder notification.

Reminder notifications&nbsp;are sent from the email address that the Workfront administrator selected to handle outgoing emails.

For information about setting up and enabling reminder notifications, see [Set up reminder notifications](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### Other Workfront emails

There are other emails you might receive from Workfront which cannot be configured. The following emails are automatically sent by Workfront when these conditions are met:

* Restore an item: When the Workfront administrator restores an object from the Recycle Bin, an email is sent to the Workfront administrator.
* Failed to be restored: When the Workfront administrator attempts to restore an object from the Recycle Bin, and the restore fails, an email is sent to the Workfront administrator.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Global POP email configuration problem detected: This email is generated as a result of Workfront having trouble connecting to a POP account which is configured to allow users to reply to email notifications. For more information about how you can allow users to reply to Workfront email notifications, see .<br>If Workfront connects to the&nbsp;POP account and it finds 10 emails in the POP account that are not&nbsp;related to comments in Workfront, it stops&nbsp;processing the rest of the emails and sends a notification to the Workfront administrator.<br>For more information about the message sent when Workfront cannot process emails from the POP account, see the section in .</li>
  -->

The following emails can only be configured at the user profile level. They cannot be enabled or disabled&nbsp;at the system level:

* Completion of personal task: when a personal task you assigned to someone else is completed, you will receive an email.&nbsp;
* Comment added to user: when someone comments on your user profile, you will receive an email.&nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3><a name="workfront-align"></a>Email notifications from Workfront Goals</h3>
<div class="workfront_plans">
<p>Your organization must have the following to use the functionality described in this article: </p>
<ul>
<li> <p>A Pro or higher <a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>. </p> </li>
<li> <p>An Adobe Workfront Goals license in addition to a Workfront license.</p> <p>Contact your Workfront account manager to learn about a Workfront Goals license. </p> <p>Workfront Goals is available only in the new Adobe Workfront experience. </p> </li>
</ul>
<p>For additional information about access to Workfront Goals, see Access needed to use Workfront Goals.</p>
</div>
<p>If you are a Workfront Goals user, you can configure notifications for yourself to receive communication about events happening in that area. For information, see Enable Adobe Workfront Goals notifications.</p>
</div>
-->

## In-app notifications

You can receive notifications inside the Workfront web application, when certain events happen.&nbsp;

For more information about in-app notifications, see [View and manage in-app notifications](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Email notifications in the mobile email app

You can receive Workfront email notifications in your mobile email app, on your mobile device.

If you have the Workfront Mobile App installed on your phone, tapping the links in the email opens them in the Workfront Mobile App. This includes tapping any of the following action buttons:

* Work On It
* Comment
* Make Approval Decision
* See All Notifications
* Add
* Get Started
* See More Details

For more information about the Workfront Mobile App, see [Use the Adobe Workfront mobile app](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
