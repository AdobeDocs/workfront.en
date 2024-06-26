---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Manage a project in the Agile View
description: You can leverage agile functionality for your project without the administrative challenges that typically accompany agile practices (such as managing a team backlog or creating iterations).
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
---
# Manage a project in the Agile View

<!-- Audited: 2/2024 -->

You can leverage agile functionality for your project without the administrative challenges that typically accompany agile practices (such as managing a team backlog or creating iterations).

If you want to work in an agile environment that uses a team backlog and allows you to create iterations from tasks on the backlog, follow the instructions in [Work in an agile environment](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Current: Review or higher</p> 
   <p>New: Contributor or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to the following areas:</p> 
    <ul> 
     <li> <p>Projects</p> </li> 
     <li> <p>Reports, Dashboards, Calendars</p> </li> 
     <li> <p>Filters, Views,&nbsp;Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Understand Agile projects

>[!NOTE]
>
>This section only applies to the legacy Agile view, not to the board view of a project.

* [Agile functionality in a project](#agile-functionality-in-a-project) 
* [Differences when using the Agile view on a project versus on an iteration](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Agile functionality in a project {#agile-functionality-in-a-project}

The following agile functionality is available when managing a project in an agile view:

* Completion Status  
  For more detailed information about completion status, see [Iteration completion status overview](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Story board  
  For more detailed information about the story board, see the [Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) section.

There are some differences when using agile views on a project versus working in a pure agile environment (with backlogs and iterations). For more information, see [Differences when using the Agile view on a project versus on an iteration](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) in this article.

### Differences when using the Agile view on a project versus on an iteration {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Tasks and subtasks follow different display rules in a project Agile view and on the story board of an iteration](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board) 
* [Backlogs and iterations are not used in the Agile view](#backlogs-and-iterations-are-not-used) 
* [Task order is maintained in the Agile view and cannot be reordered](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered) 
* [Tasks are measured only in Planned Hours on a project list](#tasks-are-measured-only-in-planned-hours) 
* [The Agile Team is not used in an Agile view](#the-agile-team-is-not-used) 
* [Each user on the project can view the project in a different Agile view](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Tasks and subtasks follow different display rules in a project Agile view and on the story board of an iteration {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Tasks that have neither a parent task nor a subtask are always displayed as a single story card on the story board of the Agile view.   
  For example, these tasks appear as follows in the project list view: 
  
  ![Agile project list - tasks with no parent or subtasks](assets/agile-project-single-list-nwe.png) 
  
  These tasks appear as follows in the project agile view:
  
  ![Project agile view - tasks with no parent or subtasks](assets/agile-project-singlecard-nwe.png)

* Parent tasks that have subtasks are always displayed in the **Stories** column of the story board of the Agile view. Subtasks are displayed in the swimlane of the parent task.   
  For example, these tasks appear as follows in the project list view:   
  
  ![Agile project list - tasks with parents and subtasks](assets/agile-project-parent-list-nwe.png)  
  These tasks appear as follows in the project agile view:   
  
  ![Agile project view - tasks with parents and subtasks](assets/agile-project-parent-nwe.png)

* Second-level subtasks (subtasks of subtasks) are displayed as a hanging gray card off the immediate parent task.
* Third-level subtasks (subtasks of subtasks of subtasks) are never displayed on the Agile view.

#### Backlogs and iterations are not used in the Agile view {#backlogs-and-iterations-are-not-used}

When viewing a project in an agile view, the following agile components are not used:

* **Backlog:** No backlog is used because any tasks in the project are automatically displayed as stories.
* **Iterations:** Rather than creating iterations to define the dates when work will be accomplished, the days currently designated on the project timeline become the working days.

#### Task order is maintained in the Agile view and cannot be reordered {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

The order in which tasks appear in a project is maintained when you view the project in an agile story board.

You cannot reorder tasks in the project when viewing the project in an agile view. Because modifying the task order can affect other tasks that might have dependencies, you must view the project in a standard view in order to modify task order.

#### Tasks are measured only in Planned Hours on a project list {#tasks-are-measured-only-in-planned-hours}

Tasks on a project are always measured in Planned Hours.

In an iteration, tasks (stories) can be measured in hours or points.

#### The Agile Team is not used in an Agile view {#the-agile-team-is-not-used}

Because agile teams complete the work on iterations that are assigned to them, agile teams are not used when viewing a project in an agile view.

Instead, any users on the project essentially become the agile team for that project.

#### Each user on the project can view the project in a different Agile view {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Unlike an agile iteration, users on a project can customize the agile view for themselves, while other users use a different agile view.

In an agile iteration, the information that is available on the agile story board (such as status columns that are available) is determined on the team level.

For information about how to customize an agile view, see [Create or customize an Agile view](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Create or edit views in in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## View a project in the Agile view

1. Go to the project you want to view in an agile view, on either the task list or the issue list.
1. Click the **Board view** icon ![Board icon](assets/board-icon-for-agile-view.png).

   The board view of the project displays by default.

   ![Board view of project](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Optional) Click **Configure** to set options for the columns and cards.

   For more information, see [Manage board columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) and [Customize which fields are displayed on a card](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Note that you can't define column policies on the board view of a project.

1. (Optional) Click **Use legacy agile** to use the legacy agile view instead of the board view.

1. (Optional – legacy agile view only) If you have created a custom agile view, or if another user has created a custom agile view and shared it with you, you can view it instead of the default agile view.

   Click the **View** drop-down menu, then click the custom agile view you want to view.  
  
   The custom agile view is used the next time you click the **Agile** icon.

   For information about how to create a new agile view, see [Create and customize Agile views](#create-and-customize-agile-views), below.

   The project is displayed in the custom agile view.

1. (Conditional – legacy agile view only) If tasks in your project are using statuses other than "New," "In Progress," or "Complete" (the default statuses for the Agile view), you must add the additional statuses to the agile view for any tasks in those statuses to be displayed.

   If tasks are in a status that is not displayed on the agile story board, the task itself is not displayed on the agile story board (however, the Percent Complete of these tasks still contribute to the Percent Complete of any parent tasks and the Percent Complete of the overall project).

   To add statuses to the agile view, either create a new agile view or customize an existing agile view, as described in [Create and customize Agile views](#create-and-customize-agile-views), below.

1. (Optional) To return to the list view, click the **List** icon.

## Create and customize Agile views {#create-and-customize-agile-views}

>[!NOTE]
>
>This section only applies to the legacy Agile view, not to the board view of a project.

As with standard views in Workfront, you can customize existing agile Views or create new agile views from scratch. Unlike standard views, you cannot create new agile Views based on existing agile views.

For more information about creating and customizing agile views, see the [Create or customize an Agile view](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) section in the article [Create or edit views in in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Share an existing Agile view

>[!NOTE]
>
>This section only applies to the legacy Agile view, not to the board view of a project.

You can share an Agile view you created or have permissions to in the same way you share any other view, or filter or grouping. 

For more information, see [Share a filter, view, or grouping](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Remove an existing Agile view

>[!NOTE]
>
>This section only applies to the legacy Agile view, not to the board view of a project.

You can remove an Agile view in the same way you remove any other view, or filter or grouping. 

For more information, see the [Remove filters, views, and groupings](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md). 
