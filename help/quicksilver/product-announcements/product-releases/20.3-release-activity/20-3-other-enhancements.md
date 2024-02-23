---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 other enhancements
description: This page describes all other enhancements made with the 20.3 release to the Production environment. These enhancements were made available in the Production environment the week of August 10, 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
---
# 20.3 other enhancements

This page describes all other enhancements made with the 20.3 release to the Production environment. These enhancements were made available in the Production environment the week of August 10, 2020.

For a list of all changes available with the 20.3 release, see [20.3 release overview](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Share a calendar with a private link

To ease the burden of sharing calendars in Workfront, you can share a private link that takes users directly to the calendar. The calendar must be shared with the user, and they have to log in to view it.

Previously, you could share a public URL that did not require a log in to view.

For more information, see [Share a calendar report](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## New Drafts area when creating requests

To give you more flexibility when working with requests, Workfront now automatically saves every request you create as a draft in the new Drafts area. If you don't have all the information needed to complete the new request, you can leave it as a draft, come back to it and finish it later. Workfront saves one request per queue topic in the new Drafts area. The draft requests can be saved for as long as you need them until you are ready to complete and submit them. You can also remove or reposition the Drafts area in the left panel using a Layout Template.

For more information about creating requests, see [Create and submit Workfront requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>For the Preview release, if you have a custom Layout Template assigned to you, you will need to add the Drafts area of your Requests by modifying your Layout Template.

## Expand or collapse items on the timesheet

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience

To help you easily manage timesheets with several items, you can now expand or collapse all items with the click of a button.

Previously, you had to click on each item individually.

For more information, see [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignore Actual Dates in Workfront Calendars

>[!NOTE]
>
>This feature released to the Preview environment on June 5, 2020. It will be available in the Production environment on June 19, 2020.

To give you more control over how objects display in Calendar Reports, you can opt to ignore actual dates even when they're available.

Previously, the calendar would automatically use Actual dates once they were available.

For more information, see [Calendar reports overview](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Use custom date fields in calendar reports

>[!NOTE]
>
>This feature released to the Preview environment on May 29, 2020. It will be available in the Production environment on June 12, 2020.

To help you better visualize and manage your daily work with calendars, custom date fields are now available as a date option.

Previously, you could manage your calendar only with projected, planned when actual dates were not available.

For more information, see [Use custom date fields in a calendar report](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (or if you are using Workfront Classic, see [Use custom date fields in a calendar report](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US)).

## Email changes

**Outbound email changes:** All email from Workfront will come from notifications@my.workfront.com. This includes automated alerts and user to user communication.

Previously, System administrators could add an custom email address in the Email Setup area.

**Inbound email POP reply changes:** System Administrators will no longer have the ability to configure a custom POP email server for incoming email replies to notifications.

For more information, see [Email spoofing and POP reply email changes](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## DomainKeys Identified Mail (DKIM) now included on outgoing Workfront emails

An email authentication technique (DKIM) will be included on all outgoing emails. This DKIM signature is not visible to the end-user but allows validation on a server level and reinforces our existing authentication framework.

## Updates to enrollment in the new Workfront experience

To make user enrollment in the new Workfront experience more manageable, Group Administrators now have access to enroll and unenroll users that belong to the groups they manage.

There is also now a User details link that displays the following user information:

* Name
* Job role
* Email address
* Profile picture

## New for administrators: Brand Workfront for specific groups, teams, job roles, and users

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience

Now you can use a Layout Template to change the logos in the top navigation area and on the Main Menu for specific groups, teams, job roles, and users who have their own branding.

For more information, see [Brand your Adobe Workfront instance](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Group Administrators can create and manage approval processes

To allow more autonomy and control of their groups' workflows, a Group Administrator can now access the Approval Process area in Setup and create and edit approval processes for a group that he or she manages. These approval processes are based on that group's statuses.

To assure that Group Administrators don't inadvertently edit approval processes that are used throughout the system or are created by other groups, they can access only the approval processes associated with the groups they manage.

For more information, see [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## For administrators: New Groups page makes it easier to create and manage groups

Group administrators can more easily manage groups now that everything they need is on the new Groups page. It's no longer necessary to navigate between various overlay boxes and Setup pages to create and modify groups.

Here are the main highlights:

* Group Details: View and edit basic information about the group, such as the group's name, description, Group Administrators' names, and whether the group is public or private.
* Group members list: View all group members and use the new toolbar to quickly add, remove, export, activate, and deactivate memberships. You can also edit members' profiles and send them Update comments.
* Group Administrator field in the header: When you are viewing a group you manage, quickly assign or unassign a group member as an administrator of the group. You can also do this in the list of group members using the new Group Role column.
* Subgroups list: View, edit, copy, export, and delete the subgroups in a group that you manage.
* Statuses list: View and manage your group's statuses.

For more information, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## New for administrators: Create up to 14 levels of subgroups

To make it easier to organize your Workfront groups to match your organization hierarchy, we've increased the levels of subgroups you can create within a group from 3 to 14.

For more information, see [Groups overview](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## New for administrators: New Setup sidebar

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience

The left sidebar in Setup is now faster and easier to use and leverages the basic layout and functionality you already know. Along with a more modern look and feel, here's what else is new:

* A new off-white background in the sidebar makes it easier to differentiate from the rest of the Setup area.
* Icons in the sidebar are a bit larger and some are redesigned to suggest more clearly what the option does.
* More vertical space between sidebar items makes them easier to read.
* You can collapse the sidebar when you need room in the main area to see and do more, such as viewing additional columns. And you can expand the sidebar again when you need to see feature names.
* While the sidebar is collapsed, you see only the icons for each feature. To see the sub-items under a main sidebar item, hover over its icon to display them in a flyout menu. For example, hover over the Processes icon to display a menu containing Approvals and Milestone Paths.
* You can access the two Kick-Starts options (Import Data and Export Data) one click faster. They have moved out from under System to display on the main level of the sidebar.

For information about how to use the Setup area, see [Administration and setup](../../../administration-and-setup/administration-and-setup.md).

## Include cluster number in Customer Info area

As a Workfront administrator, you can now easily find the cluster number inside Workfront, without having to spend additional time and effort getting it from our Support team. We added a Cluster Setup field in the Customer Info area of Setup.

For information about the Customer Info area, see [Configure basic information for your system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Base64 encoding for Event Subscriptions

The base64Encoding field is an optional field that is used to enable Base64 encoding of event subscription payloads. If a request is made using the base64Encoding field set to true, then the newState and oldState objects in the payload are delivered as Base64 encoding strings. This feature can be useful if your network is configured in such a way that it will not allow special characters in Event Subscriptions.

For more information please see [Event Subscription API](../../../wf-api/general/event-subs-api.md).

## Removed ability to create duplicate Event Subscriptions

To prevent the delivery of duplicate messages, you can no longer create duplicate subscriptions. Additionally, any duplicate subscriptions created previously have been removed.

For more information, see [FAQs - Event Subscriptions](../../../wf-api/general/event-subs-faq.md).
