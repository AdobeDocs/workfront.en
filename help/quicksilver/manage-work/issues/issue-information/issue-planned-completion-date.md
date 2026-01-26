---
product-area: projects
navigation-topic: issue-information
title: Overview of the Issue Planned Completion Date
description: The Planned Completion Date of an issue is the date by which the issue is expected to complete.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
---
# Overview of the issue Planned Completion Date

<!--Audited: 08/2025-->

The Planned Completion Date of an issue is the date by which the issue is expected to complete. 

You can either specify the Planned Completion Date of an issue, or you can leave it up to Adobe Workfront to calculate it depending on certain criteria. 

The Planned Completion Dates of issues do not affect the Planned Completion Date of the project. Only tasks' Planned Completion Dates affect the Planned Completion Date of the project. For more information about the project Planned Completion Date, see [Set the project Planned Completion Date](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>The Planned Completion Date of an issue differs from the Commit Date of the issue or the Projected Completion Date of the issue in the following ways:
>
>* The Commit Date is the date by which the person assigned to the issue manually estimates that they will have completed the issue. For more information see the following articles:
>
>   * [Commit Date overview](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md) 
>   * [Interactions between the Commit Date and the Planned Completion Date](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* The Projected Completion Date is a date calculated by Workfront that takes into account external factors to determine a real-life date for when the issue can be realistically completed. For more information, see [Overview of the Projected Completion Date for projects, tasks, and issues](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Manually set the Planned Completion Date of an issue

You must have Edit access to Issues and Manage permissions on the issue to be able to update the Planned Completion Date of the issue.

You can manually set the Planned Completion Date of an issue in the following areas of Workfront:

* In the Edit Issue box or in the Issue Details area when creating or editing an issue. For information, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).
* In the Home area if the Planned Completion Date displays in the Summary panel of an issue. For information, see [Update or edit a work item in the Home area](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* In the issue header. For information, see [New object headers](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In an issue list or report when the Planned Completion Date field displays in the view.

  For information, see [Edit issues in a list](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## How Workfront automatically calculates the Planned Completion Date for an issue

When Workfront calculates the Planned Completion Date of an issue automatically, the following can influence the date:

* Planned Start Date

  The Entry Date and Planned Start Date should match on an issue when you first create the issue.

* The Default Duration as configured in the Queue Details section of the project. For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

  If the Default Duration is 0 Days, the Planned Completion Date matches the Planned Start Date of the issue.

* Project Schedule

When set automatically, the Planned Completion Date is determined based on the following calculation: 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Example:** For example, if your task has a start date of Friday, January 14 and the Default Duration is 5 Days, the Planned Completion Date is Friday, January 21, if the Project Schedule is Monday-Friday for 8 hours a day.

The following situations exist:

* If the project does not have a Schedule, the Default Schedule of your Workfront system is taken into account. For information, see [Schedules overview](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* If the Schedule is Monday-Friday 9 AM to 1PM (4 hours a day) and your Workfront system's Typical hours per work day is 8 hours, the Planned Completion Date is January 27.

>[!TIP]
>
>Workfront takes into account Schedule Exceptions like holidays and weekends when calculating Planned Completion Dates.

 
