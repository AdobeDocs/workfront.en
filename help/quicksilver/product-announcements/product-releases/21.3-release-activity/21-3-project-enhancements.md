---
title: 21.3 Project enhancements
description: 21.3 Project enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
---
# 21.3 Project enhancements

This page describes all Project enhancements made with the 21.3 release to the Preview environment. These enhancements were made available in the Production environment the week of July 21, 2021.

For a list of all changes available with the 21.3 release, see [21.3 Release overview](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Associate a template with a group

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

To help you streamline the project creation process —and to help you more easily identify and report on which groups own which project templates—we've added the ability to assign a group to a project template.

When you assign a group to a project template, all projects created from the template are automatically associated with the template's group. For more information, see [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Also, you can attach a group approval process to a template and its template tasks if the template is associated with your group. For more information, see [Associate a new or existing approval process with work](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Easier editing of fields in the Details section

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

The following improvements allow you to more easily edit information in the Details section of any object:

* A gray outline around a field when hovering over it indicates that it is editable.
* You can edit fields by clicking them once.

Prior to this enhancement it was not clear which fields were editable and you had to double-click to edit a field.

## Consider cross-project predecessors when calculating handoff dates

With a new improvement in the way Adobe Workfront calculates handoff dates for tasks, the cross-project dependencies are now taken into account.

Previously, the handoff dates were calculated based only on the predecessors of the task from the same project.

Now, to ensure you always have an accurate handoff date for a task with a cross-project predecessor, you must recalculate the timeline of the successor task's project. After recalculating the timeline, the handoff dates of the task calculates taking into account the cross-project dependencies of the tasks.

For more information about handoff dates, see [Task Handoff Date overview](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Add existing stories and issues from the Scrum board

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

You can now add an existing story or issue directly from the Scrum board. This makes it easier to add existing stories to your current iteration without having to go to the backlog page.

For more information, see [Add stories and issues from the Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Add new stories and issues from the Scrum board

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

You can now create a new story or issue directly from the Scrum board. This makes it easier to quickly add a new story to your current iteration.

For more information, see [Add stories and issues from the Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Delete story or issue from the Kanban board

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

You can now delete a story or issue directly from your Kanban board by clicking the More icon on a story or issue card and selecting Delete. When you delete a story or issue, it is moved to the Recycle Bin for 30 days and can be recovered only by the system administrator.

For more information, see [Delete stories or issues from the Kanban board](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Agile card header and story board updates

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

On Kanban and Scrum boards, the following enhancements are now available:

* The story cards and board columns have a fixed width, so that the card sizes will not change if you adjust the browser window size.
* The Stories column has been renamed to Parent Story.
* Each card has a label at the top to identify it as a parent story, subtask (associated with a parent story), story (not associated with a parent), or issue.
* Background shading visually separates the columns.

For more information, see [Iterations overview](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Group project, task, and issue preferences

As we communicated earlier, we rolled out group-level customizations for project, task, and issue preferences in phases leading up to June 24, 2021. Now the rollout is complete and they are available in Production for all customers.

For more information, see the following articles:

* [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 
* [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Allow external users to approve a document

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

You can now use external email addresses to assign approvers to a document in the new Workfront experience.

Previously, you could add external users by email address only in Workfront Classic.

For more information, see [Request document approvals](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Export information from the Details section of a portfolio or program

>[!NOTE]
>
>This feature was released to the Preview environment on May 20, 2021. It will release to the Production environment on June 3, 2021.

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

You can now export to a .pdf file information from the Details section of portfolios and programs. Prior to this enhancement, you could export information from the Details section only from projects, tasks and issues.

For information about exporting custom forms from an object, see [Export custom forms and object details](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Added Planned Completion Date timestamp in the object's header

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

To facilitate easy access, convenience as well as accuracy, we have added the option to select a timestamp in the Planned Completion Date of the header of projects, tasks, or issues.

Prior to this enhancement, when you updated the Planned Completion Date of an object, Workfront selected midnight as the default time. Now, you can customize the time as well as the completion date.

For information about the object headers in the new Workfront experience, see [New object headers](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Add a custom form to an object without editing it

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

We have made it easier to add a custom form that someone else will fill out—or that you will fill out later—to an object. The form no longer goes into editing mode automatically when you add it. You can simply save the empty form to the object.

Previously, when you added a custom form to an object, the page went into editing mode and you had to complete any required fields on the form before you could save it to the object. This was inconvenient when the form was meant for another user to fill out, or when you did not know yet what to put in a required field on the form.

For information about adding a custom form to an object, see [Add a custom form to an object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

