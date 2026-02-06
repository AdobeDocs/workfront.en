---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Difference between Planned Duration and Duration for Tasks
description: Duration is the amount of time between the Planned Start and Planned Completion Date of a work item. Tasks have a Duration and a Planned Duration in Adobe Workfront, depending on the Duration Type of the task.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
---
# Difference between Planned Duration and Duration for tasks

Duration is the amount of time between the Planned Start and Planned Completion Date of a work item. Tasks have a Duration and a Planned Duration in Adobe Workfront, depending on the Duration Type of the task.

Issues and projects cannot be associated with a Duration Type and they have only a Duration.

## Task duration

For tasks, the Duration and the Planned Duration typically show the same value: the length of time between the Planned Start Date and the Planned Completion Date of a task.

When the Duration Type of the task is Effort Driven, the Planned Duration diminishes as you are adding resources to the task. 

**Example:** If a task with a Duration Type of Effort Driven has a Duration of 3 days and you assign one resource with a full-time schedule to the task, the Planned Duration is 3 days, as well.

If you assign three resources with a full-time schedule to the same task, the Duration stays 3 days, but the Planned Duration becomes 1 day. The Planned Duration also changes the Planned Start and Planned Completion dates of the task, to reflect the new Planned Duration. As a result, the timeline of the project is affected as well. 
You can use the Effort Driven Duration Type when you assign a task to multiple resources. This reduces the time it takes for the work to be completed on the task.

For more information about the Effort Driven Duration Type, see [Duration Type overview: Effort Driven](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Issue and project duration

Issues and projects have only one Duration value, which is the difference between the Planned Start Date and Planned Completion Date of the issue and of the project, respectively.
