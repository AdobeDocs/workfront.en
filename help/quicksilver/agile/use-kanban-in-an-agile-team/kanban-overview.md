---
filename: kanban-overview
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban overview
description: The following sections enable you to better understand how the Kanban board functions:
---

# Kanban overview

The following sections enable you to better understand how the Kanban board functions:

## Kanban board layout and functions

The Kanban board consists of the following elements:

**Backlog Column**: Displays all tasks that are currently on the backlog. This column is not displayed by default. For more information about the backlog, including how to display it on the Kanban board, see [Manage the agile backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Story Statuses**: Indicates how a story is progressing based on which status column the story is in.

For more information, see [Update the status of stories on the Kanban board](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Story statuses can be customized for the project by modifying the agile view, as described in the section [Create or customize an Agile view](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Views overview in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>A maximum of fifty cards is displayed on the Kanban board by default, but you can click **Show More** to display additional cards.

## Relationship between subtasks and stories

If a story contains subtasks, you cannot update any information on the parent story itself (such as points/hours or percent complete). Furthermore, you cannot move the story across the Kanban board to update its status. Rather, any changes you make to the story's subtasks are reflected on the story. The combined story points or hours for all subtasks determines the points or hours of the parent story.

For example, if a story has only one subtask valued at 4 points, the story itself also has 4 points. If you change the subtask point value to 3, the point value of the parent story is changed to 3. If you create another subtask on the same story and set the point value for that subtask to 4, the point value for the story is changed to 7 in order to reflect the combined point value for both subtasks.

This same logic applies to second-level subtasks (subtasks of subtasks). If a subtask has one or more second-level subtasks, the subtask is calculated based on the second-level subtasks.

## Supported features

You can do the following actions when using the Kanban board:

* [Add a subtask to an existing story on the Kanban board](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md) 
* [Add existing tasks or issues to the Kanban board](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md) 
* [Assign users to a story on the Kanban board](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md) 
* [Add stories and issues from the Kanban board](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md) 
* [Delete stories or issues from the Kanban board](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md) 
* [Edit story information](../../agile/use-kanban-in-an-agile-team/edit-story-information.md) 
* [Filter by user on the Kanban board](../../agile/use-kanban-in-an-agile-team/filter-by-user.md) 
* [Manage the work in progress (WIP) limit on the Kanban board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md) 
* [Reorder stories on the Kanban board](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md) 
* [Update the status of stories on the Kanban board](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md) 
* [Use flags on stories on the Kanban board](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md) 
* [Add the backlog to the Kanban board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)

