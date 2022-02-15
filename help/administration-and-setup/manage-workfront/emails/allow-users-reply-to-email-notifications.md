---
filename: allow-users-reply-to-email-notifications
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
---




# Allow users to reply to email notifications {#allow-users-to-reply-to-email-notifications}

You can configure `Workfront` to allow users to make a comment on a `Workfront` object by replying to an email notification.


## Email replies {#email-replies}

When a user makes a comment on an object in `Workfront`, an email notification containing the comment is delivered to users who have set up email notifications and who are tagged on the object. To learn about email notifications, see [Enable and disable event notifications](enable-and-disable-event-notification.md) and [Configure email notifications](configure-email-notifications.md).


You can configure `Workfront` to allow users to make a comment on a `Workfront` object by replying to an email notification. Using either the `Workfront` default email service or a POP email account, recipients of email notifications can make comments on `Workfront` objects without logging in to `Workfront`.


>[!NOTE]
>
>Although POP users can reply to emails sent from `Workfront`, we strongly encourage the use of the default mail service.


For information about configuring a POP email account, see [Use a POP email account to comment on work items](using-pop-email-reply.md).


For information about using the default email service, see [Comment on work items using Workfront default email service](comment-work-items-wf-default-email-service.md).


## Objects supporting email notifications {#objects-supporting-email-notifications}

You can respond to `Workfront` email that is generated from comments made to the following objects:



* Project
* Task
* Issue
* Document
* Template and template task
* Portfolio
* Program
* Iteration
* Timesheet


To learn more about making comments, see [Update work](update-work.md).


>[!NOTE]
>
>Plus addressing (such as yourname+organization@organization.com) is not supported for users commenting on `Workfront` objects via email.


