---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Task Dependency Loop Overview
description: When adding predecessor relationships to tasks you might encounter dependency loops. For information about predecessors, see Overview of task predecessors.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
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
# Task dependency loop overview

When adding predecessor relationships to tasks you might encounter dependency loops. For information about predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Dependency loop overview

Dependency loops happen when you have two or more tasks that depend on each other to be completed. Adobe Workfront does not allow you to create a predecessor relationship between tasks if it creates a dependency loop.

**Example:** Task 2 is a predecessor to Task 1, which means you must complete Task 2 before you can start working on Task 1.

If you try to make Task 1 a predecessor to Task 2, you get a dependency loop error because you cannot start Task 1 until Task 2 has been completed, but task 2 cannot be started until Task 1 is finished.

![Dependency loop error message](assets/dependency-loop-error-message-350x209.png)

![Dependency loop in task list](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considerations about dependency loops

* Dependency loops can involve more than two tasks. Sometimes any number of parents of the tasks you are connecting with a predecessor relationship are the ones creating the dependency loop. 
* A dependency loop can also happen if you try to make a parent the predecessor of a child. 
* In the case of a dependency loop you cannot save the tasks or the project. In order to fix the dependency loop, you must reevaluate the predecessor relationship between the tasks listed in the error message and remove the conflicts before you can save the tasks or the project.

 
