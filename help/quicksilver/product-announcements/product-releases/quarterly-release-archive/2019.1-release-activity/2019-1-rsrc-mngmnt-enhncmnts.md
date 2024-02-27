---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Resource Management enhancements
description: This page describes all Resource Management enhancements included with the 2019.1 release. The functionality is now available in the Production environment.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
---
# 2019.1 Resource Management enhancements

This page describes all Resource Management enhancements included with the 2019.1 release. The functionality is now available in the Production environment.

For a list of all changes made in 2019.1, see [2019.1 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Updated Default Filter in the Resource Planner

The default filter in the Resource Planner no longer filters by the Group of the Project.

When viewing the Resource Planner, you now see only the projects that are current and date-sensitive by default. Information from the following projects is included by default:

* With a Planned Completion Date that occurs after the first date of today's month. 
* With a Planned Start Date that occurs before the last date of the fourth month from today. 
* With a Status of Current or Planning.

Previously, the default filter would retrieve the information from the following additional projects:

* With a Planned Completion Date that occurs after the first date of today's month. 
* With a Planned Start Date that occurs before the last date of the fourth month from today. 
* With a Status of Current or Planning. 
* With a Group that matches the Home Group of the user who is logged in.

For information about applying filters to the Resource Planner, see [Filter information in the Resource Planner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Using Wildcards for Resource Planner Filters

You can now use wildcards when building filters in the Resource Planner. For example, you can use $$USER.ID to filter for information about the user who is logged in, or $$USER.companyID to filter information about all the users that belong to the same company as the user who is logged in. For a complete list of user-based variables, see the [User-based wildcard filter variables](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) section in [Wildcard filter variables](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Previously, wildcards were not available for the Resource Planner filters.

For information about filtering in the Resource Planner, see [Filter information in the Resource Planner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## Support for Date-Based Wildcard Filter Variables in the Resource Planner

You can now use any version of the $$TODAY wildcard filter variable when you build a filter in the Resource Planner.

Prior to this enhancement, you could use only user-based wildcard filter variables.

For information about filtering in the Resource Planner, see [Filter information in the Resource Planner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

For information about wildcard filter variables, see [Wildcard filter variables](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Export Options for the Role View in the Resource Planner

You can now select which levels of information to export from the Resource Planner in the Role view. You can export any of the following:

* Roles only 
* Roles and Projects 
* Roles, Projects, and Users

Prior to this enhancement, all levels of information were exported in the Role view. These options have been introduced to the Project and User views in a previous release.

For information about exporting information from the Resource Planner, see [Export information from the Resource Planner](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Data Formatting Options for Exporting the Resource Planner

You can now select how you want to display information in the Excel file when exported from the Resource Planner.

You can display the availability and allocation of information exported from the Resource Planner in the following ways:

* Ungrouped by the name of the objects it belongs to. In this case, the names of the objects it belongs to are displayed on each row of data. (this is the default option) 
* Grouped by the name of the objects it belongs to. In this case, the information in the exported file appears as it is displayed in Workfront.

Prior to this enhancement, the information in the exported file appeared as it appears in Workfront.

For information about exporting information from the Resource Planner, see [Export information from the Resource Planner](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Persistent Scheduling Timeline

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Scheduling timelines now keep the timeframe you have selected when you refresh the timeline or navigate away from the page.

Prior to this enhancement, the scheduling timelines returned to the default timeframe when you refreshed or navigated away from the page.

This enhancement is available in the following areas:

* Scheduling tab in the People area 
* Team Working On tab 
* Scheduling subtab on the Staffing tab of a Project

For information about working with the timeline in the Resource Scheduling areas, see "Get started with Resource Scheduling".

## New Export Options in the Resource Planner

You can now select which levels of information to export from the Resource Planner. In the Project view, you can export any of the following:

* Projects only 
* Projects and Roles 
* Projects, Roles, and Users

In the User View, you can export any of the following:

* Users only 
* Users and Projects 
* Users, Projects, Roles, Tasks, and Issues

Prior to this enhancement, all levels of information were exported in all the views of the Resource Planner by default.

For information about exporting information from the Resource Planner, see [Export information from the Resource Planner](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Update to the User View in the Resource Planner

All users in the system now display in the User View of the Resource Planner, but only the users associated with the filtered projects also show hour information.

Prior to this update, only the users assigned to work items on the projects you filter for displayed in the User View of the Resource Planner.

You can use user-based filters to reduce the number of users displayed in the User View to only those who are assigned to the projects you want to display.

For information about filters in the Resource Planner, see [Filter information in the Resource Planner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
