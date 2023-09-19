---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 3
description: This page describes all changes available in the Preview environment with the R1.3 release. The functionality on this page was made available in the Preview environment on February 1, 2017.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
---
# R1 Preview 3

This page describes all changes available in the Preview environment with the R1.3 release. The functionality on this page was made available in the Preview environment on February 1, 2017.

For a list of all changes made in R1, see [R1 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).&nbsp;

## Improved Method for Linking&nbsp;External Files

The option for linking documents from an external source (such as Google Drive, Box, Dropbox, and so forth) is now in a more prominent location in the Documents area.&nbsp;

In addition, the action of authorizing a document provider prior to linking files from that provider for the first time is now more intuitive (it is simply an extra step when linking files from an external provider).

Prior to these changes, the option to link&nbsp;files from an external source was located within the Add Documents dialog box within the Documents area. Before linking&nbsp;a document from an external source for the first time, the user linking&nbsp;the document had to authorize that document provider in the Setup area.

For more information, see&nbsp; [Link documents from external applications](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Updated&nbsp;Team Working On Calendar

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

The Working On calendar available for teams now contains additional functionality and an updated look and feel. The team Working On calendar now functions similar to the resource scheduling tool for projects.

The updated team Working On calendar includes the following improvements:

* View users alphabetically or grouped by role.
* Filter the scheduling timeline by project priorities, status, and individual projects. You can also filter the scheduling timeline by roles and users. (The Filter area includes fewer option than when scheduling resources for projects.)
* Include&nbsp;issues on the scheduling timeline.
* Display&nbsp;user allocations and modify the number of&nbsp;hours that users are allocated to certain tasks and issues for each day.
* View indicators that show when users are over-allocated on any given day.
* Configure whether completed work is displayed on the scheduling timeline.

Differences from the resource scheduling tool when scheduling resources for projects:

* All team members&nbsp;are displayed on the team Working On calendar.  
  When scheduling resources for projects, only users who have a role associated with them that matches a role of one or more tasks in the Unassigned area are displayed.
* The Swap tool is not available is not included in the team Working On calendar.
* Any team member can make changes on the team Working On calendar.  
  When scheduling resources for projects, only Resource Managers can make resourcing decisions for the project.
* Issues are displayed by default on the team Working On calendar.  
  When scheduling resources for projects, issues are not displayed by default.

For more information about using the updated team Working On calendar, see "Resource Scheduling".

## Resource Scheduling Enhancements

The scheduling timeline includes the following enhancements:

* "Use the Filter to Control Which Users Are Displayed on the Scheduling Timeline"
* "Users Remain on the Timeline after Being Assigned a Task"

### Use the Filter to Control Which Users Are Displayed on the Scheduling Timeline {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

The filter can now be used to control which users are displayed on the scheduling timeline, in addition to which tasks and issues are displayed in the Unassigned area. When users are selected in the filter, only the users you select are displayed, regardless of whether they have a role assignment that matches the role assignment of tasks in the Unassigned area. All tasks currently assigned to that user are also displayed.

Prior to this change, the filter controlled only which tasks and issues were displayed in the Unassigned area. Users were displayed in the scheduling timeline only if the user matched the role assignment of a task in the Unassigned area.

For more information about using the filter to control what is displayed on the scheduling timeline, see "Filter information in the Scheduling area", and "Manually assign unassigned tasks and issues in the Scheduling areas".

### Users Remain on the Timeline after Being Assigned a Task {#users-remain-on-the-timeline-after-being-assigned-a-task}

Users remain on the scheduling timeline after they are assigned a task or issue, even if there are no remaining tasks or issues that have a matching role assignment. This allows you to make any necessary changes after users&nbsp;are assigned.

Prior to this change, users would disappear from the scheduling timeline immediately after being assigned a task or issue if there were no remaining tasks or issue in the Unassigned area with a matching role assignment.

For more information, see "Manually assign unassigned tasks and issues in the Scheduling areas".

## Customize Workfront Terminology by Changing Object Names

You can now customize Workfront terminology by changing the names of certain objects.   
Using a Layout Template, you can now change the names of the following work objects to match the needs in your organization:

* Portfolio
* Program
* Project
* Task
* Issue

For example, if in your organization you work with campaigns instead of projects, you can replace the name of the "Project" object with "Campaign".

When you make this replacement, the following areas of the application show the updated name of the objects:

* Global Navigation Bar
* All tabs
* All menus&nbsp;
* Report builder and reporting elements (views, filters and groupings)
* Save buttons
* Exported files
* Emails

The following areas do not show the updated name of the objects:

* Resource Estimates
* Resource Budget Manager
* Capacity Planner
* Resource Grid
* Team Builder
* Portfolio Optimizer&nbsp;
* Mobile Apps
* Outlook Add-in

For more information about how to customize the Workfront terminology using a Layout Template, see the "Customizing Terminology" section in "Creating and Managing Layout Templates" and the "Understanding the Implications of Customizing Object Names" section in [Understand objects in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Include Approval Start and End Dates in Reports

You can now include the&nbsp;following fields when creating or modifying&nbsp;reports:

* Approval Path Start Date
* Approval Path Completion&nbsp;Date

These fields allow you to have insight into when the current or most recent approval path was started and when it was marked as Complete.

For more information about these fields, see [Glossary of Adobe Workfront terminology](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

For more information about approval paths, how they are created and triggered, and the function they serve in approval processes, see [Create an approval process for work items](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

The following fields were removed from Workfront and can no longer be included in reports (these fields provided information regarding the project rather than information about the approvals themselves, and were often misused):

* Approvals Planned Start Date
* Approval Projected Start Date
* Approval Estimated Start Date

## New Email Digest Options for "Requests I Have Made"

The Daily Digest delivery option has been added to the "Requests I Have Made" area of your Notifications settings.

For more information, see [Modify your own email notifications](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Remember to update the email address associated with your account to be able to test this functionality. This is required because the Preview Sandbox clears the email addresses on all users.

## Updated Look and Feel of Document Approval Email Notifications

The look and feel of the notification for "Document Approval" has been updated with a new UI:

For more information about email notifications, see [Adobe Workfront notifications](../../../../workfront-basics/using-notifications/wf-notifications.md).

Remember to update the email address associated with your account to be able to test this functionality. This is required because the Preview Sandbox clears the email addresses on all users.

## Enhancements&nbsp;in the Milestone View

The Milestone view that is available when viewing a project list or project report now contains the following enhancements:

* Planned dates are editable
* Percent Complete for projects and tasks is displayed

Prior to this change, in order to edit the dates or view percent complete, you had to go to the individual task.

For more information, see [Use the Milestone view](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
