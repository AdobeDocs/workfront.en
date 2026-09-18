---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Task Slack Date Overview
description: Tasks can sometimes start and complete late without impacting the Completion Date of the project. The Slack Date displays the exact date when a task could definitely impact the Completion Date of the project.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
TQID: https://experienceleague.adobe.com/p2lKXWr-25jYKmV38ifdEJcyJf72FZMYRccaNiD5gTw
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
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
---
# Task Slack Date overview

Tasks can sometimes start and complete late without impacting the Completion Date of the project.

The Slack Date displays the exact date when a task could definitely impact the Completion Date of the project.

## Slack Date overview

The Slack Date is different than the Projected Completion Date, as the predecessor relationships and task constraints increase the slack time.

Consider the following scenarios, depending on whether a task is on the Critical Path of a project or not:

* For tasks that are on the Critical Path of the project or have successors that are on the Critical Path, the Slack Date matches the Projected Completion Date of the task unless the Progress Status of the task is already Late or Behind.

  For information about the Critical Path, see [Overview of the project Critical Path](../../../manage-work/tasks/manage-tasks/critical-path.md).

  For information about the Progress Status of tasks, see [Task Progress Status overview](../../../manage-work/tasks/task-information/task-progress-status.md).

* For tasks that are not on the Critical Path, the slack time increases the earlier the task is scheduled. For these tasks, the Slack Date remains in the future until the tasks become so late that they begin to impact the Completion Date of the project.

## Locate the Slack Date of a task

To view the Slack Date of a task, you can add the Slack Date field to a task view or report.

For information about building a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
