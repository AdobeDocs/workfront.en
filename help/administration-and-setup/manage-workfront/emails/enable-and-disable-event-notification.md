



# Enable and disable event notifications {#enable-and-disable-event-notifications}

As a `Workfront administrator`, you can enable event notifications that send email notifications for various types of events in your organization.


Users can enable or disable their own email notifications, as described in [Configure email notifications](configure-email-notifications.md).


## Configure event&nbsp;notifications for all users {#configure-event-notifications-for-all-users}




1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Click **Email** > **Notifications**.

1.  On the **Event Notifications** tab, select the check box to the left of the event type for which you want to enable or disable notifications.
1.   Above the list of event types, click **Activate** or **Deactivate**.   



   A check mark displays in the **Active** column next to event types where notifications are enabled.   



   To see the default notification status for an event, see [Event Notifications Descriptions and Default Statuses](#event-notification-descriptions-and-default-statuses)&nbsp;below. 

1.  (Optional) Click the name of an event notification to customize the subject line of the email notification.   



   For more information about customizing the subject lines of email notifications, see [Customize email subjects for event notifications](custom-email-subjects-event-notification.md).





## Modify email notification settings in bulk {#modify-email-notification-settings-in-bulk}

If you are a `Workfront administrator` or you have a plan license allowing you to edit other users' settings, you can configure the notification settings for multiple users at one time. This includes specifying whether users receive notifications as events happen or in one daily digest email (see [Email notifications](email-notifications.md)).&nbsp; For information about the access level needed to edit users, see the section [Grant access to edit users](grant-access-other-users.md#access-to-edit)&nbsp;in the article [Grant access to users](grant-access-other-users.md).


When you configure notification settings in bulk, your changes affect only the notifications you select for the users you select. All other notifications are left intact, even if they vary from user to user. 


To modify the email notification settings of multiple users in bulk:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Users**.

1. Select the users, then click **Edit**.
1. In the** Edit Person** box that appears, click **Notifications**.

1.  Click a category to view notification settings related to that category  



   If there is at least one user selected where the notifications do not match the notifications of the other selected users, the category check box for that notification appears as a straight line.  


1.  Click any notifications that you want the users to receive either daily or instantly, or clear any that you want them to stop receiving.   



   For the **Communication** category, you can select individual notifications for instant delivery only. You must select all of the notifications to be delivered in a daily digest. 


   When you modify a notification setting, the label **Edited** appears for that notification setting, to let you know that that notification setting has been modified.&nbsp;

1.   If you selected notifications to be sent as a daily digest, select the time of the day you want the digest delivered at the top of the **Notifications** section in the **Email Daily Digest after**&nbsp;menu.&nbsp;


   After you select a delivery time, the **Email Daily Digest ****after** box displays with an orange frame to indicate that the time of the delivery has been edited.


   The daily digest includes events that meet the criteria of the notifications 24 hours prior to the selected time. Users receive one daily digest email for each notification type.&nbsp;For more information about the notification types, see [Event Notifications Descriptions and Default Statuses](#event-notification-descriptions-and-default-statuses) below.&nbsp;


   The daily digest may arrive after the time you select, depending on how many emails are queued for delivery in the system. The time listed is your local time as specified in your browser settings.

1. Click **Save Changes.**




## Event&nbsp;Notifications Descriptions&nbsp;and Default&nbsp;Statuses {#event-notifications-descriptions-and-default-statuses}

When you enable event notifications at the system level, email notifications are enabled for all users in the system. Depending on which event you enable, users receive instant, daily, or both instant and daily email notifications for the specified event.&nbsp;Users can configure in their user profile what notifications they want to receive.&nbsp;For more information, see [Configure email notifications](configure-email-notifications.md).


For a list of all of the event notifications that a `Workfront administrator` can enable at the system level, see [System-level event notifications](system-level-event-notifications.md).
