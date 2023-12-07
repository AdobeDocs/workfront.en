---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Overview of task dependency types
description: Dependency Types refer to the predecessor relationships between tasks. They define when the dependent task can start or finish based on the start or finish of its predecessor.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
---
# Overview of task dependency types

Dependency Types refer to the predecessor relationships between tasks. They define when the dependent task can start or finish based on the start or finish of its predecessor.

>[!IMPORTANT]
>
>Adobe Workfront does not restrict the dependent tasks from starting or finishing based on the dependency types unless the predecessor relationships are enforced. For information about enforcing predecessors, see [Enforce predecessors](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

You must specify the Dependency Type of a predecessor relationship when you establish this relationship between your tasks.

For more information about predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

The following are the Workfront Dependency Types:

* **Finish-Start (fs)**: The predecessor task must finish before the dependent task can start. This is the default dependency type, used when no other dependency type is specified.
* **Finish-Finish (ff)**: The predecessor task must finish before the dependent task can finish.
* **Start-Start (ss)**: The predecessor task must start before the dependent task can start. You cannot start the dependent task unless the predecessor has at least started. 
* **Start-Finish (sf)**: The predecessor task must start before the dependent task can finish. You can start the dependent task before the predecessor starts, but you cannot finish it unless the predecessor started. 
* **Scheduled-Start (sd)**: This schedules a task as Finish-Start, but actual enforcement type is a Finish-Finish. When you use this, the dependent task is scheduled to start after the predecessor task is completed. However, the enforcement makes it so the dependent task can start anytime, but cannot finish until the predecessor task is finished.

>[!NOTE]
>
>The abbreviations for the Dependency Types are used in task lists to define predecessor relationships. For more information, see [Examples of predecessor values in a task list](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [Overview of task predecessors](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

