



# Email notifications {#email-notifications}

`Workfront` sends out a number of email notifications to alert users about activity in `Workfront` and provide useful information and links. For information about all `Workfront` notifications and how they are enabled, see [Workfront notifications](workfront-notifications.md).


`Workfront` sends email notifications from the email address which your `Workfront administrator` selected to handle your outgoing emails. For information on setting up the outgoing emails for `Workfront`, see [Configure outgoing email](configure-outgoing-email.md).


## `Workfront` email notifications overview {#workfront-email-notifications-overview}

`Workfront` comes with a set of predefined event notifications that can be enabled by the `Workfront administrator`. These event notifications trigger email communication every time the condition defined by the event is met. For more information about enabling event notifications at the system level, see [Enable and disable event notifications](enable-and-disable-event-notification.md).


All users are eligible to receive email notifications from `Workfront`. However, the rules of an individual object&nbsp;restrict whether a user&nbsp;is eligible to receive a notification, based on their access&nbsp;level and their notification settings. To view restrictions for email notifications, see [Configure email notifications](configure-email-notifications.md).


After the event notifications are enabled by your `Workfront administrator`, you can select which ones you would like to receive by editing your Notifications preferences in your user profile. You can also choose whether you want to receive notifications as events happen, or if&nbsp;you want to receive events summarized in one daily digest email.


For more information about configuring email notifications based on events in `Workfront`, see [Configure email notifications](configure-email-notifications.md).


>[!NOTE]
>
>Event notifications are the only notifications that can be configured to be delivered in daily digest updates.


The following categories&nbsp;of the notification settings are enabled for daily digest emails by default. For more information about each notification category, click on the links..


Depending on how the `Workfront administrator` has configured event notifications for your `Workfront` system (as described in [Enable and disable event notifications](enable-and-disable-event-notification.md)), you might see only a subset these notifications in your settings.



* [Notifications: Action needed](notifications-action-needed.md) 
* [Notifications: Requests I have made](notifications-requests-i-have-made.md) 
* [Notifications: Communication](notifications-communication.md) 
* [Notifications: Approval information](notifications-approval-information.md) 
* [Notifications: Information about work assigned to me](notifications-information-about-work-assigned-to-me.md) 
* [Notifications: Information about projects I'm on](notifications-information-about-projects-im-on.md) 
* [Notifications: Information about projects I own](notifications-information-about-projects-i-own.md) 
* [Notifications: Information about projects I sponsor](notifications-information-about-projects-i-sponsor.md) 
* [Notifications: Miscellaneous information](notifications-misc-information.md) 


The default status shows which notifications (daily, instant, or both) are enabled by default for new users when you create the new users. 


>[!NOTE]
>
>If you want to receive email notifications from the Sandbox environment, you must&nbsp;enable emails from your user profile in that environment.&nbsp;




## Instant notifications {#instant-notifications}

Depending on the how your email is configured, you might receive an instant notification when a predefined event occurs. For more information on instant notifications, see [Configure email notifications](configure-email-notifications.md) and [Enable and disable event notifications](enable-and-disable-event-notification.md).


## Daily digest notifications {#daily-digest-notifications}

There are several things to be aware of when receiving daily digest notifications:



*  Each notifications section in your **My Settings** panel generates its own daily digest email. You can have as many daily digest emails every day as notification settings that are enabled&nbsp;for daily digest emails.  
  For example, if you selected to receive a daily digest email for several actions under the **Information about Projects I&nbsp;Own,&nbsp;**you receive one email notification listing all the events met for this area. 

*   Notifications in a daily digest email are grouped by various criteria. For example, in the case of **Information about Projects I&nbsp;Own**, the events are grouped by the project name.


  For the **Communication** category, the notifications are grouped by the object where the communication happened.&nbsp;

* The daily digest email lists events that happened for the actions&nbsp;in one particular area (like **Information about projects I Own**) within the 24 hours prior to the time chosen for delivery.&nbsp;
* The timezone for the time selected for daily digest delivery matches&nbsp;your timezone, as it is configured on your browser.&nbsp;
* The daily digest emails have the name of the section in the subject line, as well as the date on which they are delivered.
* At least one event must trigger a notification&nbsp;in order for the daily digest to be delivered. Daily digests are not sent if no events marked for daily digest emails are met.


The following example&nbsp;is the email&nbsp;you receive&nbsp;when you sign up for daily digest notifications for the&nbsp;**Information about Projects I Own**&nbsp;category:


## Notification of posted comments {#notification-of-posted-comments}

The notifications in the Communication category alert you to&nbsp;comments that have been posted in the Update stream of a specific item.&nbsp;


Daily digest emails for the Communication category are selected for all notifications available.&nbsp;


The information is summarized for the object where the communication happened, and a total number of communication messages is displayed for each object.&nbsp;


For more information about configuring email notifications, see [Configure email notifications](configure-email-notifications.md).


For instructions on commenting on Communication emails, see [Update work](update-work.md).


To learn more about Communication emails, see [Configure email notifications](configure-email-notifications.md).


&nbsp;For more information about enabling daily digest notifications, see [Configure email notifications](configure-email-notifications.md).


## Automatic reminders {#automatic-reminders}

Automatic reminders are enabled by your `Workfront administrator` to alert you of tasks and issues that are either past due and incomplete, or that are approaching a deadline. For more information about enabling automatic reminders, see [Set up automatic reminders](setting-up-automatic-reminders.md).


Automatic reminder emails are sent from the email address that your `Workfront administrator` selected&nbsp;to handle your outgoing emails.   
For more information on setting up the outgoing emails for `Workfront`, see [Configure outgoing email](configure-outgoing-email.md).


Depending which automatic reminder is activated, the following kinds of information are available in the automatic reminder email:



* The date when the task or issue was created.
* Task or issue name.
* The name of the project where the task or issue resides.&nbsp;
* Description of task or issue.&nbsp;
* A list of users assigned to the task or issue.
* The name of the user who entered the task or issue.
* The priority of the task or issue.
* Date when the task or issue became overdue.




## Reminder notifications {#reminder-notifications}

Your `Workfront administrator` can design reminder notifications and attach them to the following objects:



* Tasks
* Issues
* Projects
* Timesheets


Reminder notifications are custom emails that alert you of&nbsp;approaching deadlines for your items.


>[!IMPORTANT] {type="important"}
>
>If the deadline changes after you receive a reminder notification for any of the objects mentioned above, you do not receive another reminder notification.


Users with a Plan license and administrative access to Reminder Notifications can also create and enable Reminder Notifications. For more information about giving a Plan user administrative access, see [Assign users administrative access](assign-users-administrative-access.md).


For more information about setting up and enabling reminder notifications, see [Set up reminder notifications](set-up-reminder-notifications.md).


Reminder notifications are sent from the email address that your `Workfront administrator` selected&nbsp;to handle your outgoing emails.   
For more information on setting up the outgoing emails for `Workfront`, see [Configure outgoing email](configure-outgoing-email.md).


## Other `Workfront` emails {#other-workfront-emails}

There are other emails you might receive from `Workfront` which cannot be configured. The following emails are automatically sent by `Workfront` when these conditions are met:



* Restore an item: When the `Workfront administrator` restores an object from the Recycle Bin, an email is sent to the `Workfront administrator`.

* Failed to be restored: When the `Workfront administrator` attempts to restore an object from the Recycle Bin, and the restore fails, an email is sent to the `Workfront administrator`. &nbsp;

* Global POP email configuration problem detected: This email is generated as a result of `Workfront` having trouble connecting to a POP account which is configured to allow users to reply to email notifications. For more information about how you can allow users to reply to `Workfront` email notifications, see [Use a POP email account to comment on work items](using-pop-email-reply.md).  
  If `Workfront` connects to the POP account and it finds 10 emails in the POP account that are not related to comments in `Workfront`, it stops processing the rest of the emails and sends a notification to the `Workfront administrator`.  
  For more information about the message sent when `Workfront` cannot process emails from the POP account, see the [Understanding the Automatic Disconnect of a POP Account](using-pop-email-reply.md#understanding-the-automatic-disconnect-of-a-pop-account) section in [Use a POP email account to comment on work items](using-pop-email-reply.md).



The following emails can only be configured at the user profile level. They cannot be enabled or disabled&nbsp;at the system level:



* Completion of personal task: when a personal task you assigned to someone else is completed, you will receive an email.&nbsp;
* Comment added to user: when someone comments on your user profile, you will receive an email.&nbsp;




## Email notifications in the mobile email App {#email-notifications-in-the-mobile-email-app}

You can receive `Workfront` email notifications in your mobile email app, on your mobile device.  



If you have the `Workfront` Mobile App installed on your phone, tapping the links in the email opens them in the `Workfront` Mobile App. This includes tapping any of the following action buttons:



* Work On It
* Comment
* Make Approval Decision
* See All Notifications
* Add&nbsp;
* Get Started
* See More Details


For more information about the `Workfront` Mobile App, see [Use the Workfront Mobile App](use-the-mobile-app.md).  

