---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: Projected Duration Does not Match Planned Duration
description: This article describes troubleshooting in Adobe Workfront when you might receive the following message:'The Projected Duration of a Task/ Issue has gone to 0 and does not match the Planned Duration.'
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
TQID: https://experienceleague.adobe.com/cdGUhn51Xeqie8iW75phQTQKMvdO2ub-HSjcCjcHLec
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
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
