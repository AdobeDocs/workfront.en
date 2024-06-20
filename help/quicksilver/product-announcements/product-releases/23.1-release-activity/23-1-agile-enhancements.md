---
title: 23.1 Agile enhancements
description: 23.1 Agile enhancements
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
---
# 23.1 Agile enhancements

This page describes all Agile enhancements made with the 23.1 release to the Preview environment. These enhancements will be made available in the Production environment the week of January 16, 2023. 

For a list of all changes available with the 23.1 release, see [23.1 Release overview](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Scrum planning for Workfront Boards

The new Scrum planning features in Adobe Workfront Boards offer flexible options to manage your agile processes. Using these tools, you can:

* Track work in iterations or sprints
* Use velocity to guide team commitments
* Track burndown and rate of completion

The Scrum planning features will be a "fast follow" after the 23.1 release.

## Due dates on cards map to planned completion date on Workfront object

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

Due dates on connected cards in Workfront Boards now map to the planned completion date on the associated Workfront object. If you update the due date on a card, the planned completion date is updated on the task or issue. Changing the planned completion date also changes the due date on the card. Previously, the card due date was a manual entry and was not mapped to any date on a task or issue.

Date mapping also applies to connected checklist items that are synced to subtasks.

The due date on both connected cards and ad hoc cards now also includes a time field.

For more information, see [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Board checklist items and Workfront subtasks are now linked

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

When you add a connected card to a board for a Workfront task, any subtasks are imported as checklist items on the card. Also, when you create a checklist item on a connected card, a subtask is added to the Workfront task. Checklist items on issues are not connected to any Workfront objects.

Previously, checklist items and subtasks were not linked. If you wanted to include a subtask on the board you could import it as a separate connected card or manually add a checklist item to a card.

For more information, see [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) and [Manage checklist items on cards](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Card counter on board columns

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

A new configuration setting is available to turn on a card counter for all of the columns on a board. If you are using the WIP limit on a column, a separate card counter is not added.

For more information, see [Manage board columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Search and sort on the boards dashboard

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can now sort the boards dashboard by board name or date, and search for a specific board in the list.

For more information, see [Use the boards dashboard](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Status displays on card

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

If a card on a board is assigned a status, the status now displays on the card so that you do not have to open the card to see the status. This enhancement applies to both ad hoc and connected cards.

For more information, see [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) and [Add an ad hoc card to a board](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![status on card](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Linkable cards now available on boards

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can now send a link to a specific card to another boards user. The person must have access to view the board before they can open the link.

When you open a card on a board, the browser URL looks like this: 

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

You can copy the full URL and send it to someone else. They will go directly to the open card when they access the link.

Previously, links were available to boards but not specific cards.

For information on cards, see [Add an ad hoc card to a board](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) and [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filter by connection on Boards

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

The list of filters on a board now includes the option to filter by connection, which shows you all of the connected cards for a specific project. You can also filter by cards that are not connected.

For more information, see [Filter and search in a board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Archive cards from a board on a schedule

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can configure a board so that cards are archived, or "fall off" the board, on a schedule. Options are available to set cards in a particular column to archive in a certain number of days or weeks. For example, you could define the falloff so that cards in a Complete column are archived after they are in the column for two weeks.

If you want to display the cards again after they fall off the board, you can set the board filter to display archived cards.

For more information, see [Configure card falloff](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3412323/){target=_blank}
