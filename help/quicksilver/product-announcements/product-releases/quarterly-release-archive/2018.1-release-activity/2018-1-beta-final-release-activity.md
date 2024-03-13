---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta Final release activity
description: This page describes all changes most recently available in the Preview environment with the 2018.1 Beta Final release. The functionality was made available in the Preview environment on January 31, 2018. It will be made available in the Production environment in March, 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
---
# 2018.1 Beta Final release activity

This page describes all changes most recently available in the Preview environment with the 2018.1 Beta Final release.&nbsp;The functionality was made available in the Preview environment on January 31, 2018. It will be made available in&nbsp;the Production environment in March, 2018.

>[!IMPORTANT]
>
>&nbsp;Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2018.1, see&nbsp; [2018.1 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

The 2018.1 Beta Final release contains enhancements for both Workfront administrators and other users:

**For Administrators**

* [Configure Resource Availability and User Allocations to Calculate Based on the User Schedule](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**For All Users**

* [Mobile Enhancements](#mobile-enhancements) 
* [Jira Integration](#jira-integration) 
* [Update to proofing viewer Names](#update-to-proofing-viewer-names) 
* [Change to Synchronization Cadence When Synchronizing from the Proofing Production Environment to Preview](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview) 
* [Warning Message Displays When the 2,000 Item Limit Is Reached in the Resource Planner](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Mobile Enhancements {#mobile-enhancements}

The following functionality will be coming to the Mobile App stores in the beginning of March 2018:

* New navigation: The home page of our Mobile Apps has been redesigned.
* Home on Mobile: Our new Home functionality has now been updated on our mobile apps, as well.

The new functionality is supported for both the iOS and the Android platforms.

## Jira Integration {#jira-integration}

You can now link Jira issues to Workfront tasks or issues by installing and configuring the Workfront add-on for Jira. With this integration, your Project Managers can continue working in Workfront, while your Development Engineers can continue to work in Jira, while their individual items become linked through the integration of Workfront with Jira.

You can configure the following through this integration:

* Establish triggers for Workfront assignments to automatically create Jira issues when they occur.
* Manually link Jira issues to Workfront tasks or issues that have been previously created.
* Specify fields that should be synchronized on the linked items as soon as one of the items is updated in one of the applications.

The Workfront add-on will be available for both the On-Premise and On-Demand versions of Jira. The add-on is free and will be available for downloading in the Atlassian Marketplace at the beginning of March 2018.

For more information about the Workfront add-on for Jira, including a link to download it, see [Using Workfront with Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Update to proofing viewer Names {#update-to-proofing-viewer-names}

The names of the HTML5-based proofing viewer and the Flash-based proofing viewers have been re-named throughout the Workfront system. The previous and updated names are as follows:&nbsp;

| **Previous Name** |**Updated Name** |
|---|---|
| HTML5 proofing viewer |New proofing viewer |
| Flash proofing viewer |Legacy proofing viewer |

{style="table-layout:auto"}

&nbsp;For more information about using the new proofing viewer, see [Reviewing Proofs in the proofing viewer.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Configure Resource Availability and User Allocations to Calculate Based on the User Schedule {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

The Workfront administrator can now determine how Workfront calculates resource availability and user allocation at the system level (considering hours as well as FTE availability). The Workfront administrator can configure resource availability and user allocation to be calculated either using the default schedule or the user's schedule.

This setting affects user availability in the following circumstances when scheduling resources:

* When allowing Workfront to automatically assign resources, as described in "Manually assign unassigned tasks and issues in the Scheduling areas".

* When displaying allocation indicators, as described in "Manage user allocations in the Scheduling areas".

For more information, see "Configure how Workfront calculates resource hour and FTE availability for the Scheduling area".

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 


## Change to Synchronization Cadence When Synchronizing from the Proofing Production Environment to Preview {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>This change takes effect on February 11, 2018.

Data from the Workfront Proof Production environment is now synchronized to the Workfront Proof Preview environment each week.

Prior to this change, data was synchronized from the Workfront Proof Production environment to the Preview environment on a monthly basis, whereas the data from the Workfront Production environment was synchronized to the Workfront Preview environment on a weekly basis. This discrepancy caused some synchronization errors when using Proofing functionality in the Workfront Preview environment.&nbsp;

For more information, see [Preview Sandbox Testing Environment- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).&nbsp;

## Warning Message Displays When the 2,000 Item Limit Is Reached in the Resource Planner {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

As we are currently working on a more permanent solution to improve performance in the Resource Planner, we have introduced a limit of 2,000 items for each view you can apply to the Resource Planner:

* The User View displays only 2,000 assignments
* The Project View displays only 2,000 projects
* The Role View displays only 2,000 roles

When the Resource Planner attempts to load more than 2,000 items, a notification displays alerting you that only 2,000 items can be displayed.

For more information about these limits and how they affect the Resource Planner, see [Resource Planner display limitations](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
