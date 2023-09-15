---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 5
description: This page describes all changes available in the Preview environment with the R1 Preview 5 release. The functionality on this page was made available in the Preview environment on March 16, 2017.
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
---
# R1 Preview 5

This page describes all changes available in the Preview environment with the R1 Preview 5 release. The functionality on this page was made available in the Preview environment on March 16, 2017.

For a list of all changes made in R1, see [R1 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Track Project&nbsp;Progress with&nbsp;a Utilization Report

Now a user with Manage access to a project&nbsp;can track the progress of the&nbsp;project with a utilization report.

The utilization report enables you to keep your project within budget by allowing you to quickly see how the actual hours are tracking against the budgeted hours or planned hours&nbsp;for a given week or month, or for the overall project. In addition, you can view&nbsp;detailed information for the number of hours in each category (budgeted, planned, and actual), categorized by job role or individual user.

For more information about tracking utilization in a project, see [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

As a system&nbsp;administrator, you can configure whether the Utilization tab is available to users. By default, the Utilization tab is located in the More drop-down menu within a project. You can move the Utilization tab to another location, or you can hide it completely. If&nbsp;you have defined custom layout templates for users in your organization, you need to manually add the Utilization tab to the custom layout templates.

For more information about configuring the location of the Utilization tab, see "Customize Tabs" in "Creating and Managing Layout Templates."

## Modify an Existing Global Approval Process for&nbsp;an Individual Object

Now you can modify an existing global approval process when you associate that global approval process with an object. The modifications you make apply only to the approval process on the object where you are associating it.

For more information, see [Associate a new or existing approval process with work](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [Associate a new or existing approval process with work](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## Configure Reports to Show the New Gantt Chart by Default

You can configure the project and task reports that you create to show the new Gantt chart by default with the new option, "Show this report in a Gantt view by default."

For more information about configuring reports to show the new Gantt chart, see [Edit report settings](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

For more information about viewing the Gantt chart in project reports and task reports, see [View information in the Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)" in [View information in the Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## Recycle Bin Improvement: Tasks and Subtasks Are Restored to Their Previous&nbsp;Order

Now when you restore a task or subtask after it is deleted, the task or subtask is restored to its previous location (either in the task list or beneath the parent task), in the same order as&nbsp;it appeared prior to being deleted.

Prior to this change, tasks and subtasks that were restored were always restored as the last task&nbsp;(either in the task list or beneath the parent task), regardless of the order they appeared prior to being deleted.

For more information about restoring objects in Workfront, see [Restore deleted items](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Milestone View Improvements

The following improvements are now available when viewing a project list or project report in the Milestone view:

* **Configure whether Progress Status and Percent Complete are displayed in the view:** There is a&nbsp;new option that allow you to configure whether Progress Status icons are displayed in the Milestone view. In addition, you can also configure whether the Percent Complete information is displayed related to projects and tasks.  
  For more information, see [Use the Milestone view](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Use the Milestone view](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Edit the Percent Complete directly from the Milestone view:** Now you can edit the Percent Complete of projects and tasks directly from the Milestone view.  
  For more information, see [Use the Milestone view](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md)&nbsp;in [Use the Milestone view](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).&nbsp;

## Updated Look and Feel of Several System Setup Pages

The&nbsp;look and feel of the following pages in the System menu of the Setup area have been updated (the functionality remains the same):

* Diagnostics
* Single Sign-On (SSO) which includes:

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* Update Users for SSO

## Updated Event Notification Groupings in the Email Setup Area

The organizational headers of the Event Notifications in the Email Setup area now match the section headings that are used in the user profile settings area.

For more information about event notifications, see&nbsp; [Configure event notifications for everyone in the system](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Opt Out of Instant Notifications: In-Context Digest Configuration

The following&nbsp;options are now available within instant email notifications. These options are available only for instant notifications that also have a daily digest counterpart:

* "Add This to a Daily Digest"
* "Stop Emails of this Type"

Now, when you receive an instant email notification, you can either add that notification to a daily digest notification, or you can&nbsp;completely unsubscribe from that notification.

These options are available within the email notification. For more information about receiving email notifications, see [Adobe Workfront notifications](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Various Email Notifications Moved from the 'Action Needed' Section to Other Project-Related Sections

Several notifications have been moved from the "Action Needed" section of the user profile page to other sections, as follows:

For more information about configuring email notifications, see [Modify your own email notifications](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Notification</strong> </th> 
   <th><strong>Old Section</strong> </th> 
   <th><strong>New Section</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>An issue is added to a project I own</td> 
   <td> <p> Action Needed </p> </td> 
   <td> &nbsp; <p>Information about Projects I Own</p></td> 
  </tr> 
  <tr> 
   <td>An issue is added to a project I'm on</td> 
   <td> &nbsp; <p>Action Needed</p><p>&nbsp;</p></td> 
   <td> <p> Information about Projects I Own </p> &nbsp; </td> 
  </tr> 
  <tr> 
   <td>An unassigned issue is added to a project I own</td> 
   <td> &nbsp; <p>Action Needed</p></td> 
   <td> &nbsp; <p>Information about Projects I Own</p></td> 
  </tr> 
  <tr> 
   <td> <p> An unassigned issue is added to a project I'm on </p> </td> 
   <td> <p> Action Needed </p> &nbsp; </td> 
   <td> <p> Information about Projects I Own </p> &nbsp; </td> 
  </tr> 
  <tr> 
   <td> <p> The commit date changes for a task on one of my projects </p> </td> 
   <td> &nbsp; <p>Action Needed</p></td> 
   <td> &nbsp; <p>Information about Projects I Own</p></td> 
  </tr> 
  <tr> 
   <td> <p> The commit date changes for an issue on one of my projects </p> &nbsp; </td> 
   <td> &nbsp; <p>Action Needed</p></td> 
   <td> <p> Information about Projects I Own </p> &nbsp; </td> 
  </tr> 
  <tr> 
   <td> <p> The due date changes on a task I'm assigned to </p> </td> 
   <td> &nbsp; <p>Action Needed</p></td> 
   <td> &nbsp; <p>Information about Work Assigned to Me</p></td> 
  </tr> 
  <tr> 
   <td> <p> The due date changes on an issue I'm assigned to </p> </td> 
   <td> <p> Action Needed </p> &nbsp; </td> 
   <td> &nbsp; <p>Information about Work Assigned to Me</p></td> 
  </tr> 
  <tr> 
   <td> <p> The status changes on a task I'm assigned to </p> &nbsp; </td> 
   <td> <p> Action Needed </p> &nbsp; </td> 
   <td> <p> Information about Work Assigned to Me </p> &nbsp; </td> 
  </tr> 
 </tbody> 
</table>

## New Resource Planning Functionality (Not Available in Production in R1)

>[!NOTE]
>
>This functionality is currently available in the Preview environment. It will be removed from the Preview environment approximately one month prior to&nbsp;the R1 release to Production. It will then be re-introduced to the Preview environment in R2 Preview 1.

&nbsp;

The following changes were added to support the future Resource Planning functionality:

* The current "Resource Planning" tab has been renamed to "Legacy Resource Planning" in the People area.&nbsp;
* A new "Resource Planning" tab has been introduced in the People area where the new functionality will be developed.  
  For more information about the new Resource Planning tab, see [Get started with Resource Planning](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md)&nbsp;

* The current "Resource Pool" object has been renamed to "Legacy Resource Pool."  
  For more information about creating the new user-based Resource Pools, see [Resource pools overview](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* A new "Resource Pool" object has been created to support the new (user-based) Resource Pools.

  >[!NOTE]
  >
  >
  >   
  >   
  >   * If you are currently running reports on the existing Legacy Resource Pools, the existing reports will not change. 
  >   * If you want to create a new report for the existing (job role-based) Legacy Resource Pools, you will need to select "Legacy Resource Pools" as your object for the report. 
  >   * If you want to create a new report for the new (user-based) Resource Pools, you will need to select "Resource Pools" as your object for the report.
  >   
  >
