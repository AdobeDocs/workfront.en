---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 1 release activity
description: This page describes all changes most recently available in the Preview environment with the 2018.1 Beta 1 release. The functionality on this page was made available in the Preview environment on December 1, 2017. It will be made available in the Production environment in March 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
---
# 2018.1 Beta 1 release activity

This page describes all changes most recently available in the Preview environment with the 2018.1 Beta 1 release. The functionality on this page was made available in the Preview environment on December 1, 2017. It will be made available in&nbsp;the Production environment in March 2018.

>[!IMPORTANT]
>
>&nbsp;Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2018.1, see&nbsp; [2018.1 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

The 2018.1 Beta 1 release contains enhancements for both for Workfront administrators and other users:

**For Administrators**

* [Updated Layout Template to Support the Home Area](#updated-layout-template-to-support-the-home-area) 
* [Disable Proofing Email Notifications Sent from Workfront](#disable-proofing-email-notifications-sent-from-workfront) 
* [New Resources Added to Event Subscriptions](#new-resources-added-to-event-subscriptions)

**For All Users**

* [Home Area (Updated My Work Area)](#home-area-updated-my-work-area) 
* [Display Resource Planner Data under the Business Case and Updated Business Case Summary](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary) 
* [Display the Percentage of Planned Hour Allocation in the Resource Planner](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner) 
* [The "Automatic and On Change" and "Change Only" Update Types Trigger Updates to the Parent Objects at the Same Time as Tasks Are Updated](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated) 
* [Timeline Snapshot Available in the Gantt Chart](#timeline-snapshot-available-in-the-gantt-chart)

## Home Area (Updated My Work Area) {#home-area-updated-my-work-area}

The new Home area provides an alternate, enhanced view to the same data that is currently available in the My Work area. The Home area provides the following benefits over the My Work area:

* A more streamlined and intuitive interface
* Enhanced performance
* Update tasks and issues with rich text formatting

## Updated Layout Template to Support the Home Area {#updated-layout-template-to-support-the-home-area}

As a Workfront administrator, you can determine whether users in your organization have access to the Home area by configuring the layout template they are assigned to. Users who are not assigned a layout template can always access the Home area.

For more information, see "Create and manage Layout Templates."

## Disable Proofing Email Notifications Sent from Workfront {#disable-proofing-email-notifications-sent-from-workfront}

You can now configure whether users in your Workfront instance receive email notifications from Workfront when a comment is made on a proof.

Previously, proofing emails were always sent from Workfront when a comment was made on a proof. If notifications were also enabled in Workfront Proof, this resulted in users receiving duplicate notifications.&nbsp;

For existing Workfront customers, Workfront is configured by default to send emails when a comment is made on a proof.

For information about how to disable email notifications for proofs in Workfront so that proofing emails are sent only from Workfront Proof, see&nbsp;.&nbsp;&nbsp;

## Display Resource Planner Data under the Business Case and Updated Business Case Summary {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

The Resource Budgeting area is now available in the Business Case of a project. In this area, you can review the Budgeted Hours estimated for your resources in the Resource Planner and the Budgeted Labor Cost associated with them.

The Resource Estimates area of the Business Case has been renamed to Legacy Resource Estimates.

As part of this change, the Business Case Summary now includes financial information based on both Resource Estimates and Resource Budgeting.

Prior to this change, you could not see Resource Planner information on the Business Case of the project. You could only see Resource Estimates information which is specified in the Capacity Planner of the Legacy Resource Pools.

For more information about creating a Business Case, see [Create a Business Case for a project](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Display the Percentage of Planned Hour Allocation in the Resource Planner {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

The User View of the Resource Planner now includes a new column that enables you to view the Planned Hour Allocation as a percentage of the total Available Hours for the user and the job role.

Prior to this change, you could view the total of Planned and Available Hours for users and job roles only in separate columns.

For more information about the Planned Hours Allocation Percentage column, see the “Viewing the Difference between Available and Planned Hours or FTE in the Resource Planner” section in [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## The "Automatic and On Change" and "Change Only" Update Types Trigger Updates to the Parent Objects at the Same Time as Tasks Are Updated {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

We have changed the way parent tasks and the project update when a lower-level object is updated in a project. The time when a parent object updates is determined by the Update Type field on a project. You can select from the following Update Types:

* Automatic and On Change
* Change Only
* Automatic Only
* Manual Only

Now, when you select the "Automatic and On Change" or "Change Only" Update Types, the changes you apply to the individual tasks are also applied to the parent task and the project immediately.

Prior to this change, you had to refresh the page to ensure that the parent objects and the timeline of the project also updated.

For more information about the Update Type of a project, see [Select the project Update Type](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Timeline Snapshot Available in the Gantt Chart {#timeline-snapshot-available-in-the-gantt-chart}

You can now quickly scroll to a certain point in the lifetime of a project by using the new timeline snapshot in the Gantt chart.

When you select a more granular time frame for the Gantt chart while viewing a task or a project list, a horizontal scroll bar is shown at the bottom of the Gantt chart. Clicking the scroll bar allows you to see the entire timeline of the project in a snapshot. You may click anywhere inside the Gantt chart snapshot to navigate to a specific point in the lifetime of the project.

Prior to this change, you had to scroll horizontally on the entire Gantt chart to find a certain point in time, or you had to zoom out of the granular view.

For more information about how information displays in the Gantt chart, see [Configure how information displays on the Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## New Resources Added to Event Subscriptions {#new-resources-added-to-event-subscriptions}

Now you can create event subscriptions for the following resources:

* **Expense:** Notifies you when an expense is added or modified.
* **Assignment:** Notifies you when an assignment is added or modified on a task or issue for a user, job role, or team.
* **Timesheet:** Notifies you when a timesheet is submitted, rejected, or approved.

To learn more about event subscriptions, see [Event Subscription API](../../../../wf-api/general/event-subs-api.md).
