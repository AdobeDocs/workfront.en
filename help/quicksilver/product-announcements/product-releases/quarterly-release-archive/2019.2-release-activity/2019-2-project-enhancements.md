---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2 Project enhancements
description: This page describes all Project enhancements included with the 2019.2 release. The functionality is planned to be available in the Production environment the week of May 20, 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
---
# 2019.2 Project enhancements

This page describes all Project enhancements included with the 2019.2 release. The functionality is planned to be available in the Production environment the week of May 20, 2019.

For a list of all changes made in 2019.2, see [2019.2 Release Activity Overview](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Find Groups Faster When Customizing Statuses

The drop-down menu on the Statuses tab in the Setup area is now a typeahead menu. This allows you to quickly search and find any group in the system, making it easier to customize statuses.

Previously, the drop-down menu displayed a limited number of groups. If the group you wanted did not display, you had to navigate to Setup > Groups and find the specific group in order to customize the group's statuses.

For more information, see [Create or edit a status](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Attach Default Custom Forms and Approval Processes to Tasks

You can now configure default custom forms and approval processes to attach to tasks when you add tasks to a project. You can configure the default settings at the project level.

For information about configuring default custom forms and approval processes for tasks at the project level, see the "Tasks" section in the [Edit projects](../../../../manage-work/projects/manage-projects/edit-projects.md) article.

## Display the Entire Row of a Parent Task in Bold in a Task List

In a task list, the row that contains a parent task is displayed in bold. This change is visible when the list is sorted by the Work Breakdown structure or by the Task Number in ascending order.

## Reverse Changes on the Task Lists

A&nbsp;new Autosave button on the task list enables you to select whether you want the changes you make to be automatically saved, or whether you want to see the effects your changes make before saving them. This setting applies both to the task list and the Gantt chart.

Prior to this enhancement, all changes were always saved automatically.

For information about editing tasks in a task list, see [Edit tasks](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

For information about editing tasks in the Gantt chart, see [Update information in the task list Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## New Column Width Defaults in New Lists

Now, Workfront automatically adjusts the width of the columns according to the valueformat information in each column. For example, columns that display a number are wider than those that display the Description field.

Prior to this improvement, column widths in the new project and task views were set to 100 pixels, unless otherwise specified.

For information about column widths, see [Modify column width and order](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Deactivate Unused Objects

>[!NOTE]
>
>This feature was released directly to the Production environment during the 2019.2 Preview timeframe.

If you have objects that are no longer used, you can now deactivate them to hide them from lists in order to prevent users from associating them with other objects.

Now, when you edit any of the objects below, you can indicate whether they should be active. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects. Objects not set to Active are not visible in drop-down menus and type-ahead fields to attach to other objects.

* Approval Processes
* Companies
* Custom Forms
* Milestone Paths
* Portfolios
* Programs
* Templates

Anything you deactivate that is currently used continues to function as it always has, and is not removed or blocked.

>[!IMPORTANT]
>
>When creating these objects via the Workfront API, the default value for the "isActive" parameter is true. This is a new field for all objects and is not available for you to edit prior to version 11 of the API. This field did previously exist for Portfolio's, except that the default value was false; it will change to a default value of true starting with version 11 of the API.

## Display Budgeted Cost of Work Scheduled (BCWS) and Performed (BCWP) in Views

You can now display the Budgeted Cost of Work Scheduled (BCWS) and the Budgeted Cost of Work Performed (BCWP) in project and task views.

Although these project performance metrics were used in financial calculations in Workfront before, they were not visible in the system prior to this enhancement.

For information about calculating BCWS, see [Calculate Budgeted Cost of Work Scheduled (BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

For information about calculating BCWP, see [Calculate Budgeted Cost of Work Performed (BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

