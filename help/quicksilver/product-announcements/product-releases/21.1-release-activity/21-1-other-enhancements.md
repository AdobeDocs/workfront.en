---
content-type: release-notes
keywords: notes,quarterly,update
navigation-topic: product-releases
title: 21.1 Other enhancements
description: This page describes all other enhancements made with the 21.1 release to the Preview environment. These enhancements will be made available in the Production environment the week of February 15, 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
---
# 21.1 Other enhancements

This page describes all other enhancements made with the 21.1 release to the Preview environment. These enhancements will be made available in the Production environment the week of February 15, 2021.

For a list of all changes available with the 21.1 release, see [21.1 release overview](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Updates to Event Subscription failure requirements

We are updating the soft-disable requirements of Event Subscription failures. In addition to the existing requirements, Event Subscriptions will now be soft disabled if they fail to achieve a successful delivery within 2000 attempts. This is to strengthen the existing 70% failure rule which can lead to excessive amounts of failures, under some conditions.

Additionally, we'll be adding in hard-disable requirements as of February 2021.

For additional information about the new soft-disable and hard-disable requirements, see [FAQs - Event Subscriptions](../../../wf-api/general/event-subs-faq.md).

## New Team fields available to the Daily Digest

We've added Team approval and assignments fields to the Action Needed Daily Digest email.

For more information, see [Notifications: Action needed](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Replacing POP email option in Request Queues

We're replacing the POP email option for request queues with a new Workfront-managed system. You will still be able to submit requests via email, but you'll need to set up a new Adobe Workfront-managed email address in the Request Queue area instead.

These changes are available to test in Preview.

Email is automatically disabled in all Preview environments. To enable email for testing purposes, see [Enable delivery of emails from the Preview Sandbox environment](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

For more information, see [Enable users to email an issue into a Request Queue project](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

For more information about why we are making this change, see [New Adobe Workfront managed system to replace POP email for Request Queues with 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

This feature is now included in the [Queue Management in the new Workfront experience](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) learning path on Workfront One.

## Restrict hour editing on timesheets

To provide more control over timesheets and hour editing, we've added a setting that allows you to restrict hour editing to timesheet owners and system administrators.

Previously, users with the Timesheets & Hours option enabled in their access level could edit hours on any timesheet.

For more information, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Improved filters and views in the Timesheets area

We've added the following improvements when you add a Project, Task, or Issue to a Timesheet:

* Filters: We've added filters for Projects and Issues. Click More options to view these filters. Previously, only Tasks had filtering available.
* Views: We've added View and Grouping options to the Search page.

For more information, see [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Hide the overtime box in Timesheets

You can now hide the overtime box to ease user confusion if you do not track overtime in Workfront. You can hide the overtime box for a single-use timesheet or in the Timesheet Profile:

* Single-use Timesheet: When you opt to hide the overtime box in an individual timesheet, it is hidden only for that timesheet. For more information, see [Create a single-use timesheet](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Timesheet profile: When you opt to hide the overtime box in the Timesheet Profile, all future timesheets created for the user(s) assigned to that profile will not see the overtime box. For more information, see [Create, edit, and assign timesheet profiles](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Previously, you could not hide the overtime box on timesheets.

## Expand or collapse items in the breadcrumb navigation

To allow easier viewing of the full breadcrumb path, we've added expand and collapse functionality.

Now, any truncated items are grouped before the Project with the text "more". For example, "3 more" indicates that there are 3 objects that aren't displaying.

Previously, you had to click the ellipsis to display any truncated objects in a drop-down menu.

To view all items in the breadcrumb, click "more" at the beginning of the breadcrumb to expand the items. Once expanded, you can click "Less" to collapse the items again.

## New look and feel to breadcrumb navigation

To help users to better identify where they are in Workfront and more easily navigate between objects, we've made the following improvements to breadcrumb navigation:

* Each item in the breadcrumb now includes an object label.
* The current page is now included in the breadcrumb and is in italics.
* Keyboard navigation and screen reader navigation are now available for the breadcrumbs.
* Additional minor styling changes

