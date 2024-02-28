---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Project enhancements
description: This page describes all changes Project enhancements made with the 2019.3 release. It was made available in the Production environment the week of August 19, 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
---
# 2019.3 Project enhancements

This page describes all changes Project enhancements made with the 2019.3 release. It was made available in the Production environment the week of August 19, 2019.

For a list of all changes made in 2019.3, see [2019.3 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Change the display type of a field in a custom form

Now you can change the display type of a field in a custom form.

For example, if you have created a Checkboxes field, you can change it to a Dropdown field or a Radio Buttons field. These three field display types are interchangeable.

Or, if you have created a Single Line Text Field, you can change it to a Paragraph Text field. These two field display types are interchangeable.

Previously, to change the display type of a custom field, you had to create a new field and delete the old one. This required transferring data, which was often time consuming.

For more information, see [Create or edit a custom form](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in the article [Create or edit a custom form](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

>[!NOTE]
>
>Preview availability:&nbsp;August 9, 2019
>
>Production availability:&nbsp;August 30, 2019

## Create time off calendars and reports

You can now see user's time off for better planning and execution. You can also add new time off reports and calendars to your dashboards for a real-time view of user availability.

>[!NOTE]
>
>Preview availability:&nbsp;August 9, 2019
>
>Production availability:&nbsp;August 30, 2019

## The Open filter now shows more results in a list of Issues

When you apply the Open filter to a list of issues, the list includes issues that:

* Are in a Closed - Pending Approval status
* Are associated with a resolving object

Prior to this change, these issues were not included in the list when applying the Open filter.

## New experience when inline editing information in lists

When you inline edit information in the new lists, the rows that have been edited will be dimmed, but the information will remain visible. Prior to this change, the edited rows were grayed out and the information was not visible.

You can find the new lists in the following areas of Workfront:

* Project and Tasks lists
* Hours tab for Projects, Tasks, and Issues

## Updated Lists for Project, Task, and Issues Hours Tabs

The improved list views are now available in the Hours tabs for projects, tasks, and issues.

Prior to this enhancement, the new lists were applied only to the following:

* A list of tasks
* A list of projects

For information about viewing items in a list, see [Get started with lists in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Edit Gantt without Enabling a Special Editing Mode

You can now edit the task list Gantt chart when the Autosave is enabled or not. You cannot undo changes when the toggle is on. In this case, the changes you make to the project are saved automatically.

For information about editing the task list Gantt chart, see [Update information in the task list Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Removing the Issues tab from the Kanban board

We are removing the Issues tab from the Kanban board in the 19.3 Production release. You can still access the Issues subtab from the Backlog on the Kanban board.

## Removing the Documents and Issues tabs from the iteration details page

>[!NOTE]
>
>This change will occur in Production with the 2019.3 release. It will not be made in the Preview environment prior to the Production release.

We are removing the Documents and Issues tabs from the Agile iteration details page:

* **Documents:** All documents stored in the Documents tab must be moved before the production release. If you fail to move your documents, you will no longer have access to them.
* **Issues:** This tab is generally located under the More drop-down menu. You can still access the Issues subtab from the Work Items tab on the iteration.

## Consider or ignore user time off in task dates

You can now decide whether to allow the time off schedule of the Primary Assignee of a task to adjust the planned dates.

You can make this decision either at the system level, as a Workfront administrator, or at the project level, as a project manager.

Prior to this change, the time off of the Primary Assignee always adjusted the planned dates of the task, if the Task Constraint allows for the dates to be modified.

For information about the system-level User Time Off setting, see [Configure system-wide project preferences](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

For information about the project-level User Time Off setting, see [Edit projects](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Preview availability:&nbsp;July 22, 2019
>
>Production availability:&nbsp;August 9, 2019

## Custom Conditions

Now you can do the following to customize the Conditions you use for projects, tasks, and issues and better meet the needs of your organization:

* Create custom Conditions with your own labels and colors.
* Change the order of Conditions in the drop-down lists where users select them.
* Use custom Conditions that you create in place of the built-in default Conditions that Workfront assigns automatically to work items.
* Change the names and colors of the built-in default Conditions for projects, tasks, and issues.

Also, if you have rights to edit a task or issue but you are not assigned to it (perhaps because you are overseeing it), you can now change its Condition using the Conditions column in a list view.

Previously, Conditions could not be customized or changed, and only users could change the Condition of a task or issue if they were assigned to it.

For more information, see [Custom conditions](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Preview availability:&nbsp;July 4, 2019
>
>Production availability:&nbsp;Late September or early October

## New email notification for Teams

There is a new email event notification for teams. Team members receive an email notification when a project with tasks assigned to their team becomes active. This setting is turned off by default.

Previously, team members could not notified when projects they were on became active.

For more information, see Notifications: Information about projects I'm on.

>[!NOTE]
>
>Preview availability:&nbsp;July 4, 2019
>
>Production availability:&nbsp;July 18, 2019

## Document Updates Now Appear on the Associated Object and Project

When you comment on a document, your update now appears on the Updates tab both for the document and for the object where the document is attached.

If the object is part of a project, your comment on the document also appears on the Updates tab for the project.

Previously, update comments appeared only on the Updates tab for the document.

For more information, see the section [Update work](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) in the article [Update work](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Preview availability:&nbsp;June 6, 2019
>
>Production availability:&nbsp;June 20, 2019

## Visibility into the Time-off Schedule of a User When Assigning Them to Tasks and Issues

When you assign a user to a task or an issue, you can now see an in-line warning if the user selected has time off scheduled any time between the planned dates of the task or issue.

For information about assigning tasks, see [Assign tasks](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

For information about time off, see [Configure personal time off](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Preview availability:&nbsp;May 30, 2019
>
>Production availability:&nbsp;June 13, 2019

## Add Fields That Represent Objects in Custom Forms

We have created a new field type in the custom form builder called Typeahead. This field allows you to add fields that represent objects to your custom forms. Currently, the User object is enabled with Typeahead, and other objects are coming in the future.

Previously, administrators had to manually maintain users as individual options in custom form drop-down menus.

For more information, see [Create or edit a custom form](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>Preview availability:&nbsp;May 30, 2019 
>
>Production availability:&nbsp;June 13, 2019 
>
>Prior to the Production release date, the new custom fields are not supported on Mobile, Outlook, MS Teams, and the native Salesforce integration. 
>
>In Production, Outlook and MS&nbsp;Teams are now supported. Mobile has been supported as of late June or early July; Salesforce integrations has been supported as of June.

## New Request "Subject" Field Has Been Renamed to "Name"

>[!NOTE]
>
>This feature was removed and will not be included in the 2019.3 release.

Now, when you submit a new request to a Request Queue, you enter the name of the request in the "Name" field of the new request form.

Prior to this change, you would enter the name of the request in the "Subject" field.

For information about creating requests, see [Create and submit Workfront requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

