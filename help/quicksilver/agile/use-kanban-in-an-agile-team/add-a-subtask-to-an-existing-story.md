---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Add a Subtask to an Existing Story on the Kanban Board
description: Review this article to learn how to create subtasks for existing stories on the Kanban board.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
---
# Add a subtask to an existing story on the Kanban board

When creating subtasks for existing stories, keep in mind the following:

**When the [!UICONTROL Summary Completion Mode] setting for the project is set to [!UICONTROL Manual]:**

* You can move a parent story with subtasks to [!UICONTROL Complete], which updates the parent story to 100% and the [!UICONTROL Status] to [!UICONTROL Complete]. Subtasks are not updated.
* To update the [!UICONTROL Percent Complete] for the story, you must update it from the [!UICONTROL Stories] tab or from the [!UICONTROL Details] page of the object.

**When the [!UICONTROL Summary Completion Mode] setting for the project is set to [!UICONTROL Automatic]:**

* You can't move the parent story across the board. To update the [!UICONTROL Percent Complete] for the story, you must update the [!UICONTROL Percent Complete] for any subtasks. The [!UICONTROL Percent Complete] for the story is calculated based on the [!UICONTROL Percent Complete] of all subtasks.
* Moving a parent story with subtasks to [!UICONTROL Complete] updates the parent story to 100% and the [!UICONTROL Status] to [!UICONTROL Complete]. Subtasks are also updated to 100% and the [!UICONTROL Status] is updated to [!UICONTROL Complete].

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p> 
   or
   <p>Current: [!UICONTROL Work] or higher</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>[!UICONTROL Contribute] or [!UICONTROL Manage] access to the task the subtask is on</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add a subtask to an existing story on the [!UICONTROL Kanban] board

1. Go to the [!UICONTROL Kanban] board that contains the story where you want to add a subtask.
1. Click the name of the task on the story tile on the [!UICONTROL Kanban] board.
1. Add a subtask to the task as you would in any other task list within [!DNL Workfront], as described in [Create subtasks](../../manage-work/tasks/create-tasks/create-subtasks.md).
