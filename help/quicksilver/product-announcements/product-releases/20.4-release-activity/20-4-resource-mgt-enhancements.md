---
title: 20.4 Resource Management enhancements
description: 20.4 Resource Management enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
---
# 20.4 Resource Management enhancements

This page describes all Resource Management enhancements made with the 20.4 release to the Preview environment. These enhancements will be made available in the Production environment the week of November 9, 2020.

For a list of all changes available with the 20.4 release, see [20.4 release overview](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Plan work using Work Effort instead of Planned Hours

To give you flexibility when you're planning work on your projects, we have introduced the new concept of Work Effort for tasks. You can estimate whether the Work Effort for a task is small, medium, or large without manually estimating the Planned Hours for the task. Each level of effort is calculated based on a percentage of time from the typical hours per day as configured in your instance.

The following improvements are now available with this new feature:

* Enable this setting for projects and templates to make it available for tasks and template tasks
* Update this setting for each task with a Simple Duration Type which automatically updates the Planned Hours of the task
* Disable this setting using a Layout Template for users who would rather continue using Planned Hours.
* Display the value of this new field in a task list or report.

For information about Work Effort, see [Work Effort overview](../../../manage-work/tasks/task-information/work-effort.md).

This feature is now included in the [Planner Fundamentals, Part 2 learning path](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) on Workfront One.

## Project status-based colors for work items in the Workload Balancer

For better visibility and increased customization of your experience in the Workload Balancer, you can now change the colors of the projects and their work items to match the status of the projects' status. The colors correspond to group-level or system-level project statuses. The colors displayed can correspond to both system as well as custom project statuses.

For information about customizing the view in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Adjust user allocation using percentage values in the Workload Balancer

You can now manage your users' allocations in the Workload Balancer using percentages instead of hours.

For information about managing allocations in the Workload Balancer, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Show or hide completed work in the Workload Balancer

A new setting now allows you to show or hide completed work items in the Workload Balancer. The setting is enabled by default and completed work items that match the filtering criteria and the time frame selected display in the Workload Balancer.

Prior to this enhancement, completed work items always displayed in the Workload Balancer.

For more information about adjusting settings in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Usability improvements in the Workload Balancer

To ensure a streamlined and user-friendly experience when you manage your resources in the Workload Balancer, the following usability improvements are now available:

* You can now open the Summary for issues and tasks from the Summary icon instead of the More menu. This experience is now consistent to that of lists.

  >[!NOTE]
  >
  >This option is available only in the new Adobe Workfront experience.

* You can access the More menu to the left of an object bar rather than at the end of an object bar. This makes it easier to find when objects span a long period of time.
* You can access the assignment features with a keyboard shortcut. Previously, this was available only from the More menu.
* You can load all remaining items under a user's name instead of just the following 20 items by clicking Load More.

For more information about navigating the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## User allocation chart in the Workload Balancer

To allow you to have a high-level visual representation of users' allocation within a given time frame, a new setting now enables a chart view for how allocations are displayed in the Workload Balancer. Enabling this setting displays the users' allocation in a line chart that indicates the overallocations in red blocks, and the underallocations in blue.

For more information about configuring settings in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualize completed work in the Workload Balancer

To allow you to easily identify work that has already been completed so you can manage user assignments correctly, we have enabled a visual indicator in the Workload Balancer that shows when items for a selected time frame have been completed. You can now see a green check mark for tasks, issues when they are completed. The project also displays the green check mark when there are work items completed during the time frame displayed on the screen.

For information about viewing information in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## New Default filter for the Assigned Work area in the Workload Balancer

The Default filter for the Assigned Work area in the Workload Balancer now displays only users that are members of all the teams that you, as the logged-in user, are associated with. The new filter now displays the most relevant information to you, by default.

Before this enhancement, all users that you had access to view displayed in this area.

For information about using filters in the Workload Balancer, see [Manage filters in the Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## New icon for switching between hours and percentage values, or allocated and remaining time in the Workload Balancer

We have added a new setting that allows you to switch between allocated Hours and Percentages as you view the Workload Balancer. With this new icon, we have also eliminated the User Workload section in the Settings panel. The Workload Balancer shows allocated time by default, and we have moved the Remaining hours setting to the new Percentage or Hours icon.

This improvement eliminates clicks and makes navigating the Workload Balancer easier and more efficient.

For information about managing settings for the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## A new built-in filter for the Workload Balancer: Users on projects

To make your filtering experience in the Workload Balancer more efficient, we have added a new built-in filter in the Assigned Work area. You can now apply the Users on projects filter which displays users assigned to tasks and issues in the projects you specify.

For information about using filters in the Workload Balancer, see [Filter information in the Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

