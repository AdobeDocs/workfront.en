---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Automatic Reminders vs. Reminder Notifications
description: This article describes the differences between automatic reminders and reminder notifications and provides scenarios for each.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
TQID: https://experienceleague.adobe.com/hSVm-rgiBcbHaCwO1veCLEo-q6U5SWzt58qO6KqC84M
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Automatic reminders vs. reminder notifications

This article describes the differences between automatic reminders and reminder notifications and provides scenarios for each. For more information on all [!DNL Adobe Workfront] notifications, see [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

## Automatic reminders

The following characteristics are specific to automatic reminders:

* Can only be turned on and edited by a [!DNL Workfront] administrator
* Are triggered on all tasks and issues when they are due, late, or near the planned completion date
* Can only be sent to the assignee, assignee's manager, or the manager of the immediate manager.
* Cannot not have an email template attached to them.

Scenario: If you want reminders to be triggered on all tasks and issues throughout the system, then configure the automatic reminder settings. For more information, see [Set up automatic reminders](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## Reminder notifications

The following characteristics are specific to reminder notifications:

* Can be created by an administrator or any users with a Standard of Plan license and administrative access to Reminder Notifications
* Can only be associated manually to an object
* Can only notify regarding the attached object
* Can be sent to various object stakeholders, such as owner, creator, approver, or assignee
* Can either use the default email or use a customized email template that is attached

Scenario: If you want to build reminders for projects, timesheets, or want to customize reminders for tasks and issues, then configure reminder notifications. For more information, see [Set up reminder notifications](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
