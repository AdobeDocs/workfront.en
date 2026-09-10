---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overview of Task Original Duration and Original Planned Hours
description: As part of planning a project, you should determine the values for the Planned Hours and for the Duration (or Planned Duration) of every task in the project.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
TQID: https://experienceleague.adobe.com/iVgsZM7ZaG62fbKcLLzHM9ncuNXfqFX4JtcJSM7XoQ0
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
---
# Overview of task Original Duration and Original Planned Hours

As part of planning a project, you should determine the values for the Planned Hours and for the Duration (or Planned Duration) of every task in the project.

For more information about Planned Hours on tasks, see [Planned Hours overview](../../../manage-work/tasks/task-information/planned-hours.md).

For more information about task Duration, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

You can see these values in the Task Details tab, or while editing a task.

If you build a view for a task list or a task report, you can additionally see the Original Planned Hours and the Original Duration fields for the tasks.

## Original Planned Hours

The Original Planned Hours of a task represent the number of Planned Hours that a task originally had before it became a parent task. When a task becomes a parent task, the Planned Hours of the children tasks roll up to the parent task to indicate the Planned Hours of the parent.

Displaying the Original Planned Hours field in a task report or list you can see the original number of Planned Hours before the task inherited the number of Planned Hours of its children.

>[!NOTE]
>
>When you create a task, the number of Original Planned Hours is zero. If the task becomes a parent task, the value of this field is populated with the number of the Planned Hours of the task before it was changed to a parent. This value remains in this field even when the task reverts back to being a standalone task.

## Original Duration

The Original Duration of a task is the Duration that a task originally had before it became a parent task, in minutes. When a task becomes a parent, the Duration between the Planned Start Date of the earliest child and the Planned Completion Date of the last child rolls up to the parent task and becomes the Duration of the parent task. This replaces the Duration of the original task.

Displaying the Original Duration field in a task report or list you can see the original number of days for the Duration of the task before it inherited the Duration of its children.

>[!NOTE]
>
>When you create a task, the Original Duration is zero. If the task becomes a parent task, the value of this field is populated with the Duration of the task before it was changed to a parent. This value remains in this field even when the task reverts back to being a standalone task. This value displays in minutes.

## Example

For example, when two tasks are standalone tasks, their Original Duration and Original Planned Hours are zero.

![original_planned_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

When the first task becomes the parent of the second task, the Original Duration and Original Planned Hours fields are populated with the values for the Duration and Planned Hours of the task before it became a parent. The Original Duration is displayed in minutes. The Duration and the Planned Hours of the child become the Duration and the Planned Hours of the parent.

![original_and_planned_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

When the parent becomes a standalone task again, the Duration and Planned Hours revert back to the original values, while the Original Duration and the Original Planned Hours remain populated. They do not revert to zero.

![original_duration_and_planned_hours_after_reversal_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
