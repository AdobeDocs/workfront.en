---
title: 22.1 Project enhancements
description: 22.1 Project enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
---
# 22.1 Project enhancements

This page describes all Project enhancements made with the 22.1 release to the Preview environment. These enhancements will be made available in the Production environment 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

the week of January 17, 2022.

For a list of all changes available with the 22.1 release, see [22.1 Release overview](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Change the default option for predecessors when copying or moving tasks

To minimize the number of manual steps when copying or moving tasks, we have updated the information that is copied or moved with the task by default. Now, all predecessors are copied or moved with the task by default, as the All Predecessors option is selected by default.

Prior to this enhancement, the All Predecessors option was deselected by default when copying or moving a task.

For more information, see the articles:

* [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) 
* [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## Updated toolbar on dashboard list and reports in dashboards

The toolbar on four dashboard pages now has a modern look and feel that matches other Workfront lists such as projects, tasks, and issues. This intuitive toolbar now makes it easier to add, edit, share, copy, and delete dashboards.

The pages with the updated toolbar are:

* Task reports (displayed in dashboards)
* All Dashboards list
* My Dashboards list
* Shared Dashboards list

For more information, see [Create and manage dashboards](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Add and edit custom forms Summary panel for documents

You can now add and edit custom forms directly in the document Summary panel.

With this change, you'll also see a new look and feel in the document Summary. There is a new Overview section, which contains the image thumbnail as well as the document details. You can also check documents in and out in the document details section.

Previously, you had to go to the custom forms tab in the Document Details to make edits or add custom forms.

For more information, see [Summary for documents overview](../../../documents/managing-documents/summary-for-documents.md).

## New experience when copying one or multiple tasks

To make your use of Workfront consistent with the new Adobe Workfront experience, we have redesigned the interface when copying a task. This is currently available when copying a task at the task level or copying a task or multiple tasks in a list.

Some of the improvements include:

* All information that you must update before you copy the task displays on one continuous page.
* Workfront checks whether you have access to the destination project immediately after choosing the project. Prior to this enhancement, a warning message indicating that you don't have the correct access showed after you confirmed the copy, which resulted in extra steps and the copy not being allowed.
* Ability to request access for a project where you want to copy the task without leaving the Copy Task box.

For more information, see [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## New experience when moving one or multiple tasks from a list

To offer a consistent experience when performing the same task, we have now updated the interface for moving one or multiple tasks from a list to match the experience when moving the task at the task level. (We had updated the experience for moving a task at the task level in a previous Preview release.)

For more information, see [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## New experience when moving a task at the task level

To make your use of Workfront consistent with the new Workfront experience, we have redesigned the interface for moving a task. This is currently available when moving a task at the task level. In a following release, we will extend this redesign to moving a task from a list.

Some of the improvements of this newly redesigned interface include:

* All information that you must update before the move displays on one continuous page.
* Workfront will check whether you have access to the destination project immediately after choosing the project. Prior to this enhancement, Workfront warned you that you don't have the correct access after you have confirmed the move which resulted in extra steps and the move not being allowed.
* Ability to request access for a project where you want to move the task without leaving the Move Task box.

For more information, see [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## New experience when converting an issue to a project using a template at the issue level

>[!NOTE]
>
>This feature was temporarily removed from the Production environment on March 4, 2022. It was later released in a phased roll-out beginning April 28, 2022. The roll-out was completed on May 5, 2022. This is now available in Preview and Production for all customers. (For the latest updates on the status of this feature releasing to Production, see [22.3 Release overview](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

To make your use of Workfront consistent with the new Workfront experience, we have redesigned the interface for converting an issue to a project when using a template when you convert it from the issue page.

You can now more easily access your list of favorites immediately after selecting to convert the issue.

The redesigned interface matches the experience when creating a project from a template which we have also updated recently.

For more information, see [Convert an issue to a project in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Convert issues to projects using a template from lists, reports, and dashboards

>[!NOTE]
>
>This feature was temporarily removed from the Production environment on March 4, 2022. It was later released in a phased roll-out beginning April 28, 2022. The roll-out was completed on May 5, 2022. This is now available in Preview and Production for all customers. (For the latest updates on the status of this feature releasing to Production, see [22.3 Release overview](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

To increase the efficiency of your work and make it easier for you to convert issues in a fast-paced environment, we have added the ability to convert an issue to a project using a template from a list, report, or a dashboard.

Prior to this enhancement, this functionality existed only when you converted the issue from the issue page.

For more information, see [Convert an issue to a project in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Filter by user list on agile boards shows users with most assignments first

>[!NOTE]
>
>This feature will not be included with the 22.1 release. It was removed from the Preview environment.

Now the filter shows the users with the most assignments first so they are easier to locate without scrolling through the list.

Previously, the filter by user list on both Kanban and Scrum boards was displayed alphabetically.

For more information, see the following information

* [Filter by user on the Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md) 
* [Filter by user on the Kanban board](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Limit the ability to add documents to a template you are sharing

Sometimes people add documents to a project template thinking that they're adding them to a project. Now you can help to prevent this—when you share a template with View access, you can disable the new advanced setting Add Documents. This disables your recipients' ability to add documents to the template.

For instructions on sharing a template, see [Share project templates](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

For information about the new advanced setting Add Documents, see the section in the article [Sharing a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Share a document folder

Now you can share a document folder and its contents from the Documents area. Previously this was not possible—you had to share each document in a folder separately.

For more information, see [Share a document folder](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

