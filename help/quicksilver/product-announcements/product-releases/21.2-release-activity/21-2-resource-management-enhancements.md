---
content-type: release-notes
keywords: notes,quarterly,update,release
navigation-topic: 2021-2-release-activity
title: 21.2 Resource Management enhancements
description: This page describes all Resource Management enhancements made with the 21.2 release to the Preview environment. These enhancements will be made available in the Production environment the week of May 10, 2021. For a list of all changes available with the 21.2 release, see 21.2 Release overview.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
TQID: https://experienceleague.adobe.com/cAM0R2azvfhRW25brnRKCUXZ5f2ZLGeBVd19okbdBpU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource Management
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
    internal-label: Workload Balancer
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
    internal-label: Resource Planner
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
---
# 21.2 Resource Management enhancements

This page describes all Resource Management enhancements made with the 21.2 release to the Preview environment. These enhancements will be made available in the Production environment the week of May 10, 2021. For a list of all changes available with the 21.2 release, see [21.2 Release overview](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Month-level view in the Workload Balancer

To help you manage the allocation of resources for larger periods of time, we have now implemented a month-level view for the Workload Balancer. You can view up to three months at a time and update monthly resource allocations. Prior to this change, you could view the Workload Balancer only by day or week.

For information, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Connection between the Scenario Planner, Workload Balancer, and task list

>[!NOTE]
>
>Available only in the new Adobe Workfront experience.

To help you with the strategic planning of your projects and ensure they align with the bigger-picture initiatives of the Scenario Planner, we have created a new area on the project that displays job role requirements from the initiatives as well as planned hours estimated on the project's work items. This area is available for the project-level Workload Balancer as well as for the task list in the new Workfront experience. In the classic experience this is available only for the project Workload Balancer.

For information, see the following articles:

* [Overview of reconciling resource allocations between projects and initiatives](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>This new functionality is visible to all users, in both the new and the classic Workfront experience. This is also visible to customers who have not purchased a Workfront Scenario Planner license.

## Use Planned Hours when calculating Net values in the Resource Planner

A new setting in the Resource Planner allows you to use Planned Hours when calculating Net values.

Prior to this enhancement, Workfront calculated Net values only using Budgeted Hours. Net values display the difference between Available and Budgeted or Planned hours, FTE, or cost. Budgeted Hours is still the default setting when calculating Net values.

For information, see [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 12-week view in the Workload Balancer

You can now view up to 12 weeks of information in the Workload Balancer. Prior to this enhancement, you could view 2,4, and 6 weeks of information.

For information about viewing the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Navigate the Workload Balancer.

## Change in the way the Job Role filter works in the Unassigned area of the Workload Balancer

To improve the way the Job Role filter works in the Workload Balancer and to match users' expectations, we have modified the functionality of the filter in the Unassigned area. You can now view only the hours allocated to the job roles you specify in the filter.

Prior to this enhancement, when applying the Job Role filter to the Unassigned area the Workload Balancer displayed all hours associated with the work items assigned to the job roles .

For information about filtering information in the Workload Balancer, see [Manage filters in the Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
