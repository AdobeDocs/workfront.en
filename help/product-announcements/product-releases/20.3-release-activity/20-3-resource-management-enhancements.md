---
filename: 20-3-resource-management-enhancements
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Resource Management enhancements
description: This page describes all Resource Management enhancements made with the 20.3 release to the Production environment. These enhancements were made available in the Production environment the week of August 10, 2020.
---

# 20.3 Resource Management enhancements

This page describes all `Resource Management` enhancements made with the `20.3` release to the Production environment. These enhancements were made available in the Production environment the week of August 10, 2020.

For a list of all changes available with the `20.3` release, see [20.3 release overview](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Include hours from issues in the Assigned Work area of the Workload Balancer

To allow you to see a complete picture of all your people's workloads, we have introduced a setting that allows you to include hours from issues in the Assigned Work area of the Workload Balancer.

For information about working in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

`<iframe class="vimeo-player_0" src="assets/430815976?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>`

[View this video in full-screen mode.](https://vimeo.com/430815976/8c304e9fe7)

## Adjust allocations for non-working days in the Workload Balancer

You can adjust allocations for your resources for non-working days using the Workload Balancer.

For information about managing allocations in the Workload Balancer, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

`<iframe class="vimeo-player_0" src="assets/430817953?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>`

[View this video in full-screen mode.](https://vimeo.com/430817953/738e8b3539)

## Variable filters available in the Workload Balancer

To improve your experience as well as to give you more flexibility when you share information, we have now implemented variable filters for the Workload Balancer. The following filters have been added to the Workload Balancer:

* "Me" (when filtering by users)
* "My Primary Role" (when filtering by roles)
* "My Home Team" or "All My Teams" (when filtering by teams).

These filters replace the wildcard filter variables of $$USER.ID, $$USER.roleID, $$USER.homeTeamID, and $$USER.teamIDs

When you apply one of these filters and then share the Workload Balancer or place it on a dashboard, all other users will see their own information.

For information about applying filters to the Workload Balancer, see [Manage filters in the Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

`<iframe class="vimeo-player_0" src="assets/425680462?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>`

[View this video in full-screen mode.](https://vimeo.com/425680462/5e65fb50f7)

## New sorting for projects in the Workload Balancer

The Workload Balancer now sorts the projects based first on the earliest Planned Start Date and secondly the latest Planned Completion Date of the tasks in the project which occur during the timeframe the user displays on the screen. This allows you to organize work in a tree-like hierarchy which helps you more easily identify work for a day.

For information about viewing projects and work items in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

`<iframe class="vimeo-player_0" src="assets/425681656?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>`

[View this video in full-screen mode.](https://vimeo.com/425681656/50139ed937)

## Display actual work progress in the Workload Balancer

To give you an accurate perspective of the progress of your workload, we have introduced a new setting in the Workload Balancer that shows the timeline of tasks and issues according to their Projected Dates. You can enable the Show Projected Dates setting to view the projected timeline of the work item in addition to the planned timeline.

Also, with this improvement, if a task or an issue is completed earlier than their Planned Completion Date, the allocated hours from the remaining days are struck through to indicate that they do not count towards the user’s overall allocation.

For information about navigating the Workload Balancer and enabling settings see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

`<iframe class="vimeo-player_0" src="assets/434808390?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>`

[View this video in full-screen mode.](https://vimeo.com/434808390/495d145726)

## Workload Balancer features previously communicated as releasing with the 20.2 release

* [Adjust daily and weekly allocation in the Workload Balancer](#adjust) 
* [Update Task Planned Hours in the Workload Balancer](#update) 
* [A more convenient way to update allocations in the Workload Balancer](#a)

### Adjust daily and weekly allocation in the Workload Balancer

To avoid the burnout of your resources, you can now adjust your users' daily and weekly allocation to work using the Workload Balancer.

Prior to this enhancement, this was only possible using the Resource Scheduling tools.

For information about managing allocations in the Workload Balancer, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

`Available in these environments:`

* `Adobe Workfront Classic` 
* `The new Adobe Workfront experience`

`<iframe class="vimeo-player_0" src="assets/405985254?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>`

[View this video in full-screen mode.](https://vimeo.com/405985254/2012ee6036)

### Update Task Planned Hours in the Workload Balancer

>[!NOTE]
>
>This enhancement will be available in Production soon after the 2020.2 release.

A new option in the Resource Management area of the access level now allows users with this access to edit Planned Hours from the Workload Balancer. When you adjust allocations in the Workload Balancer, the total of daily allocations does not need to match the number of Planned Hours of the tasks. Once you save your allocations, the total of the allocation hours will become the Planned Hours of the task. This is only possible for tasks that have a Simple Duration Type.

For information about managing allocations in the Workload Balancer, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

For information about granting access to Resource Management, see [Grant access to Resource Management](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### A more convenient way to update allocations in the `Workload Balancer`

To make it more convenient to manage a user's allocations to a work item in the `Workload Balancer`, you can now double-click the work item. You can also still use the existing Edit allocations menu option. In addition, you are no longer required to enable displaying allocations to be able to update them.

For information about managing allocations in the Workload Balancer, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
