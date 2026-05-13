---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Configure Card Falloff
description: You can configure a board so that cards are archived, or fall off the board, on a schedule.
author: Courtney
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/iSsqfrcgbod28qez5XkHDP-nDSQO-UKDGm13zPeeBZ0
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
# Configure card falloff

You can configure a board so that cards are archived, or "fall off" the board, on a schedule. You can set cards in a particular column to fall off the board in a certain number of days or weeks.

When a card falls off the board, it is archived. You can display archived cards with a filter. For more information, see [Filter and search in a board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

## Configure card falloff

{{step1-to-boards}}

1. Access a board. For information, see [Create or edit a board](../../agile/get-started-with-boards/create-edit-board.md).
1. Click **[!UICONTROL Configure]** on the right of the board to open the Configure panel.
1. Expand **[!UICONTROL Cards]**.
1. Turn on **[!UICONTROL Automatically archive cards from the board]**.

   ![Card falloff settings](assets/card-falloff-switch.png)

1. Select when to archive cards from the board. You can choose up to 8 weeks or up to 60 days.

   The date is determined from when the card was last modified.

1. Select which column to remove cards from.
1. Click **[!UICONTROL Save]** on the confirmation message.
1. Click **[!UICONTROL Hide configure]** to close the [!UICONTROL Configure] panel. The configuration settings are applied automatically when you refresh the board.
