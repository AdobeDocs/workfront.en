---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: '2020.2 Resource Management enhancements: The Workload Balancer'
description: This page describes all Resource Management enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
---
# 2020.2 Resource Management enhancements:&nbsp;The Workload Balancer

This page describes all Resource Management enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.

For a list of all changes available with the 2020.2 release, see [2020.2 release overview](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

People are a Tier 1 asset. With the Workload Balancer, you can protect them from burnout and empower them to do their best work, while aligning them to key company strategies. Introducing a reimagined scheduling experience that allows you to visualize and manage people's workloads and demand in the same view. The user interface provides clear visual mapping of over and underutilization and is transparent to all stakeholders. People managers can use that information as an input and from the same screen rebalance the effort through the timeline, which is then reflected in the rest of the Workfront platform.

>[!NOTE]
>
>The Workload Balancer began releasing as a beta with the 2019.4 release. All Workload Balancer enhancements are generally available with the 2020.2 release. The enhancements described on this page were added with the 2020.2 release. For an overview of the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Adjust daily and weekly allocation in the Workload Balancer

To avoid the burnout of your resources, you can now adjust your users' daily and weekly allocation to work using the Workload Balancer.

Prior to this enhancement, this was only possible using the Resource Scheduling tools.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## Workload Balancer filters

To make the information in the Workload Balancer relevant to you, you can now create filters for both the Unassigned Work and the Assigned Work areas of the Workload Balancer and save them for future use. You can then edit the saved version to make small changes to it instead of starting from scratch with a new filter.

For information about filtering in the Workload Balancer, see [Manage filters in the Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## Show remaining hours in the Workload Balancer

To help you make correct assignment decisions, a new setting now allows you to view the difference of hours between the hours a user is available to work according to their schedule and the hours that they have already been allocated to work (the remaining hours). The new setting is now available in the Workload Balancer.

For information about viewing information in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (or if you are using Adobe Workfront Classic, see [Navigate the Workload Balancer](https://experienceleague.adobe.com/en/docs/workfront/using/home).)

**Available in these environments:**

* The new Adobe Workfront experience

## Show daily Planned Hours for tasks and projects in the Unassigned Work area of the Workload Balancer

To help you understand how tasks will affect the workload of your users before you assign them, the "Show allocations" setting is now managing what information displays in the Unassigned Work area of the Workload Balancer. When this setting is enabled, Planned Hours for both tasks and projects display in the Unassigned Work area of the Workload Balancer.

Prior to this change, this setting was updating only information in the Assigned Work area of the Balancer.

For information about navigating the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (or if you are using Adobe Workfront Classic, see [Navigate the Workload Balancer](https://experienceleague.adobe.com/en/docs/workfront/using/home).). 

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience (Previously available only for tasks)

## New Settings box for the Workload Balancer

To streamline your experience, a Settings box is now available that displays additional tools to update the view in the Workload Balancer. This box includes the following settings:

* Group by Project
* Display either the Allocated hours or the Remaining hours for your tasks and projects.

For information about viewing information in the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (or if you are using Adobe Workfront Classic, see [Navigate the Workload Balancer](https://experienceleague.adobe.com/en/docs/workfront/using/home).).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## Share the Workload Balancer with a link

You can now share your people's workload with executives so that they can have context about your staffing needs. For this, you can now share the Workload Balancer by sharing a unique URL to the Workload Balancer with anyone else.

For information about navigating the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (or if you are using Adobe Workfront Classic, see [Navigate the Workload Balancer](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## Alter the date range in the Workload Balancer

To further help you customize the timeline duration for the Workload Balancer to match your needs, you can now select a custom period of 2, 4, or 6 weeks to display at one time.

Prior to this enhancement, the Workload Balancer always displayed information starting with the current week.

For information about navigating the Workload Balancer, see [Navigate the Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (or if you are using Adobe Workfront Classic, see [Navigate the Workload Balancer](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience (Previously available)

## Moving and copying tasks to another project keeps the task constraint when tasks can fit within the project's timeline

We have made an improvement to the way Workfront handles the date-specific Task Constraint of a task when you copy the task or move it to another project. Examples of date-specific Task Constraints are Must Start on, Must Finish On, Fixed Dates, Start No Later Than, and so forth.

For example, when you move or copy a task with a Must Start On constraint to another project whose Planned Start Date is prior to the Start Date of the task, the task keeps the constraint after it is copied or moved. When you move or copy a task with a Must Start On constraint to a project whose Planned Start Date is after the Start Date of the task, the Task Constraint changes to As Soon As Possible.

Prior to this change, the Task Constraint always changes to As Soon As Possible.

For information about moving tasks see, [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md) (or if you are using Adobe Workfront Classic, see [Moving Tasks](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

For information about copying tasks, see [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (or if you are using Adobe Workfront Classic, see [Copy and Duplicate Tasks](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

For an overview of all Task Constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (or if you are using Adobe Workfront Classic, see [Task Constraint Overview](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## Preventing data loss while making changes in the Details tab or a task list

To prevent data loss when you are updating information on the Details page on an object or tasks in a task list at the project level when saving changes manually, a warning message now displays, to notify you that you have unsaved changes before you attempt to edit information in the header. The only actions allowed before you save your changes are subscribing or adding the object to your favorites.

For information about editing tasks in a list, see [Edit tasks in a list](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Available in these environments:**

* The new Adobe Workfront experience

## Create approval processes for groups using custom statuses

To make it easier for groups to manage their own unique workflows, you can now use group-specific custom statuses in approval processes.

Previously, a group could not use its own custom statuses with its group-specific approval processes. Only system-wide statuses were available and these didn't always fit group approval processes.

Custom statuses can be used now in both single-use and system-wide approval processes:

* Create a single-use approval process for an object (project, task, or issue) and base it on statuses that are associated with the group working on that object. This includes any custom statuses associated with the group.
* Create a global approval process and make it available only for the group or for everyone in the system.

For users with administrative access to approval processes, information about configuring approval processes is available in [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (or if you are using Adobe Workfront Classic, see [Creating Approval Processes](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

For users, information about associating approval processes with work items is available in [Associate a new or existing approval process with work](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (or if you are using Adobe Workfront Classic, see [Associating a New or Existing Approval Process with Work](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## A more convenient way to update allocations in the Workload Balancer

To make it more convenient to manage a user's allocations to a work item in the Workload Balancer, you can now double-click the work item. You can also still use the existing Edit allocations menu option. In addition, you are no longer required to enable displaying allocations to be able to update them.

For information about managing allocations in the Workload Balancer, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Update Task Planned Hours in the Workload Balancer

>[!NOTE]
>
>This enhancement will be available in Production soon after the 2020.2 release.

A new option in the Resource Management area of the access level now allows users with this access to edit Planned Hours from the Workload Balancer. When you adjust allocations in the Workload Balancer, the total of daily allocations does not need to match the number of Planned Hours of the tasks. Once you save your allocations, the total of the allocation hours will become the Planned Hours of the task. This is only possible for tasks that have a Simple Duration Type.

For information about managing allocations in the Workload Balancer, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

For information about granting access to Resource Management, see [Grant access to Resource Management](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Removing the "beta" label from the Workload Balancer

With the 2020.2 release, the Workload Balancer will no longer in a beta state and you will be able to use the Resource Balancer to review and manage your resource assignments and allocations. The "beta" label has been removed in the Preview environment. This same change will be made with the 20.2 Production release. For information about the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
