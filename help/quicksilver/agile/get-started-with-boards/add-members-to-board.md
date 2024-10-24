---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Add or Remove Members from a Board
description: People must be added to the board as members before they can view the board and be assigned to cards.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
---
# Add or remove members from a board

People and teams must be added to the board as members before they can view the board.

The creator of a board is the owner by default. The board owner is the only person who can delete that board or update its filters in the Configure panel. Only a system administrator or the current board owner can change the board owner.

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

## Add members to a board

{{step1-to-boards}}

1. Create a new board or edit an existing board. For information, see [Create or edit a board](../../agile/get-started-with-boards/create-edit-board.md).
1. Click the **[!UICONTROL Add member]** icon ![Add members](assets/boards-addmember-spectrum-25x25.png).
1. In the **[!UICONTROL Add members]** box, start typing a name, then select it when it displays in the list.

   You can select an individual member or a team. If you choose a team, the team itself is added to the board.

   >[!NOTE]
   >
   >An individual user must have the **[!UICONTROL View]** or **[!UICONTROL Edit]** option set in their access level for teams, or they will not be able to view the board.


   ![Add members to board](assets/boards-add-members.png)

## Remove members from a board

{{step1-to-boards}}

1. Create a new board or edit an existing board. For information, see [Create or edit a board](../../agile/get-started-with-boards/create-edit-board.md).
1. Click the **[!UICONTROL Add member]** icon ![Add members](assets/boards-addmember-spectrum-25x25.png).
1. In the **[!UICONTROL Add members]** box, click the X next to a person or team name to remove them from the board.

   ![Remove member from board](assets/boards-remove-member-from-board-350x367.png)

   When you remove a member from a board, they are not removed from any cards they are assigned to. For connected cards, the assignments are also updated on the [!DNL Workfront] task or issue.

   Members are only removed from this board. They are not removed from other boards they belong to.

   >[!NOTE]
   >
   >You can't remove the board owner.

## Change the board owner

   >[!NOTE]
   >
   >Only a system administrator or the current board owner can change the board owner. A board can only have one owner.

{{step1-to-boards}}

1. Access the board.
1. Click the **[!UICONTROL More]** menu ![More menu](assets/more-icon-spectrum.png) next to the board name, then choose **[!UICONTROL Change board owner]**.
1. In the Change board owner dialog box, search for and select the user you want to make the owner.

   You can't search for users who are already members on the board. To make an existing member the owner, you must first remove them from the board. Making a user the board owner adds them to the board.

   Only a user can be the board owner. A team can't be an owner.

1. Click [!UICONTROL **Update**].
