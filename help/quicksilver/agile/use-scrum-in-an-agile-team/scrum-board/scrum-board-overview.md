---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Scrum Board Overview
description: The Scrum agile story board displays together with the completion status and the burndown chart.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
---
# [!UICONTROL Scrum] board overview

The [!UICONTROL Scrum] agile story board displays together with the completion status and the burndown chart. These agile components are available in the following situations in [!UICONTROL Adobe Workfront]:

* On agile iterations. For more details about using the agile story board, burndown chart, and completion status in a pure agile environment (with backlogs and an iteration), see [Work in an agile environment](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* When viewing a project in an agile view. For information about how you can leverage the agile story board, burndown chart, and completion status within an existing project, see [Manage a project in the Agile View](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Agile iteration](assets/agile-iteration-with-callouts.png)

## Story Board Layout and Functions

![Agile story board](assets/agile-storyboard-callouts.png)

The story board consists of the following elements:

* **[!UICONTROL Parent Story] Column:** Unlike the other columns on the story board, the  [!UICONTROL Parent Story]  column is not a task status, but rather exists to house any stories that contain subtasks in the iteration or project. Only parent stories that have at least one subtask on the story board can reside in this column. The parent stories themselves do not move from status to status across the story board.

   In an iteration, this column appears on the story board only when one or more stories on the story board contains at least one subtask that meets the following requirements:

    * Assigned to the same agile team as the parent task
    * Belongs to the iteration

      In a project, this column appears any time a task has at least one subtask.

      ![Parent story column](assets/agile-parentstory-swimlane.png)

* **Task Statuses:** Indicate how a story is progressing through the iteration or project based on which status column the story is in.

   Task statuses can be customized for the project by modifying the agile view, as described in [Create or customize an Agile view](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Views overview in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **Swim Lane:** When a parent story and its subtasks appear on the story board, a swim lane is created specifically for the story and its subtasks. This provides a visual distinction to better view how a story's subtasks are progressing across the story board.

   In an iteration, swim lanes appear on the story board only when a story on the story board contains at least one subtask that meets the following requirements:

    * Assigned to the same agile team as the parent task
    * Belongs to the iteration

   In a project, swim lanes appear any time a task has at least one subtask or one parent task.

* **Individual Stories:** Individual stories and issues are displayed below any swim lanes on the story board. This provides a visual distinction from the stories that are part of a swim lane.

## Relationship between Subtasks and Stories

If a story contains subtasks, you cannot update any information on the parent story itself (such as points/hours or percent complete). Furthermore, you cannot move the story across the story board to update its status. Rather, any changes you make to the story's subtasks are reflected on the story. The combined story points or hours for all subtasks determines the points or hours of the parent story.

For example, if a story has only one subtask valued at 4 points, the story itself also has 4 points. If you change the subtask point value to 3, the point value of the parent story is changed to 3. If you create another subtask on the same story and set the point value for that subtask to 4, the point value for the story is changed to 7 in order to reflect the combined point value for both subtasks.

This same logic applies to second-level subtasks (subtasks of subtasks). If a subtask has one or more second-level subtasks, the subtask is calculated based on the second-level subtasks.

## Relationship between the Story Board and the Backlog

>[!NOTE]
>
>The information in this section applies only to agile views on an iteration; agile views on a project do not use a backlog. (For more information about the differences between agile views on an iteration and a project, see "Differences When Using the [!UICONTROL Agile] View on a Project verses on an Iteration" in [Manage a project in the Agile View](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

The iteration backlog shows only stories or subtasks where you can set an estimate. If a parent story has subtasks that are displayed on the story board (because they are assigned to the same agile team and belong to the iteration), the parent task is not displayed on the backlog. In this situation, only the subtasks are displayed on the backlog, while the subtasks and the parent story are displayed on the story board.

For example, suppose that Story A contains Subtask 1 and Subtask 2 (and both subtasks are assigned to the same agile team). In this situation, Story A is displayed on the story board in a swim lane with Subtask 1 and Subtask 2. However, only Subtask 1 and Subtask 2 are displayed in the backlog.

This same logic applies to second-level subtasks (subtasks of subtasks). If a subtask has one or more second-level subtasks assigned to the same agile team and belong to the iteration, only the second-level subtask is displayed in the backlog.

For more information about the backlog, see [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
