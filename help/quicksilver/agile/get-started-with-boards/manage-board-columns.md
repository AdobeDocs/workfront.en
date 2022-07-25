---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Manage board columns
description: A new board contains three columns by default. You can add more columns, change the order of the columns, rename columns, and delete any columns that you don't need.
author: Lisa
feature: Agile
---

# Manage board columns

A new board contains three columns by default. You can add more columns, change the order of the columns, rename columns, and delete any columns that you don't need.

Column settings include policies, which allow you to define options for what happens to a card when it is moved into that column.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add a column to a board

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Boards**.
1. Access a board. For information, see [Create or edit a board](../../agile/get-started-with-boards/create-edit-board.md).
1. Click **Add Column** to the right of the existing columns.
1. In the new column, type a name and click **Add Column**.

   ![Add new column](assets/boards-add-column.png)

## Reorder columns on a board

1. Access the board.
1. Drag and drop the columns into the correct order. Be sure to select the top of the column before dragging it to another location.

   ![Drag and drop column](assets/boards-dragdropcolumn.png)

## Rename a board column

1. Access the board.
1. Click on the column name, type the new name, and press Enter.
   
   Or
   
   Click the **More** menu ![More menu](assets/more-icon-spectrum.png) on the column and select **Edit**. In the Settings area, type the new name in the **Column name** field, and click **Close**.

## Delete a board column

1. Access the board.
1. Click the **More** menu ![More menu](assets/more-icon-spectrum.png) on the column, and select **Delete**.

   >[!NOTE]
   >
   >Columns that contain cards, including archived cards, can't be deleted. If you try to delete a column that contains cards, you must choose another column for those cards.

## Define column settings and policies

1. Access the board.
1. Click the **More** menu ![More menu](assets/more-icon-spectrum.png) on the column, and select **Edit**.

   The Settings area appears. The **Column name** lets you know which column you are defining settings for.

1. Enable the **Update field values automatically** policy to change certain field values automatically when a card is moved to this column.

   ![Column settings and policies](assets/boards-column-policies-enabled.png)

1. (Optional) Set a value for the card status:

   1. Select the **Status** check box.

   1. Select the status to apply to a card when it is moved to this column.

      ![Status for columns](assets/boards-column-status.png)

      The status translation options for connected cards are also displayed. (Status translation does not apply to ad hoc cards.) These options determine the status applied to the task or issue in Workfront when a connected card is moved to this column.

   1. To change the default status translation selections, click the **Edit** icon ![Edit icon](assets/edit-icon-spectrum.png).
   1. Select a status for tasks and a status for issues. Only the default Workfront statuses are available, not custom statuses.  

   >[!NOTE]
   >
   >If you do use custom statuses in Workfront, the first time you move a connected card into this column you will be prompted to choose a status. For example, if the connected project has multiple status types that all correspond to Completed, you must choose which status to use in Workfront. You can set your choice as the default so you don't have to make the selection every time you move a card to the column.
   >For more information on statuses, see [Statuses overview](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

1. (Optional) Set a value for the card assignees:

   1. Select the **Assignees** check box.
   1. Select an action.

      * **Add on assignees:** The assignees you select are added to the existing list of assignees on a card when it is moved to this column.
      * **Override assignees:** The assignees you select override all other assignees, and become the only assignees on a card when it is moved to this column.

   1. Select the assignees from the drop-down list. Only members on the board are available to choose from. For more information, see [Add or remove members from a board](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

      ![Assignees for column](assets/boards-column-assignees.png)

1. (Optional) Set a value for the card tags:

   1. Select the **Cards** check box.
   1. Select an action.

      * **Add on tags:** The tags you select are added to the existing list of tags on a card when it is moved to this column.
      * **Override tags:** The tags you select override all other tags, and become the only tags on a card when it is moved to this column.

   1. Select the tags from the drop-down list. Only tags already created in the Tag Manager are available to choose from. For information on adding new tags, see [Add tags](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tags for column](assets/boards-column-tags.png)

   >[!NOTE]
   >The WIP limit policy in the column settings is available only via the early feature opt-in. For details, see [Early feature opt-in for Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).
   >
   >1. Enable the **Work in progress limit** policy to limit the number of cards that can be added to the column.
   >1. Type the limit number in the **Set limit** field.
   >
   >The number of cards and the limit display at the top of the column. If the column contains more cards than the limit, the counter turns red. Note that the WIP limit is simply a visual warning and does not restrict you from having more items in each column than the limit you set.
   >
   >![WIP limit counter](assets/boards-wip-limit-counter.png)

1. Click **Close** to exit the Settings area and view the column and its cards.
