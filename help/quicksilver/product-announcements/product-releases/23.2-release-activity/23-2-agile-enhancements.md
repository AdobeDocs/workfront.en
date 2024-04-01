---
title: 23.2 Agile enhancements
description: 23.2 Agile enhancements
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc97f4a2-9c51-4ccd-8121-c00fd1ac6988
---
# 23.2 Agile enhancements

This page describes all agile enhancements made with the 23.2 release to the Preview environment. These enhancements will be made available in the Production environment with the 23.2 release. 

For a list of all changes available at this point in the 23.2 release cycle, see [23.2 Release overview](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Add tasks and issues from object details to a Workfront board or workstream

You can now add existing tasks or issues to a Workfront board or workstream card list directly from the object details. Any items you add to a board will become connected cards, and any items added to a workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Iteration functionality available in Adobe Workfront Boards

Several new features available in Workfront Boards make it possible to use agile Scrum functionality. These features include:

* Workstreams for grouping boards related to the same team, and collaborating on work
* A list of cards, or backlog of work, with the option to use sources to connect cards to Workfront tasks and issues
* Iteration planning and iteration process boards

Note that collections have been renamed to workstreams. Workstreams help you visualize data in different ways. You can display items on cards in a list, on a board, or on an iteration. Cards in a workstream can also be shared among multiple boards. You can easily facilitate workflows using cards and boards in a workstream.

For more information, see [Manage workstreams](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Create an iteration in a workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md), and [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3417059/){target=_blank} 

## Add tasks and issues from lists and reports to a workstream card list

You can now add existing tasks or issues to a workstream in Workfront Boards directly from a list or report view. Any items you add to the workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Add custom fields to cards on a board

You can now include custom fields on Adobe Workfront Boards. The field must already be created in Workfront. You can't design and create new custom fields within a board.

Like the default fields, you can choose to display the custom field on the full view of a card and the condensed view on the board.

Any data from the custom field on the card is read-only.

For more information, see [Customize which fields are displayed on a card](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

## Add tasks and issues from lists and reports to a Workfront board

You can now add existing tasks or issues to a Workfront board directly from a list or report view. Any items you add to the board will become connected cards.

Also, the Boards field is now available to add to lists and reports for tasks or issues. This field displays all boards that a task or issue has been added to.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).


## Log hours on connected cards on a board

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can now log hours on connected cards, the same way you would on a task or issue. You must have the correct permissions to the task or issue to log the time.

The time logging fields are not displayed on connected cards by default. You must enable **Hours** in the Configure area under Cards.

For more information, see [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).


## Customize display of fields on a card

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.


Customization is now available to configure which fields are displayed on a card, both in the the full view when the card is open, and in the condensed card view on the board. When you disable a field is is not displayed in either view. You can also enable a field in the full view and hide it from the condensed view.

For more information, see [Customize which fields are displayed on a card](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3415710/){target=_blank} 

## Define a default status for cards moved into a board column

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can now set a default status to apply to cards moved into a specific column, by selecting a custom status and a system status in the column policies. When you move a card into the column, Workfront first tries to apply the custom status (for example, Awaiting Feedback). If the custom status is not available for that card, Workfront will apply the system status instead (for example, On Hold). Also, if the status on the connected task or issue is changed to the custom or system status set in the column policy, the card is automatically moved to the column.

Previously, you were prompted to select a status for every card moved into the column, if multiple statuses were available.

For more information, see [Manage columns](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3415711/){target=_blank} 

## Collections now available in Adobe Workfront Boards

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can now create collections on the boards dashboard. A collection is a group of boards for collaborating on work. Once you have named the collection, you can add boards to the collection using a set of templates that offer predefined settings such as column names. You can also move standalone boards into a collection. Once a board is in a collection, it can be moved to another collection but it can't become a standalone board.

Adding members to a collection works the same way as adding members to a board. A person or team must be a member on the collection before they can be added as members on a board in the collection.

For more information, see [Manage collections](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md). 

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3415609/){target=_blank} 

## Estimation field on connected cards maps to Story Points field on Workfront objects

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

The Estimation field on connected cards in Workfront Boards now maps to the Story Points field for the associated Workfront object. 

The new Story Points field is an editable, free form field that you can add to a view in a list or report for tasks or issues. It is not tied to planned hours or team assignments.

Previously, the card estimation was a manual entry and was not mapped to any field on a task or issue.

Also, the Estimation field on both ad hoc and connected cards no longer has a character limit. Previously, the maximum number of characters was 99.

For more information, see [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Preview card in intake column

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can now click on a connected card in the intake column to see a view-only version of its contents. You can't edit the card contents until the card is moved out of the intake column to another column on the board.
