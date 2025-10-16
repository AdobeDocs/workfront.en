---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: Projected Duration Does not Match Planned Duration
description: "This article describes troubleshooting in Adobe Workfront when you might receive the following message:'The Projected Duration of a Task/ Issue has gone to 0 and does not match the Planned Duration.'"
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
---
# Projected Duration does not match Planned Duration

## Problem

You receive the following error message: "The Projected Duration of a Task/ Issue has gone to 0 and does not match the Planned Duration."

## Cause

This is caused when the Projected Start Date matches the Projected Completion Date.

## Solution

There are many factors that can cause the Projected Start and Completion dates to match. This problem is largely tied to the allocation of time on the task or issue in question.

In most cases, depending on the Duration Type and Task Constraint on the task, the allocation should extend the Projected Completion Date out much further than expected. However, in some cases based on the way Duration Type and Task Constraint are configured, it is possible that this will instead be zero. 

Here are the best things to check in those cases with links to their supporting articles:

* Projected Completion Date: [Overview of the Projected Completion Date for projects, tasks, and issues](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* Task Constraint: [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* Duration Type: [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

If the Projected Completion Date, Task Constraint, or Duration type are working as expected, contact support for more in-depth troubleshooting.
