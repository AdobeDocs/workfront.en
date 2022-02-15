---
filename: auto-reminders-vs-reminder-notifications
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Automatic reminders vs. reminder notifications {#automatic-reminders-vs-reminder-notifications}


This article describes the differences between automatic reminders and reminder notifications and provides scenarios for each. For more information on all `Workfront` notifications, see [Workfront notifications](workfront-notifications.md).


## Automatic reminders {#automatic-reminders}

The following characteristics are specific to automatic reminders:



* Can only be turned on and edited by a `Workfront administrator`
* Are triggered on all tasks and issues when they are&nbsp;due, late ,or near the planned completion date
* Can only be sent to the assignee, assignee's manager, or the&nbsp;manager of the immediate manager.
* Cannot not have an email template attached to them.


Scenario:&nbsp;If you want reminders to be triggered on all tasks and issues throughout the system, then configure the automatic reminder settings. For more information, see [Set up automatic reminders](setting-up-automatic-reminders.md).


## Reminder notifications {#reminder-notifications}

The following characteristics are specific to reminder notifications:



* Can be created by an admin or any users with a Plan license and administrative access to Reminder Notifications
* Can only be associated manually to an object
* Can only notify regarding the attached object
* Can be sent to various object stakeholders, such as owner, creator, approver, or assignee
* Can either use the default email or use a customized email template that is attached


Scenario: If you want to build reminders for projects, timesheets, or want to customize reminders for tasks and issues, then configure reminder notifications. For more information, see [Set up reminder notifications](set-up-reminder-notifications.md).
