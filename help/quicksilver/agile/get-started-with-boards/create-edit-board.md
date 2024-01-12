---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Create or edit a board
description: From the [!UICONTROL boards] dashboard, you can create a new board or edit an existing board.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
---
# Create or edit a board

<!-- Audited: 12/2023 -->

From the [!UICONTROL boards] dashboard, you can create a new board or edit an existing board.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Contributor or higher </p>
 <p>or</p> 
<p>Current: [!UICONTROL Request] or higher </p> 
</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Create a new board

{{step1-to-boards}}

1. Click **[!UICONTROL Add board]**.

1. Select a template for the board.

   | Template | Description |
   |---------|----------|
   | Basic board | Three default columns are provided on the board. You can add new columns and rename or delete the default columns. <p>Three default columns are provided on the board. You can add new columns and rename or delete the default columns. |
   | Kanban board | The following columns are provided on the board: Backlog, New, In Progress, Complete, and On Hold. You can add new columns and rename or delete the default columns.<p>To use the backlog, you must set up filters for the intake column. For information, see [Add an intake column to a board](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>To review the default policies for each column, click the [!UICONTROL **More** menu] on a column and select [!UICONTROL **Edit**]. You can change any of these pre-set policies. For information, see [Manage board columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospective board | The following columns are provided on the board: What went well? What could be improved? Who should we celebrate? What can we do to move faster? You can add new columns and rename or delete the default columns. <p>No column policies are applied. |
   | Dynamic board | The following columns are provided on the board: Unselected, New, In Progress, On Hold, and Complete. You can add new columns and rename or delete the default columns. (The Unselected column can be renamed but not deleted. This column holds all cards with a status that doesn't match any of the other column statuses.) <p>The default column policies assign cards to columns based on their status. For information, see [Manage board columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. For a dynamic board only, follow the setup wizard steps:

   1. Search for and select [!DNL Workfront] [!UICONTROL **Projects**] to bring tasks and issues onto the board.
   1. Search for and select [!UICONTROL **Assignments**] to bring tasks and issues onto the board.

      All objects appear on the board as connected cards.

      The [!UICONTROL **Cards being added**] counter shows how many cards will be on the board. For example, if you select a project with 100 tasks and issues, the counter shows 100. If you add a user assignment and that person is assigned to 5 tasks on the project, the counter shows 5.

   1. (Optional) Select [!UICONTROL **Include completed work as archived cards**] to bring completed tasks and issues onto the board as archived cards.
   
      >[!NOTE]
      >
      >By default, archived cards are not displayed on the board. To display archived cards, you must turn on a configuration setting and then filter the board to show archived cards. For details, see [Customize which fields are displayed on a card](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) and [Filter and search in a board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).
      >
      >If this option is not selected, completed cards at the time of board creation do not appear on the board. Cards later marked as complete remain on the board in the Complete column and are not archived unless you set up card falloff. For more information, see [Configure card falloff](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

   1. (Optional) Click [!UICONTROL **Use advanced filters**] to display additional filter options.

      This is the same process as creating a filter on an intake column. For more information, see [Add an intake column to a board](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. After adding the filters, click [!UICONTROL **Create board**].

1. Type a name for the board in the **[!UICONTROL Board]** field and press Enter.
1. Configure the board as needed.

   For information, see [Add or remove members from a board](../../agile/get-started-with-boards/add-members-to-board.md), [Manage board columns](../../agile/get-started-with-boards/manage-board-columns.md), [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md), and [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Click **[!UICONTROL All Boards]** to return to the boards dashboard.

   You can also locate the drop-down menu labeled with the name of the current board, and click it to switch to another board.

   ![List of boards](assets/boards-button-list-of-boards-350x188.png)

## Edit an existing board

{{step1-to-boards}}

1. On the dashboard, select the board to open.
1. Edit the board as needed. You can click on the board name to rename it.

   For information, see [Add or remove members from a board](../../agile/get-started-with-boards/add-members-to-board.md), [Manage board columns](../../agile/get-started-with-boards/manage-board-columns.md), and [Add a card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

1. Click **[!UICONTROL All Boards]** to return to the boards dashboard.

   You can also locate the drop-down menu labeled with the name of the current board, and click it to switch to another board.
