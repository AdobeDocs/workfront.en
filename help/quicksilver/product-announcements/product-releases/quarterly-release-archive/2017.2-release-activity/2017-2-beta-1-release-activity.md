---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 1 release activity
description: This page describes all changes available in the Preview environment with the 2017.2 Beta 1 release. The functionality on this page was made available in the Preview environment on May 10, 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
---
# 2017.2 Beta 1 release activity

This page describes all changes available in the Preview environment with the 2017.2&nbsp;Beta 1 release. The functionality on this page was made available in the Preview environment on May 10, 2017.

>[!IMPORTANT]
>
>Functionality described on this page is subject to change prior to availability in the Production environment.

The 2017.2 Beta 1 release contains enhancements both for Workfront administrators and other users:

**For Administrators:**

* [Restore Documents](#restore-documents) 
* [New Preview Banner with Release Information](#new-preview-banner-with-release-information)&nbsp;
* [API 7 Availability](#api-7-availability)

**For All Users:**

* [Subscribe to Tasks and Issues](#subscribe-to-tasks-and-issues) 
* [Resource Scheduling Improvements](#resource-scheduling-improvements) 
* [Compare Proofs](#compare-proofs) 
* [New Field for Resource Pools for Users and Projects](#new-field-for-resource-pools-for-users-and-projects) 
* [Updated Look and Feel in the Dashboard List](#updated-look-and-feel-in-the-dashboard-list) 
* [Removing the Endorsements Functionality in Workfront](#removing-the-endorsements-functionality-in-workfront) 
* [Reorder Columns in Any List with Drag-and-Drop (Functionality Is Being Removed)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Restore Documents {#restore-documents}

Workfront administrators&nbsp;can now restore individual documents that were deleted within the past 30 days.&nbsp;

Prior to this change, Workfront administrators could restore only projects, tasks, and issues (including documents that were deleted in conjunction with the deleted project, task, or issue).

For more information, see [Restore deleted items](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## New Preview Banner with Release Information {#new-preview-banner-with-release-information}

The blue banner at the top of the Preview Sandbox environment now displays the release name and version number of the Preview environment. Clicking the name of the release will take you to a Help Site article where you can find more information about the current Preview release. For more information about the Preview Sandbox Environment, see [The Adobe Workfront Preview Sandbox Environment](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)&nbsp;

## API 7 Availability {#api-7-availability}

API 7 is now available and includes new and updated objects.

For more information, see [What's New in API Version 7](../../../../wf-api/api/new-api-version-7.md).

## Subscribe to Tasks&nbsp;and&nbsp;Issues {#subscribe-to-tasks-and-issues}

Workfront sends notifications about items you are assigned to or that you own.

Starting with the current release, if you want to follow items that are not assigned to you but might impact your work, you can subscribe to them.

You can subscribe to issues and tasks you have permissions to at least View. When a new comment is added to the issue or task that you subscribe to, you will be notified in an email about that comment.

For more information about subscribing to issues and tasks, see [Subscribe to items in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Resource Scheduling Improvements {#resource-scheduling-improvements}

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

The following improvements are available when scheduling resources:

* [View More Items on the Resource Scheduling Timeline in a Single View](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view) 
* [Configure the Project Name to Display on Tasks and Issues on the Scheduling Timeline](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline) 
* [Configure Whether Parent Tasks Are Displayed on the Scheduling Timeline](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline) 
* [More Easily Expand or Collapse All Tasks and Issues on the Scheduling Timeline](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline) 
* [Role and User Information Remains at the Top of the Scheduling Timeline When Scrolling](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### View More Items&nbsp;on the Resource Scheduling Timeline in a Single View {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

When scheduling resources for a team or for any projects for which you are the Resource Manager, tasks and issues now consume less vertical space on the scheduling timeline. This allows you to see more&nbsp;tasks and issues in a single view.

If you decide to show project names on each task and issue on the scheduling timeline, the vertical space of each task and issue is expanded,&nbsp;resulting in fewer tasks and issues displaying in a single view.

For more information about scheduling resources, see&nbsp; "Get started with Resource Scheduling".

### Configure the Project Name to Display on Tasks and Issues on the Scheduling Timeline {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

When scheduling resources for a team or for any projects for which you are the Resource Manager, you can now configure the project name to display on each task and issue on the scheduling timeline.&nbsp;This allows users viewing the scheduling timeline to quickly see the name of the project where the task or issue resides.

For more information, see "Get started with Resource Scheduling".

### Configure Whether Parent Tasks Are Displayed on the Scheduling Timeline {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

When scheduling resources for projects for which you are the Resource Manager, you can now configure whether&nbsp;parent tasks display&nbsp;on the scheduling timeline when the Summary Completion Mode option on the project is set to Manual.

Prior to this change, parent tasks always displayed on the scheduling timeline when the Summary Completion Mode on the project was set to Manual.&nbsp;

When the Summary Completion Mode on the project is set to Automatic, parent tasks cannot be displayed on the scheduling timeline. This experience has not changed.

For more information, see "Get started with Resource Scheduling".

### More Easily Expand or Collapse All Tasks and Issues on the Scheduling Timeline {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

A new link is available that allows you to more easily collapse all tasks and issues on the scheduling timeline.

For more information, see "Get started with Resource Scheduling".

### Role and User Information Remains at the Top of the Scheduling Timeline When Scrolling {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Now when scrolling down on the scheduling timeline to view additional information, the role name and user name remain at the top of the Users and Roles area on the scheduling timeline, making it easier to see which&nbsp;user and role the tasks and issues are associated with.

Prior to this change, the role name and user name would scroll out of the current view.

For more information about scheduling resources, see&nbsp; "Get started with Resource Scheduling".

## Compare Proofs {#compare-proofs}

You can now compare two document proofs&nbsp;within any single document list, such as within the Documents tab in a project, task, issue, portfolio, or within the main Documents area in the Global Navigation Bar.&nbsp;

The two proofs are displayed&nbsp;within the Review and Approval tool, and you can proof each document while comparing them in a&nbsp;side-by-side view.

For more information, see [Compare proofs](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## New Field for Resource Pools for Users and Projects {#new-field-for-resource-pools-for-users-and-projects}

The R1.5 release introduced&nbsp;new functionality around Resource Planning to the Preview environment. This&nbsp;functionality allows you to create new Resource Pools, which are collections of users.

Now you can associate these Resource Pools with projects, as well as with users. You will now see a new field called "Resource Pools" on the project, as well as on the user object.

For more information about the new Resource Pools and how they can be associated with projects and users, see [Resource pools overview](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Updated Look and Feel in the Dashboard List {#updated-look-and-feel-in-the-dashboard-list}

Now when viewing a dashboard list, the look and feel is more modern and scalable.

This functionality was previously available only for users enrolled in Early Access. This is now available for all users in the Preview environment. It&nbsp;will be made available to all users in the Production environment with the 2017.2 release.&nbsp;

For more information about dashboards, see [Create a dashboard](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Removing the Endorsements Functionality in Workfront {#removing-the-endorsements-functionality-in-workfront}

While evaluating the functionality contained in the update stream, we have identified Endorsements to be a low adoption and a low usage feature. In 2017.2, the following functionality around Endorsements will be removed&nbsp;from Workfront starting with the 2017.2 release (this functionality is no longer available in Preview):

* The Endorsements tab in the user profile area;
* The Endorsements object will be removed from the API explorer; if you are currently pulling API reports for the objects "Endorsement" or "Endorsement Share", the calls will be invalid after the removal of this object.

The following functionality will continue to stay in the web application:

* The endorsement of a user by another user which was made prior to the removal&nbsp;of this feature will remain in the update stream of the endorser.&nbsp;

Endorsements have not been a reportable object, therefore there are no changes around reporting for this object.

## Reorder Columns in Any List with Drag-and-Drop (Functionality Is Being Removed) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

The functionality for changing the order of columns in any list by dragging a column from one location and dropping it in another is being removed from Early Access in the Production environment with the 2017.2 release and will no longer be available to any users.&nbsp;

For more details about this functionality, see [Modify column width and order](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
