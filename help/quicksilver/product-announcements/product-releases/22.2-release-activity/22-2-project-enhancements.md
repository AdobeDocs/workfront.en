---
title: 22.2&nbsp;Project enhancements
description: 22.2&nbsp;Project enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
---
# 22.2&nbsp;Project enhancements

This page describes all Project enhancements made with the 22.2 release to the Preview environment. These enhancements will be made available in the Production environment 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

the week of April 4, 2022. For a list of all changes available with the 22.2 release, see [22.2 Release overview](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront Boards are now available!

Boards are flexible tools that allow team collaboration by providing access to a shared board containing columns and cards.

Using boards, you can:

* Quickly set up a task board with multiple columns
* Configure columns to show a status or category
* Add other users to the board and assign them to cards
* Quickly add open ended cards and checklists

Note that the cards on a board are not connected to objects and work items in Adobe Workfront.

A system administrator must enable Boards in layout templates to make the option available to all users in the main menu.

For more information, see [Boards overview](../../../agile/boards-overview.md).

## Additional improvements to Workfront Boards

The following additional improvements are now available for Workfront Boards:

* Tag cards on Boards

  You can now categorize cards on your board with color-coded tags. Tags allow you to quickly identify cards. You can even sort your board based on applied tags.

* Manage cards on Boards

  We've added the following features to help you manage cards on your board:

   * Copy a card: Create a copy of an existing card on your board.
   * Move a card: Quickly move cards to either the top or bottom of a board with the new Top of column and Bottom of column menu options.

* Search in Boards

  We've added a search bar to help you search all of the cards on your board.

* Set a due date for a card in Boards

  You can now set a due date for individual cards on your board.

For more information, see [Get started with boards in Adobe Workfront](../../../agile/get-started-with-boards/get-started-with-boards.md).

## Undo option for Update posts

It is now easier to catch mistakes when posting an update. Finalizing a comment in an object's Update tab now creates a pop-up window for 7 seconds that allows you to cancel the post and return to editing—before the system timestamps it or sends any emails and in-app notifications. If you dismiss the pop-up window, leave the page, or wait 7 seconds for the window to time out, the post will be made normally.

For more information, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Updated experience when copying and moving issues

To make your use of Workfront consistent with the new Adobe Workfront experience, we have redesigned the interface for copying and moving issues. This is currently available when copying or moving a single issue or when copying or moving issues in bulk from a list or report.

Some of the improvements of this newly redesigned interface include:

* All information that you must update before the move displays on one continuous page.
* Workfront checks whether you have access to the destination project immediately after choosing the project. Prior to this enhancement, Workfront warned you that you don't have the correct access after you have confirmed the move which resulted in extra steps and the move not being allowed.
* Ability to request access for a project where you want to move the issues without leaving the Move Task box.
* Ability to remove items (assignments, progress, documents, permissions, updates) from an issue when you move it to another location. This functionality was previously available only for copying issues.
* Ability to select a destination task in addition to a selecting a destination project when copying an issue.

For more information about moving or copying issues, see the following articles:

* [Copy issues](../../../manage-work/issues/manage-issues/copy-issues.md) 
* [Move issues](../../../manage-work/issues/manage-issues/move-issues.md)

## New experience when copying a project

To make your use of Workfront consistent with the new Adobe Workfront experience, we have redesigned the interface for copying projects. This is currently available when copying a project from the project page or when copying a project from a list or report. Prior to this update you could only copy a project from the project page.

For more information, see [Copy a project](../../../manage-work/projects/manage-projects/copy-project.md).

## Ability to manage projects from lists and reports from a new More menu

We have added a new More menu in project lists and reports to allow you to perform the following actions from these areas:

* For several projects at a time:
* Recalculate Timeline
* Recalculate Finance
* Recalculate Custom Expressions
* For a single project:
* Attach Template
* Export to MS Project
* Subscribe

For more information, see the following articles:

* [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) 
* [Recalculate project finances](../../../manage-work/projects/project-finances/recalculate-project-finances.md) 
* [Edit information in custom form fields](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md) 
* [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md) 
* [Export a project to Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md) 
* [Subscribe to items in Adobe Workfront](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Keep users on the dashboard, list, or report after converting issue to project

To increase efficiency and eliminate the number of clicks, we have released an improvement when converting issues to projects from a list, report, or a dashboard.

Users remain on the list, report or a dashboard after converting an issue to a project instead of being redirected to the project's page. A success notification with the link to the project displays after the conversion is complete, to allow you to easily navigate to the project, if needed.

For more information, see [Convert an issue to a project in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Allocation hours will no longer be removed when making changes to assignments

>[!NOTE]
>
>This feature was originally planned to release with the 22.2 release. It will be released to Production on April 21, 2022.

To ensure the accuracy of your data, we have made a change to preserve allocation hours and to keep task Planned Hours unchanged when making changes to assignments on the task.

The following changes have been made to tasks with a Simple Duration Type:

* Planned Hours are preserved when removing all assignees.
* Individual assignment allocations are preserved when replacing users and roles.
* Individual assignment allocations are preserved on the role when removing the user. (Removed from release. Now, Planned Hours will be set to 0 after removing all assignees.)

For more information about Planned Hours, see [Planned Hours overview](../../../manage-work/tasks/task-information/planned-hours.md).

## Share folders only in the top five levels of a folder hierarchy

>[!NOTE]
>
>This feature is temporarily unavailable. We will update this release note when the feature is available in Production.

To ensure the best performance for users sharing folders, we are currently limiting sharing to the top five levels in a folder hierarchy on an object.

Each folder at the sixth level or below inherits its sharing configurations from the folder directly above it.

For more information about sharing folders, see [Share a document folder](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

