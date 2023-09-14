---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Task Handoff Date overview
description: The Handoff Date is the date that a task becomes available for work. This typically means that its predecessors have resolved and the assignee of the task can start working on it.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
---
# Task Handoff Date overview

The Handoff Date is the date that a task becomes available for work. This typically means that its predecessors have resolved and the assignee of the task can start working on it.

>[!TIP]
>
>Handoff Dates do not exist for issues and projects.

## How Adobe Workfront calculates the Handoff Date

>[!NOTE]
>
>The Handoff Date is calculated only if the project status equates to the following statuses:
>
>* On Hold
>* Current
>* Complete
>* Dead
>

Workfront uses the following rules for calculating the Handoff Date of a task:

* **When the task has an incomplete predecessor**: The Handoff Date for the task is null. 
* **When the task has a complete predecessor**: The Handoff Date is the same as the Actual Completion Date of the predecessor task. If the predecessor has a lag, Workfront calculates the Handoff Date of the successor task using the following formula:

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   For information about lag time, see [Overview of Lag Types](../use-prdcssrs/lag-types.md). 

   If the successor task has more than one predecessor, the Handoff Date is calculated based on the latest Actual Completion Date of the predecessors. For example, if the two predecessors' Actual Completion Dates are November 8, 2022 and November 20, 2022, the Handoff Date of the successor is November 20, 2022.

   >[!NOTE]
   >
   >   Calculating the Handoff Date of a successor task based on the Actual Completion Date or a predecessor task is the same whether the predecessor is enforced or not. For more information about enforced predecessors, see [Enforce predecessors](../use-prdcssrs/enforced-predecessors.md).

   
* **When the task has no predecessor and**:

   * **The Planned Start Date is in the past**: The Handoff Date is the same as the Planned Start Date of the project if the task has no forced constraint set. For the cases where tasks have forced constraints, see the "When the task has a forced constraint for the Planned Dates" section below. 
   * **The Planned Start Date is in the future (any date after the current date)**:  The Handoff Date is the same as the Planned Start Date of the task if the task has no forced constraint set. For the cases where tasks have forced constraints, see the "When the task has a forced constraint for the Planned Dates" section below.

>[!NOTE]
>
>When the task has a cross-project predecessor, the handoff date of the successor recalculates only when either of the following occur:
>
>* You manually recalculate the timeline of the successor's project. You must have Manage permissions to the project to recalculate timeline. 
>* The timeline of the successor's project is automatically recalculated at night. 
>
>For information about recalculating the project's timeline, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **When the task has a forced constraint for the Planned Dates**: The Handoff Date varies depending on the type of constraint and whether the task has an Actual Start Date or not.   
  The following are forced constraints on tasks:

   * Must Start On
   * Must Finish On
   * Start No Earlier Than
   * Start No Later Than
   * Fixed Date

  The following scenarios exist: 

   * **When the task has a constraint of Must Start On or Start No Earlier Than**: If the task constraint date is in the past and there is no Actual Start Date on the task (the task hasn't started yet) the Handoff Date is the closest possible date the task can be started to be worked on. If the task has started, the Handoff Date equals the start date of the project.
   * **When the task has a constraint of Must Finish On or Start No Later Than**: If the task constraint date is in the future and there is no Actual Start Date on the task (the task hasn't started yet) the Handoff Date is the task's Planned Start Date. If there is as Actual Start Date on the task then the Handoff Date is the project's start date.
   * **When the task has a constraint of Fixed Dates**: The Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Locate the Handoff Date

You can display the Handoff Date of a task in a task report or the view of a task list.  
For more information about building a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
