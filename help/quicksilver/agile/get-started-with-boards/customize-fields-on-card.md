---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Customize which fields are displayed on a card
description: You can customize which fields are displayed on a card by disabling a field so it is not displayed in the full card or condensed view, or hiding a field on the condensed card view.
author: Lisa
feature: Agile
---

# Customize which fields are displayed on a card

>[!NOTE]
>
>This feature is available only through the early feature opt-in for [!DNL Workfront] [!UICONTROL Boards]. For details, see [Early feature opt-in for Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

By default, all available fields are displayed on a card, both in the the full view when the card is open, and in the condensed card view on the board. You can customize which fields are displayed by:

* Disabling a field so it is not displayed in either view
* Hiding a field on the condensed card view

If a field contains a value and you disable the field, the value is retained if you enable the field again later.

You can also display custom fields that were previously created. You can't design and create new custom fields within a board.

>[!NOTE]
>
>Any field customizations you make only apply to the board you are working in.

## Access requirements

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

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Configure cards {#configure-cards}

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Boards]**.
1. Access a board. For information, see [Create or edit a board](../../agile/get-started-with-boards/create-edit-board.md).
1. Click [!UICONTROL **Configure**] on the right of the board to open the Configure panel.
1. Expand [!UICONTROL **Cards**].

   Most fields are enabled by default.

1. Turn off a field to disable it in both card views.
1. Click the Hide icon ![Hide icon](assets/eye-hide-icon.png) next to a field to hide it on the condensed view.
1. To display all of the fields in both views, click [!UICONTROL **Restore all fields to default**].
1. Click [!UICONTROL **Hide configure**] to close the Configure panel.

## Add custom fields to cards

>[!NOTE]
>
>When you add a custom field to your cards, the data on the card is read-only. Also, custom fields are only available on connected cards.

1. Access a board and click [!UICONTROL **Configure**] to open the Configure panel.
1. Expand [!UICONTROL **Cards**].
1. Under [!UICONTROL Card Fields], click [!UICONTROL **Add custom field**].
1. Select [!UICONTROL **Task**] or [!UICONTROL **Issue**].

   The categories of available fields for tasks or issues appear. Expand a category to see all of the fields. You can also search for a field.

   ![Search for custom field](assets/boards-search-for-custom-field.png)

1. Select the field name.   

   The custom field is added to the list of available fields and is enabled by default. You can disable or hide the custom field following the steps in the [Configure cards](customize-fields-on-card.md#configure-cards) section above, or delete it from the board.

