---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Project enhancements
description: This page describes all enhancements made to Projects with the 2020.1 release. These enhancements are currently available in the Preview environment and will be made available in the Production environment in late March or early April, 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
---
# 2020.1 Project enhancements

This page describes all enhancements made to Projects with the 2020.1 release. These enhancements are currently available in the Preview environment and will be made available in the Production environment in late March or early April, 2020.

For a list of all changes available with the 2020.1 release, see [2020.1 release overview](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## More easily see who is tagged in an update

It's now easier to see which users are tagged in an update. Tagged users name's display in blue and link to the user profile.

Tagged users are also listed under the comment box.

Before this enhancement, the users previously tagged didn't show up in the Notify box.

For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Include and identify quoted text in an update comment or reply

As you type a comment, you can mark part of your comment as quoted text in order to distinguish it from your own comment. Use the Block Quote button in the HTML&nbsp;editor.

For more information, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Quote a previous comment in an update comment or reply

When you comment in an update thread, you can quickly include text from a previous comment in the thread. Look for the Quote Reply option in the More menu next to the comment you want to quote.

For more information, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Additional risks information

To help you better understand the risks of your projects, you can now see who and when a risk was entered and when it was updated on a project. You can access this information in a risk view and through the public Workfront API. These fields will be available with API version 11, which releases with the 2020.1 Production.

For information about risks in Workfront, see [Create and edit risks on projects](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Additional fields added to Baselines and Baseline Tasks

To help you better understand the financial progress of your projects, you can now include additional cost and revenue information in a Baseline or a Baseline Task report. The additional financial information is not added to the baselines that you have currently saved, but it is added for new baselines.

For information about project and task financial fields that are accessible from the Baseline and Baseline Task objects see [Project finances included in project baselines](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Issues in "Closed-Pending Approval" status are considered incomplete

The way Workfront handles issues in a "Complete-Pending Approval" status has been changed. Now, these issues are perceived as Open, and the project cannot be marked as Complete until the approval is resolved.

Prior to this change, issues in a "Closed-Pending Approval" status were considered Closed.

All issues that have been placed in a Closed - Pending Approval status before this change will behave the same way as they did previously, being considered as completed and allowing for the project to complete as well. All issues placed in this status after this change is made will be considered as incomplete.

For information about project statuses, see [Access the list of system project statuses](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

