---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 4 release activity
description: This page describes all changes most recently available in the Preview environment with the 2017.3 Beta 4 release. The functionality on this page was made available in the Preview environment the week of September 25, 2017. It will be made available in the Production environment in early November, 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
---
# 2017.3 Beta 4 release activity

This page describes all changes most recently available in the Preview environment with the 2017.3 Beta 4 release. The functionality on this page was made available in the Preview environment the week of September 25, 2017. It will be made available in&nbsp;the Production environment in early November, 2017.

>[!IMPORTANT]
>
>&nbsp;Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2017.3, see&nbsp; [2017.3 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

The 2017.3 Beta 4 release contains enhancements for both for Workfront administrators and other users:

**For Administrators**

* [New Resource Management Preferences Area in the Setup Area](#new-resource-management-preferences-area-in-the-setup-area)

**For All Users**

* [Duplicate Tasks](#duplicate-tasks) 
* [Automate Assignments When Scheduling Resources](#automate-assignments-when-scheduling-resources) 
* [Modify Assignments for Multiple Tasks When Scheduling Resources](#modify-assignments-for-multiple-tasks-when-scheduling-resources) 
* [Apply FTE Distribution to the Resource Planner](#apply-fte-distribution-to-the-resource-planner) 
* [Job Role Section for User Settings Includes Percentage of FTE Availability](#job-role-section-for-user-settings-includes-percentage-of-fte-availability) 
* [Save and Manage Filters in the Utilization Report on a Project](#save-and-manage-filters-in-the-utilization-report-on-a-project) 
* [Additional Filtering Options in the Utilization Report](#additional-filtering-options-in-the-utilization-report) 
* [View the Utilization Report by Program or Portfolio](#view-the-utilization-report-by-program-or-portfolio) 
* [Show Original Issue Information in Project and Task Reports](#show-original-issue-information-in-project-and-task-reports) 
* [Filter System Updates in the Update Stream Is Now Persistent across Objects](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects) 
* [Report on Active Proof Stages within Workfront](#report-on-active-proof-stages-within-workfront) 
* [Assign Custom Workfront Proof Permission Profiles to Users within Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront) 
* [Hour Resource Added to Event Subscriptions](#hour-resource-added-to-event-subscriptions)

## Duplicate Tasks {#duplicate-tasks}

You can now quickly duplicate a task or a set of tasks within a project. This action creates an identical task to the original one. There are no additional options during the duplication process that would allow you to make any changes to the newly created task. &nbsp;

Prior to this change, you could copy a task to either a new project, or the existing project and modify some information as you copied it.

For &nbsp;more information about duplicating tasks, see [Copy and duplicate tasks](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automate Assignments When Scheduling&nbsp;Resources {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

You can now allow Workfront to automatically propose assignments for unassigned tasks and issues when scheduling resources for multiple projects (from the Scheduling tab) or when scheduling resources for a single project (from the Staffing tab).

Workfront analyzes current work assignments across your available users and propose intelligent, logical assignments for any tasks or issues&nbsp;that are&nbsp;not yet assigned. You can modify any proposed or existing assignments prior to finalizing&nbsp;the assignments.

For more information, see "Manually assign unassigned tasks and issues in the Scheduling areas".

## Modify&nbsp;Assignments for&nbsp;Multiple Tasks When Scheduling Resources {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

When assigning, swapping, or unassigning users in&nbsp;bulk when scheduling resources (either from the Scheduling tab or the Staffing tab), you can now modify assignments for specific&nbsp;tasks that you designate (including&nbsp;all sub-tasks and associated issues) within one or more projects.

Prior to this change, you could modify assignments to tasks and issues only across entire projects (you could not designate specific tasks within a project).

For more information, see "Manually assign unassigned tasks and issues in the Scheduling areas".

## Apply FTE Distribution to the Resource Planner {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>This functionality is not currently available in Preview on all clusters.

You can now display the correct amount of Available Hours for each role of the user based on the Percentage of FTE Availability for each role, when users have more than one role.

For example, if the schedule of a user indicates that they are available to work 100 hours in one month, and their Percentage of FTE Availability for the Primary Role is 75% and the Percentage of the FTE Availability of their Other Role is 25%, the Resource Planner will list the user with 75 Available Hours under the Primary Role and with 25 Available Hours under their Other Role.

Prior to this change, the name of the user displayed in the Resource Planner only for the Primary Role, and the full availability of the user based on their schedule (100 hours) was associated only with the Primary Role. The user's Other Role displayed in the Resource Planner only if the user was assigned to a task in that role and the Available Hours for the user in the Other Role were zero.

For more information about how Available Hours and Available FTEs are calculated for users and roles in the Resource Planner, see [Overview of calculating hours and FTE for users and roles in the Resource Planner](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Job Role Section for User Settings Includes Percentage of FTE Availability {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>This functionality is not currently available in Preview on all clusters.

Now when updating a user profile, you can add additional job roles to a user and define the percentage of the FTE allocated to each job role.

Prior to this change, you could not allocate a specific amount of FTE to any of the job roles with which the user was associated.

For more information about updating the Percentage of FTE Availability for the user's job roles, see [Edit a user's profile](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)&nbsp;or [Configure My Settings](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## New Resource Management Preferences Area in the Setup Area {#new-resource-management-preferences-area-in-the-setup-area}

You can now find a new area in Setup called Resource Management. In this area, we have introduced a setting which allows you to specify how to calculate user availability in the Resource Planner. You can calculate it using the following methods:

* Manually: The Default Schedule of the system in addition to the individual FTE of the user are used to determine the hour availability of the user in the Resource Planner. The Schedule of the user is ignored.
* Automatically: The Schedule of the user is used to determine the hour availability of the user in the Resource Planner. The FTE availability is calculated based on the Schedule of the user and the Default Schedule. The value of the user FTE is ignored.&nbsp;

For more information about configuring Resource Management preferences for your system, see [Configure Resource Management preferences](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Save and Manage Filters in the Utilization Report on a Project {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Now you can save filters that you create in the Utilization report. Additionally, you can rename a saved filter, duplicate a saved filter, delete a saved filter, or modify a saved filter.

Previously, you had to specify individual filter options each time you filtered the Utilization report.

For more information about saving and managing filters in the Utilization report, see [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Additional Filtering Options in the Utilization Report {#additional-filtering-options-in-the-utilization-report}

Now when running the Utilization report, new filtering fields for Portfolios, Programs, and Projects are now available&nbsp;when creating your filter, in addition to the&nbsp;Tasks, Issues, and Roles fields that were previously available.

Prior to this change, the you could filter by portfolio, program, and project only by adding a new filter rule.

For more information,&nbsp;see [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## View the Utilization Report by Program or&nbsp;Portfolio {#view-the-utilization-report-by-program-or-portfolio}

You can now view a Utilization report by program or portfolio. This enables you to see information from&nbsp;multiple projects within a single Utilization Report.

To facilitate this change, the Utilization tab&nbsp;is now available both in the Reporting area within Workfront, as well as within an&nbsp;individual project.

Prior to this change, Utilization Reports could be accessed&nbsp;only within a project.

For more information, see&nbsp; [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).&nbsp;

## Show Original Issue Information in Project and Task Reports {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>This functionality is not currently available in Preview on all clusters.

You can now find the following information about the original issue in a project or task report, for the projects and tasks that were created by converting an issue:

* Original Issue Entry Date
* Original Issue Name
* Original Issue Originator ID

This information can be displayed in a task or project report or list by building a custom view in text mode.

Prior to this change you were not able to report on this information.

For more information about building the custom text mode view which captures the information from the original issue, see [View: display original issue information on task and project lists](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Filter System Updates in the Update Stream Is Now Persistent across Objects {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>This functionality did not release to the Preview environment with Beta 4. It will be available in Preview the first half of October.

The Filter System Updates option is now persistent across objects throughout the Workfront site. This allows you to hide system updates and view only user comments in the Update Stream on one object, and have that setting remain as you browse to other objects.

Prior to this change, you had to choose to filter out system updates for each object as you browsed the Workfront site.

For more information, see [Update work](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Report on Active Proof Stages within Workfront {#report-on-active-proof-stages-within-workfront}

When creating a Document Version report within Workfront, there is now a column called "Active Proof Stages." This column allows you to view the proof stage that is currently active on each document version in the report. The name of the stage is displayed in the "Active Proof Stages" column. If no stage is currently active on the document version, the column is blank.

For more information about available fields in views and reports, see [Glossary of Adobe Workfront terminology](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Assign Custom Workfront Proof&nbsp;Permission Profiles to Users within&nbsp;Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Now when enabling proofing capabilities for a user in Workfront, you can assign a custom Workfront Proof permission profile.&nbsp;

Prior to this change, only the following permission profiles were available: Supervisor, Manager, Administrator.

## Hour Resource Added to Event Subscriptions {#hour-resource-added-to-event-subscriptions}

Using the new Hour resource, you can now create an event subscription to keep your billing application in sync with Workfront.

To learn more about event subscriptions, see [Event Subscription API](../../../../wf-api/general/event-subs-api.md).
