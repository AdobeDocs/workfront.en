---
title: project updates during the 22.3 release timeframe
description: project updates during the 22.3 release timeframe
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
---
# 22.3 Project enhancements

This page describes all Project enhancements made with the 22.3 release to the Preview environment. These enhancements were made available in the Production environment the week of July 11, 2022. For a list of all changes available with the 22.3 release, see [22.3 Release overview](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Out-of-office work delegation

Now, you can temporarily delegate the tasks and issues assigned to you to other users when you plan to be out of the office for a brief period of time. This ensures that your absence does not become a roadblock to work being completed.

Prior to this enhancement, you could only delegate approvals.

The following are some of the features we added with this update:

*   A setting in the Tasks & Issues Preferences area of Setup for the System or Group Administrator to enable delegation in your environment.
    
*   A new option for "Delegate tasks and issues" in the Home area for users with a Review or higher license to delegate their work items.
    
*   Indication in the Home and in the Assignments area of task and issue headers that items are delegated to others.
    
*   Event notifications in the Setup area and Email notifications in the user profile to control email notifications about delegated work
    

>[!NOTE]
>
>Only users with a Review or higher license can delegate their work to others. Work can be delegated to any user, regardless of their access level. Delegated users receive the same permissions as the assignees on the delegated items. If these permissions are lower than a user's access level configuration, the delegated users might be prevented from performing some of the activities on the tasks and issues that are delegated to them.


For more information, see [Delegate task and issue overview](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## New experience when converting an issue to a task

To make your use of Workfront consistent with the new Workfront experience, we have redesigned the interface for converting an issue to a task.

This update includes:

*   An updated user interface that matches the rest of the new Workfront experience.
    
*   Access to convert an issue to tasks from a list or a report.
    
*   The default custom forms defined in the Tasks Settings area of the destination project added to the new task.
    

For more information, see [Convert an issue to a task in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## New experience when converting an issue to a project without a template

To make your use of Workfront consistent with the new Workfront experience, we have redesigned the interface for converting an issue to a project without using a template.

In addition to an updated user interface that matches the rest of the new Workfront experience, we have also added the ability to convert an issue to blank projects from a list or a report.

For more information, see [Convert an issue to a project in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Smart tagging in the update stream

We have improved tagging users in the update stream when you create a new update or reply to an existing one. Now, when you tag a user to include them in an update, in addition to their name and avatar, we also display their Primary Role and their email. This helps distinguish between multiple users with similar or identical names.

For more information, see [Tag others on updates](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## New syntax for calculations in custom fields

To prepare for future enhancements that will help you add calculations to custom forms, we have standardized the syntax for referenced fields that you add to a calculation. It's easy to use this new syntax because the system enters it for you when you start typing the name of a field and then select it.

## Keep accurate information when two users with a common role are involved in an approval process

To ensure accuracy of your data for approving work, we have made a change in the way approval information is recorded on an item when a multi-role approval process is associated with the item.

Some approval processes require approval from two different roles, and two different approvers might have one of those roles in common. Now when this happens, after the approval decisions are made, Workfront records each approver and their respective role associated with the approval process.

Prior to this change, both approvals were recorded for the second user because they shared one of the approval roles with the first approver. In this case, the second approver was overwriting the first approver's information.

For more information about approval processes in Workfront, see [Approval process overview](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Allocation hours will no longer be removed when making changes to assignments

>[!NOTE]
>
>This feature was originally planned to release with the 22.2 release. It was released to Production on April 21, 2022.


To ensure the accuracy of your data, we have made a change to preserve allocation hours and to keep task Planned Hours unchanged when making changes to assignments on the task.

The following changes have been made to tasks with a Simple Duration Type:

*   Planned Hours are preserved when removing all assignees.
    
*   Individual assignment allocations are preserved when replacing users and roles.
    
*   Individual assignment allocations are preserved on the role when removing the user. (Removed from release. Now, Planned Hours will be set to 0 after removing all assignees.)
    

For more information about Planned Hours, see [Planned Hours overview](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Boards enhancements

The following enhancements have been added to Adobe Workfront boards:

*   Filter options - You can now filter by due date or status on a board. The filter has also been updated with collapsible sections to separate the options.
    
*   Archive board - You can now archive a board while you are in the board, instead of having to go to the boards dashboard.
    
*   Add a team to a board - When you search for members, you can add an entire team. Choosing a team adds everyone on the team to the board.
    
*   Drop zones in columns - When dragging and dropping a card from one board column to another, a gray "drop zone" now shows where the card will be placed. Previously there was not a visual indicator of the card placement.
    
*   Connected cards - You can now add cards that are connected to Workfront tasks and issues. Updating the name, description, or assignee in the card or the task will update the same fields in the other location.
    
*   Status field on all cards - A Status field and a Mark Complete button have been added to both ad hoc and connected cards. When you click Mark Complete, the status automatically changes to Complete.
    
*   Convert ad hoc card to connected card - You now have the option to convert an ad hoc card to a connected card from the card details.
    
*   Disconnect connected card - Disconnecting a connected card breaks the connection with the Workfront object. The card remains as an ad hoc card on the board, and the Workfront object is not affected.
    
*   Status mapping in columns - New column settings and policies allow you to define a status, assignee, or tag that is applied to cards moved to that column. Also, the default column names on a new board have been changed to Column 1, Column 2, and Column 3.
    
*   Field update indicator - An indicator now displays when you save a card, to confirm that your updates were saved.
    

For more information, see [Get started with boards in Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Share folders only in the top five levels of a folder hierarchy

To ensure the best performance for users sharing folders, we are currently limiting sharing to the top five levels in a folder hierarchy on an object.

Each folder at the sixth level or below inherits its sharing configurations from the folder directly above it.

For more information about sharing folders, see [Share a top-level document folder](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Workfront Campaigns (Beta) – a new way to manage your work

>[!NOTE]
>
>This feature is planned to be removed from Preview on January 9, 2023. For more information, see the [23.1 Release overview page](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>This feature will not be included with the 22.3 Production release. It will be released to Production with a future release.


>[!NOTE]
>
>This functionality is available only as a beta and is currently under construction. We will continue to add features for the Campaign workflow with future releases. Participation in the beta program for Workfront Campaigns is voluntary. 

We are introducing a new object to Adobe Workfront that has the potential to change the way you manage work.

Workfront Campaigns enables you to organize projects from different portfolios and programs in a new work container. This new container will evolve in future releases to eventually include all work objects that are currently managed in separate silos.

The following features are included with this release:

*   A new Workfront object called Campaign
    
*   A new Campaigns (Beta) area in the Main Menu
    
*   A list of Campaigns in the Campaigns area
    
*   A Campaign Details page that displays additional information about a campaign
    
*   Ability to add Projects to a Campaign
    
*   Ability to edit information about a Campaign
    
*   Ability to rename the Campaign object from the Layout Template
    
    Workfront system and group administrators can add the Campaigns (Beta) area in the Main Menu of a Layout template. This makes it available for all users assigned to the template. After it's available, anyone in Workfront can create a campaign.
    



