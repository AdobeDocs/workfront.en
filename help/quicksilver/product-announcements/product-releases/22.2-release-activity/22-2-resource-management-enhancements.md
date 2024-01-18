---
title: 22.2 Resource Management enhancements
description: 22.2 Resource Management enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
---
# 22.2 Resource Management enhancements

This page describes all Resource Management enhancements made with the 22.2 release to the Preview environment. These enhancements will be made available in the Production environment 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

the week of April 4, 2022.

For a list of all changes available with the 22.2 release, see [22.2 Release overview](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Improvements to the Workload Balancer navigation

To improve your experience when using the Workload Balancer, we have introduced the following enhancements:

* The Cancel and Save buttons when adjusting allocations are now sticky, even when the task is longer than the timeframe included on the screen or when the Summary panel displays.
* The left panel that displays the names of users and work items is now sticky, to allow you to scroll horizontally for longer timeframes and to still be able to read the names of items listed in the panel.
* You can collapse and expand all items listed in the left panel with one click instead of at the user or project level.
* The left panel is now also resizable.
* There is now a full-screen mode for the Workload Balancer.

For more information about navigating the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Access Advanced Assignments in the Workload Balancer

To make assigning work items easier and more accurate, you can now make advanced assignments when you assign work items manually in the Workload Balancer. Prior to this enhancement, you could access Advanced Assignments when editing items, from the items' headers, or in lists.

For more information, see [Assign work manually using the Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## New formula for calculating user availability when The Default Schedule preference is selected

To provide more accurate information in resource management tools, we have changed the formula that Workfront uses to calculate user availability when the Workfront administrator selects The Default Schedule in Resource Management Preferences. With the new update, Workfront uses the following formula to calculate user availability:

User Available Hours = (Default Schedule Hours - Exceptions) &#42; FTE - Time off hours

Prior to this update, Workfront used the following formula to calculate user availability when The Default Schedule was selected:

User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) &#42; User FTE value

For more information, see [Configure Resource Management preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

