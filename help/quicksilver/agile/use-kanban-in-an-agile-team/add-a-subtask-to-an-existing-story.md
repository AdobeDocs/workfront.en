---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Add a Subtask to an Existing Story on the Kanban Board
description: Review this article to learn how to create subtasks for existing stories on the Kanban board.
author: Courtney
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Wbiao1UjwOzItIGJkh1E9A81RcUfLDJqgYjRDL46qvQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
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

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> 
   <p>Work or higher</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>Contribute or Manage access to the task the subtask is on</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add a subtask to an existing story on the [!UICONTROL Kanban] board

1. Go to the [!UICONTROL Kanban] board that contains the story where you want to add a subtask.
1. Click the name of the task on the story tile on the [!UICONTROL Kanban] board.
1. Add a subtask to the task as you would in any other task list within [!DNL Workfront], as described in [Create subtasks](../../manage-work/tasks/create-tasks/create-subtasks.md).
