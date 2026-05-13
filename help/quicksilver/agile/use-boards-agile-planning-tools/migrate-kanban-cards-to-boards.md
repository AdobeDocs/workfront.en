---
content-type: reference
navigation-topic: boards
title: Migrate Agile Team Kanban Cards to Workfront Boards
description: You can migrate your work items from an Agile team Kanban board to a new or existing Workfront board.
author: Courtney
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/RXk7PYF6JsdF71pRVwEA-Wk23h-UqbgLPXSyNR7VX5Y
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
# Migrate Agile team Kanban cards to Workfront boards

You can migrate your work items from an Agile team Kanban board to a new or existing Workfront board. When you run the migration, all of the cards on the Kanban board are copied to the Workfront board. You are not permitted to choose specific cards.

The placement of cards on the Workfront board is based on column policies. (For example, a policy could move all cards with a status of "In Progress" to a specific column. For more information on column policies, see [Manage board columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) If there are no policies or the cards don't match the policies, the cards are placed in the leftmost column on the board. At this time, cards in the Backlog column on the legacy board are not added to the Workfront board.

The cards are not removed from the Agile team Kanban board, and card status changes will sync to both boards. You can keep both boards active until you are ready to switch to Workfront Boards.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or higher</p> 
   <p>Request or higher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Migrate Kanban cards to a new board

{{step1-to-team}}

1. Access a Kanban board.
1. Click [!UICONTROL **Add to Boards**] and select [!UICONTROL **New Board**].
1. On the [!UICONTROL Add to new board] dialog, type a name for the new board (the name of the current [!UICONTROL Kanban] board is automatically displayed) and click [!UICONTROL **Add**].

   ![Add Kanban cards to new board](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Optional) On the success message that appears, click the link to open the new board.

## Migrate Kanban cards to an existing board

{{step1-to-team}}

1. Access a Kanban board.
1. Click [!UICONTROL **Add to Boards**] and select [!UICONTROL **Existing Board**].
1. On the [!UICONTROL Add to existing board] dialog, search for and select the board to migrate the cards to. Then, click [!UICONTROL **Add**].

   ![Add Kanban cards to existing board](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Optional) On the success message that appears, click the link to open the board.
