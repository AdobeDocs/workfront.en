---
title: 23.3 Agile enhancements
description: 23.3 Agile enhancements
author: Lisa
feature: Product Announcements
---
# 23.3 Agile enhancements

This page describes all agile enhancements made with the 23.3 release to the Preview environment. These enhancements will be made available in the Production environment with the 23.3 release. 

For a list of all changes available at this point in the 23.3 release cycle, see [23.3 Release overview](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

For details on how to opt in to new Boards features before the quarterly release, see [Early feature opt-in for Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

## Agile View of a project displays a kanban board

The Agile View of a project now includes additional functionality to filter, group, and sort work in a kanban board. The new, flexible design of the view includes a robust search feature and the ability to add new tasks to the project directly from the board.

>[!NOTE]
>
>The Agile View exists only on a single project because it is an alternative view of the project, and you can't access it from other areas of Workfront such as the Boards dashboard.

While you are in the board, you can opt to switch to the legacy Agile View.

For more information, see [Manage a project in the Agile View](/help/quicksilver/manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3421283/){target=_blank}

## Sort by board columns

We have added the ability to sort the cards in the columns on a board. When you select an option to sort by, all columns are sorted. You can't sort a single column, and the backlog or intake column is not sorted.

You can sort in ascending or descending order by card name, due date, estimation, status, or connection (project name). Connection applies to connected cards only, and the other options will sort both connected and ad hoc cards in the column.

The "user order" option returns the cards to the order they were manually set, before any other sort options were applied. This is the default sort for the columns.

For more information, see [Filter and search in a board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3420932/){target=_blank}

## Dark mode now available on Adobe Workfront Boards

You can now display all of your boards and workstreams in dark mode. The new setting is available through the preferences on the Boards dashboard.

>[!NOTE]
>
>If your organization's instance of Workfront has been onboarded to the Adobe Unified Experience, you can enable dark theme formatting for all of Adobe Experience Cloud through your preferences menu (your profile picture), and you will not see a separate dark mode option for Workfront Boards.

For more information, see [Boards email notifications and preferences](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

## Goals available in workstream iterations in Adobe Workfront Boards

We have added the ability to add goals to an iteration, without having to list the goals on a card. Goals are added in a checklist format and can be marked complete. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.

Also, the Next Iteration column is now available on iteration boards. When you place a card in this column, it is automatically carried to the next iteration and does not return to the backlog. On the next iteration, the card appears in the column that corresponds with its status.

For more information, see [Create an iteration in a workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

## Add comments to cards on boards

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

You can now add comments to both ad hoc and connected cards on boards, and tag other users on the comments. Comments are available in the card details. The comment feature for boards uses the new Adobe Workfront commenting experience.

For more information, see [Add an ad hoc card to a board](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) and [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3420832/){target=_blank}

## Enhancements to the Boards tag manager

The tag manager interface has been improved, allowing you to create new tags quickly and apply them to cards. You can also create tags for workstreams.

For more information, see [Add tags](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

## Simple filters available on board intake columns

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

Simplified filters have been added to the intake column setup to allow you to define the intake column more quickly. The available filters are Workfront projects and assignments by team or user. You can switch to the advanced filters if you prefer.

For more information, see [Add an intake column to a board](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3419420/){target=_blank}

## Simple filters added to dynamic board template

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

The filters on the dynamic board template have been simplified to allow you to create a board more quickly. The available filters are Workfront projects and assignments by team or user. You can switch to the advanced filters if you prefer. These filter options are also in the Configure panel for dynamic boards.

For more information, see [Create or edit a board](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Dynamic board template

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

A new template, dynamic board, is now available for standalone boards. This template is not available for boards inside of a workstream.

The dynamic board allows you to automatically populate a board with cards based on a Workfront project. Using filters, cards are added to columns based on their status.

For more information, see [Create or edit a board](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3418600/){target=_blank}

## Migrate agile team Kanban cards to Boards

A new **Add to Boards** button on agile team Kanban boards allows you to add all cards from the Kanban board to a Workfront board. You can choose to create a new Workfront board or add the cards to an existing board.

The placement of cards on the Workfront board is based on column policies. (For example, a policy could move all cards with a status of "In Progress" to a specific column.) If there are no policies or the cards don't match the policies, the cards are placed in the leftmost column. At this time, cards in the Backlog column on the legacy board are not added to the Workfront board.

The cards are not removed from the agile team Kanban board, and card status changes will sync to both boards. You can keep both boards active until you are ready to switch to Workfront Boards.

For more information, see [Migrate agile team Kanban cards to Workfront boards](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md). 

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3420425/){target=_blank}

## Left navigation added to card details on Boards

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards.

As more field options are added to cards on Workfront Boards, the card details have grown longer. A new navigation panel on the left of the card details allows you to select a section and move automatically to that group of fields.

Also, you can now add URLs in the Description field and they will become clickable links when the card details are saved. These updates apply to both ad hoc and connected cards.

For more information, see [Add an ad hoc card to a board](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) and [Use connected cards on boards](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3418598/){target=_blank}

## Boards email notifications and preferences

>[!NOTE]
>
>This feature is available only through the early feature opt-in for Workfront Boards. Because email notifications are generally not used in Preview, this feature was released to Preview and Production (for early feature opt-in customers only) at the same time.

Email notifications are now available for Adobe Workfront Boards. The notifications are turned on by default and you can select in your preferences which emails you want to receive. You will receive an email when you are added to a board and when a card is assigned to you.

For more information, see [Boards email notifications and preferences](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3418597/){target=_blank}
