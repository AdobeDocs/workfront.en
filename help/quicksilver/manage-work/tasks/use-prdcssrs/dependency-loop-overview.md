---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Task Dependency Loop Overview
description: When adding predecessor relationships to tasks you might encounter dependency loops. For information about predecessors, see Overview of task predecessors.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
---
# Task&nbsp;dependency loop overview

When adding predecessor relationships to tasks you might encounter dependency loops. For information about predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Dependency loop overview

Dependency loops happen when you have two or more tasks that depend on each other to be completed.&nbsp;Adobe Workfront does not allow you to create a predecessor relationship between tasks if it creates a dependency loop.

**Example:** Task 2 is a predecessor to Task 1, which means you must complete Task 2 before you can start working on Task 1.

If you try to make Task 1 a predecessor to Task 2, you get a dependency loop error because you cannot start Task 1 until Task 2 has been completed, but task 2 cannot be started until Task 1 is finished.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considerations about dependency loops

* Dependency loops can involve more than two tasks. Sometimes any number of parents of the tasks you are connecting with a predecessor relationship are the ones creating the dependency loop. 
* A dependency loop can also happen if you try to make a parent the predecessor of a child. 
* In the case of a dependency loop you cannot save the tasks or the project. In order to fix the dependency loop, you must reevaluate&nbsp;the predecessor relationship between the tasks listed in the error message and remove the conflicts before you can save the tasks or the project.

&nbsp;
