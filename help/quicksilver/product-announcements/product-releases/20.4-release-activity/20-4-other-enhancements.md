---
title: 20.4 Other enhancements
description: 20.4 Other enhancements
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
---
# 20.4 Other enhancements

This page describes all other enhancements made with the 20.4 release to the Preview environment. These enhancements will be made available in the Production environment the week of November 9, 2020.

For a list of all changes available with the 20.4 release, see [20.4 release overview](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## New for administrators:&nbsp;Switch Workfront environment option available

For a more efficient and convenient experience, Group administrators and Workfront administrators can now quickly switch between different Workfront environments from any page in Workfront without having to log out.

In the new Workfront experience, the option Switch to Classic appears in the Main Menu.

In Workfront Classic, the option Switch to the new experience appears in the menu that displays when clicking the profile picture in the top-right corner of the Global Navigation Bar.

This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One.

## Improved encryption for Workfront Proof

We are making some changes to improve the strength of data-in-motion encryption of the Workfront Proofing Application. The weak TLS ciphers will be deprecated on November 11, 2020.

Please ensure you are using a supported browser when accessing Workfront. For more information about supported browsers, see [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).

## New look and feel for 3 email templates

To improve the readability and overall experience, the following email templates have a new look and feel:

* New Work Request
* A Dependent Task You're Assigned to Is Now Ready to Start
* Team Email Notification with Predecessor Complete

To enable email for testing purposes in your Preview environment, see the Managing emails in preview section in [Modify your own email notifications](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## New email notifications for teams

We've added the following email notification for teams:

* A predecessor of a task assigned to my team is completed: The team assigned receives an email notification when a predecessor of one of their tasks is marked complete.
* All predecessors of a task assigned to my team are completed: The team assigned receives an email notification for each predecessor that is marked complete.

For more information, see [Notifications: Information about work assigned to me](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## New for administrators: Email notification enhancements

Now, with a single click, you can enable or disable an event email notification in Setup. Just click the On/Off switch next to the name of the notification.

Also, notice our modern styling now improving the experience of configuring event notifications in the Email Notifications area.

For information about configuring email notifications, see [Configure event notifications for everyone in the system](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

This feature is now included in the [Email and in-app notifications learning path](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) on Workfront One.

## New API&nbsp;objects that trigger event subscription updates

Two new API objects, documentVersion and proofApproval, were created and are configured to trigger event subscription updates when a document is versioned or approved.

For a full list of fields that are associated with each object, please see [Event subscription resource fields](../../../wf-api/api/event-sub-resource-fields.md).
