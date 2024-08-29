---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Use the Card List
description: You can create a card list on a workstream and add the cards to iterations.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
---
# Use the card list

>[!IMPORTANT]
>
>Workstreams are not available for all customers.

You can create a card list on a workstream and add the cards to iterations.

The card list can function as a backlog of work for the workstream.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>New: [!UICONTROL Contributor] or higher</p> 
   <p>or</p>
   <p>Current: [!UICONTROL Request] or higher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add cards to the card list

{{step1-to-boards}}

1. To open a workstream, click [!UICONTROL **View workstream**].
1. Click the [!UICONTROL **Card List**] tab.
1. Click [!UICONTROL **Add card**].
1. In the [!UICONTROL **Create/Edit Card**] dialog, add the following information:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>The name of the card.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>A description of the card.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>The estimated number of hours for the card to be completed. This is a manual entry only.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Select a status for the card.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>Select an iteration to assign the card to.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>To assign the card, start typing a name in the search field, then select it when it displays in the list. You can add both individuals and teams, and you can assign more than one person or team to a card.</p><p>Assignees must be members on the workstream or they will not appear in the selection list.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Click [!UICONTROL **Save**].
1. Continue adding cards until you have built the card list.

## View cards

To view all cards for the workstream in a single list, click [!UICONTROL **List view**] on the Card List tab.

To view all cards for the workstream grouped by iteration, click [!UICONTROL **Iteration view**]. Unplanned cards are displayed in their own group.

To edit an existing card, select it in the list and click [!UICONTROL **Edit**].

To delete a card, select it in the list and click [!UICONTROL **Delete**].

### Filter cards

Cards can only be archived from the iteration board. When a card is archived, it is not displayed in the card list unless you filter to show archived cards. For information about archiving a card, see [Delete or archive a card from a board](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Access the card list for the workstream.
1. Click [!UICONTROL **Filter**] and select [!UICONTROL **All**], [!UICONTROL **Active cards**], or [!UICONTROL **Archived cards**].

   When a filter other than the default is applied on the card list, an indicator is displayed on the filter icon ![Filter applied](assets/boards-filterapplied-30x30.png).

### Search in the card list

1. Access the card list for the workstream.
1. Click [!UICONTROL **Search**] and type a search term. Then, press Enter.

   All cards that contain the search term are displayed.
   Click the X to clear the search.

   ![Search for cards in a board](assets/boards-searchbox.png)

## Add cards to an iteration

>[!NOTE]
>
>You must create an iteration before you can add cards to it. For information, see [Create an iteration in a workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Access the card list for the workstream.
1. Select the [!UICONTROL **Iteration view**] to see which cards are assigned to an iteration and which are unplanned.
1. Select an unplanned card in the list and click [!UICONTROL **Edit**].
1. Select an iteration in the [!UICONTROL **Iterations**] field.
1. If you are using story points, enter a value in the [!UICONTROL **Estimation**] field.
1. Click [!UICONTROL **Save**].

   The card is moved to the iteration, and the iteration metrics reflect the number of cards and points.

   You can also drag and drop a card from the Unplanned cards group into the iteration, or click [!UICONTROL **Add card**] to add a new card to the iteration.

>[!TIP]
>
>If you have created an iteration process board, all unplanned cards on the card list appear in the [!UICONTROL Backlog] column. When a card is moved into another column, it becomes part of the active iteration. Cards that you add to the iteration in the card list are added to a column based on their status.
