---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Manage workstreams
description: A workstream is a configurable group of boards  and cards for collaborating on work.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
---
# Manage workstreams

>[!IMPORTANT]
>
>Workstreams are only available to a specific group of customers.

A workstream is a configurable group of boards and cards for collaborating on work. Workstreams can include different types of boards created from templates and a card list of work items. In a workstream, you can track work in iterations or sprints.

For more information, see [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) and [Create an iteration in a workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Workstreams appear on the dashboard along with individual boards you have access to that are not part of a workstream. For information about the boards dashboard, see [Use the boards dashboard](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). You can click any board name on the dashboard to open it.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Create a workstream

{{step1-to-boards}}

1. Click **[!UICONTROL Add workstream]** in the [!UICONTROL Workstreams] area of the dashboard.
1. Type a name to replace **[!UICONTROL Untitled Workstream]** and press Enter.

   You can add boards to the workstream or click [!UICONTROL **All Boards**] to return to the dashboard.

## Create a new board in a workstream

1. If you are not already in a workstream, click [!UICONTROL **View workstream**] on the dashboard to open an existing workstream.
1. Click **[!UICONTROL Add board]** on the [!UICONTROL Boards] tab of the workstream.
1. Select a template for the board.

| Template | Description |
|---------|----------|
| Basic board | Three default columns are provided on the board. You can add new columns and rename or delete the default columns. <p>No column policies are applied. |
| Kanban board | The following columns are provided on the board: Backlog, New, In Progress, Complete, and On Hold. You can add new columns and rename or delete the default columns.<p>To use the backlog, you must set up filters for the intake column. For information, see [Add an intake column to a board](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>To review the default policies for each column, click the [!UICONTROL **More** menu] on a column and select [!UICONTROL **Edit**]. You can change any of these pre-set policies. For information, see [Manage board columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Retrospective board | The following columns are provided on the board: What went well? What could be improved? Who should we celebrate? What can we do to move faster? You can add new columns and rename or delete the default columns. <p>No column policies are applied. |
| Iteration process | This is the board used to define and run an iteration. <p>The following columns are provided on the board: Backlog, New, In Progress, Complete, and On Hold. You cannot add any columns to the board. <p>To review the default policies for each column, click the [!UICONTROL **More**] menu on a column and select [!UICONTROL **Edit**]. You can change any of these pre-set policies. For information, see [Manage board columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

For more information on setting up the board, see [Create or edit a board](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filter the list of boards on a workstream

When filters other than the defaults are applied on the board list, an indicator is displayed on the filter icon ![Filter applied](assets/boards-filterapplied-30x30.png). Click [!UICONTROL **Clear All**] to remove all filters, and click [!UICONTROL **Hide filters**] to close the filter panel.

{{step1-to-boards}}

1. On the dashboard, click [!UICONTROL **View workstream**] to open a workstream.
1. Click the [!UICONTROL **Boards**] tab if it is not already displayed.
1. Click [!UICONTROL **Filter**].
1. Select the boards you want to see by status (archived boards, active boards, or all boards).
1. Select the boards you want to see by template.

## Add members to a workstream

People and teams must be added to the workstream as members before they can view the workstream and its contents. A workstream member can add and remove members on the workstream and see which boards are in the workstream.

>[!NOTE]
>
>A workstream member can't open a board on a workstream until they are added to that specific board as a member.

{{step1-to-boards}}

1. On the dashboard, click [!UICONTROL **View workstream**] to open a workstream.
1. Click the **[!UICONTROL Add member]** icon ![Add members](assets/boards-addmember-spectrum-25x25.png) to add members and teams to the workstream.
   
   This is the same process as adding members to a board. For more information, see [Add or remove members from a board](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Add sources to a workstream

A source determines where the cards in the workstream come from.

{{step1-to-boards}}

1. Click the [!UICONTROL **Sources**] icon ![Sources icon](assets/sources-icon.png) to define a source to import cards into the workstream. At this time, the only available source is [!DNL Adobe Workfront].
1. Add filters to import tasks and issues from Workfront as cards.

   Adding filters for workstream sources is the same as adding advanced filters for an intake column on a basic board or Kanban board. For more information, see [Add an intake column to a board](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Configure a workstream

{{step1-to-boards}}

1. On the dashboard, click [!UICONTROL **View workstream**] to open a workstream.
1. Click [!UICONTROL **Configure**] to open the [!UICONTROL Configure Workstream] panel.
1. (Optional) Expand [!UICONTROL **Workstream**] and type a description of the workstream. This description displays on the dashboard.
1. (Optional) Expand [!UICONTROL **Iterations**] to define an iteration process for this workstream.

   The total number of cards, number of cards pointed, and number of iterations are displayed in the Card List section. Click [!UICONTROL **View list**] to open the list and add cards. For more information, see [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   If an iteration has already been defined, its start date, number of cards, and number of points are displayed. Click [!UICONTROL **View board**] to open the iteration board. For more information, see [Create an iteration in a workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Optional) Expand [!UICONTROL **Tags**] to add tags to the workstream. Search for a tag, or type a new tag name in the search box and press Enter to create it.
