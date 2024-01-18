---
content-type: release-notes
keywords: notes,quarterly,update,release
navigation-topic: 2021-2-release-activity
title: 21. 2 Reporting enhancements
description: This page describes all Reporting enhancements made with the 21.2 release to the Preview environment. These enhancements will be made available in the Production environment the week of May 10, 2021. For a list of all changes available with the 21.2 release, see 21.2 Release overview.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
---
# 21. 2 Reporting enhancements

This page describes all Reporting enhancements made with the 21.2 release to the Preview environment. These enhancements will be made available in the Production environment the week of May 10, 2021. For a list of all changes available with the 21.2 release, see [21.2 Release overview](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Restrict hour editing in projects and reports

To provide more control over hour editing on the Hours tab in a project and Hour reports, we've added a setting that allows Workfront administrators to restrict hour editing to hour owners and system administrators.

Previously, users with Timesheets & hours enabled in their access level could edit hours.

For more information, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## New look and feel for the Assignments field in updated lists and reports

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

To match the modern look of other areas in the new Workfront experience, the styling has changed for the Assignments field in updated lists and reports. This redesign includes:

* A rounded avatar for the user profile pictures, job roles, and teams
* Initials display for users without profile pictures
* A new Job role icon
* A new People icon for advanced assignments
* A new Restricted Access icon
* Other minor design changes

For more information on assignments in lists, see [Assign tasks](../../../manage-work/tasks/assign-tasks/assign-tasks.md) or [Assign issues](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## New look and feel for typeahead fields in updated lists and reports

>[!NOTE]
>
>Temporarily removed from the Production environment on May 20, 2021.

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

To match the modern look of other areas in the new Workfront experience, the styling has changed for typeahead fields in updated lists and reports. These changes include:

* The Typeahead icon has been removed from the field.
* When you click a typeahead field, the suggestions menu now displays before you enter text. 
* The suggestions menu is more responsive to the length of values and these values are now truncated at the end when the character limit is met instead of in the middle of the value.

For information on updated lists, see the [The difference between the updated and the legacy lists](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) section in the article [Get started with lists in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Report on system updates

The new Journal Entry report gives you greater auditability by allowing you to drill in to system updates, including:

* Status changes on a project, task, or issue
* Deleted tasks or issues
* Values in custom fields
* Planned Completion Dates
* Project owner changes

For example, you can set up this report to show activity around a specific custom field, including the project for the custom field, when a value was first entered, what that value was, when the field was updated, what the previous value was, what the newly entered value was, which users completed these actions, etc.

Previously, you could report on system updates only via the Workfront API.

To learn more about this report and what you can use it for, see [Report on the Updates area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

