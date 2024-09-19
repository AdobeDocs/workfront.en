---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Team Requests Overview
description: Team requests are found in the Teams area in the Main Menu.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
---
# Team requests overview

## Understand team requests

Team requests are found in the [!UICONTROL Teams] area in the [!UICONTROL Main Menu]. Click on the [!UICONTROL Team Requests] icon ![Request icon](assets/request-icon.png) in the left panel to view team requests.

>[!NOTE]
>
>Agile teams do not have team requests.

The [!UICONTROL Team Requests] tab shows the requests awaiting assignment for the team that is currently selected in the drop-down list. The number in parentheses indicates how many items are ready to be worked on.

A team request represents a pending work item that is not assigned to a specific user. Instead, it is assigned to a team, and any member of that team can volunteer to accept responsibility for the item. If a user volunteers to work on a team request, the user is accepting the work assignment as their own. The task is assigned to the individual user in addition to the team.

>[!NOTE]
>
>A team request should not be used for collaborative task assignments. If you need to assign multiple users to work together on a task, do this through [!UICONTROL Advanced Assignments] and not through Team requests. For more information, see [Create advanced assignments](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Understand the [!UICONTROL Ready to Start] and [!UICONTROL All] options

There are two options at the top of the Team Requests section: [!UICONTROL Ready to Start] and [!UICONTROL All].

The [!UICONTROL Ready to Start] option shows only tasks and issues that meet all of the following criteria:

* All predecessors have met the conditions for their predecessor dependency types.  
  For example, if the type of predecessor relationship is [!UICONTROL Finish-Start] (predecessor task must finish before the dependent task can start), the predecessor must be marked as [!UICONTROL Complete]. (For more information about predecessor dependency types, see [Overview of task dependency types](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* The logged-in user is the person assigned to these tasks and issues (for work requests), or the selected team is assigned to these tasks and issues (for team requests).
* The project status is in a status of [!UICONTROL Current].
* The [!UICONTROL Projected Start Date] or [!UICONTROL Planned Start Date] has passed or is scheduled to begin within two weeks from today's date (or no [!UICONTROL Projected Start Date] or [!UICONTROL Planned Start Date] has been defined).
* The [!UICONTROL Handoff Date] has already occurred or will occur within two weeks from the current date.

>[!NOTE]
>
>If the task meets the first three criteria and has a Handoff date within two weeks of the current date, it will show as [!UICONTROL Ready to Start] even if the Planned/Projected dates are further out than two weeks. If the task doesn't have a Handoff date, then the Planned/Projected dates must be within two weeks of the current date.

The [!UICONTROL All] option shows all tasks and issues on current projects that are assigned to the logged-in user or all tasks or issues assigned to the team.
