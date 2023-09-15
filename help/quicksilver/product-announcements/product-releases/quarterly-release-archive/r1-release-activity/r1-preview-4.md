---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 4
description: This page describes all changes available in the Preview environment with the R1.4 release. The functionality on this page was made available in the Preview environment on February 15, 2017.
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
---
# R1 Preview 4

This page describes all changes available in the Preview environment with the R1.4 release. The functionality on this page was made available in the Preview environment on February 15, 2017.

For a list of all changes made in R1, see [The Workfront R1 release](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Updated Project, Task, and Issue Approvals

When creating approval processes for project, task, and issue approvals, the following enhancements and changes are now available:&nbsp;

* Approval "Steps" are now called approval "Stages."
* Include&nbsp;multiple types of approvers per stage.  
  This includes, users, teams, and job roles.  
  Prior to this change, you could include multiple approvers of the same type only. For example, you could include multiple job roles, but not a job role and a team.

* The following pre-existing limitations related to modifying existing global approval processes have been removed:

   * The modified approval process is&nbsp;reflected only on objects throughout the system where the approval process has either not yet started or where the approval process has not been modified. Objects where the approval process is already started or where the approval process has been modified are not updated with your changes.
   * You cannot modify the status that determines when the approval starts.

* Updated look and feel.

For more information about creating approval processes, see [Create an approval process for work items](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

When associating an approval process with a project, task, or issue, the following enhancements and changes are now available:

* Updated look and feel.
* Approval diagram is displayed on the Approvals tab, showing a visual representation of previous, current, and future approval steps.

For more information about associating approvals with projects, tasks, and issues, see [Associate a new or existing approval process with work](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Change the Status of a Project Directly from the Project Page

You no longer need to edit a project in order to change the project status. You can now change the status of a project directly from the main page of the project.

For more information, see [Change the status of a project](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Schedule Users for Deactivation

You can now schedule users to be deactivated at a future date.

Prior to this enhancement, you could only manually deactivate a user immediately.

Scheduling a user to be deactivated can be useful in a variety of scenarios. For example, if you create&nbsp;users in Workfront who are hired on a temporary basis, you can set them up to be deactivated when their contract ends.

This feature is also available when bulk editing users.&nbsp;

For more information about scheduling users for deactivation, see [Deactivate or reactivate a user](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) and [Add users](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## New Email Digest Options for "Actions Needed"

The Daily Digest delivery option is now available in&nbsp;the "Action Needed" area of your Notifications settings.

For more information, see [Modify your own email notifications](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Remember to update the email address associated with your account to be able to test this functionality. This is required because the Preview Sandbox clears the email addresses on all users.

## Recycle Bin Improvement: Recorded in the Update Stream and Receive Email Notification

The following enhancements were added when restoring deleted projects, tasks, and issues:

* You&nbsp;now receive an email notification after restoring an object.  
  As a Workfront administrator, you now receive an email notification after restoring a project, task, or issue that was previously deleted. The email notification informs you about the status of the restore process.  
  For more information about restoring objects in Workfront, see [Restore deleted items](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* When the object is restored, the deletion and restoration of the object is now recorded in the update stream of the object&nbsp;itself and in the update stream of the parent object.  
  Previously, only the deletion was recorded in the update stream of the parent object.  
  For example, when the task is restored, a message is added to the update stream of both the project&nbsp;and the task&nbsp;itself, indicating that the task was restored. (Deletions and restores are not recorded on subtasks. Information regarding deletions and restores of subtasks is available only on parent tasks.)  
  For more information, see [Restore deleted items](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

&nbsp;

## Updated Dialog Box for Managing Group Membership

There is a new interface for the management of Groups and Subgroups that offers an easier, more user-friendly experience.

The Group Owners field and the Group Members field are now combined into a single field, with a list of group members listed below. Additionally, you can filter the list of group members and change whether they are an Owner or a Member.&nbsp;

For more information about adding subgroups to groups as well as designating users as members or group owners of groups, see [Create a group](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)&nbsp;and [Create a group](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).&nbsp;

&nbsp;

## Copy Text in the Mobile App

You can copy text in the following fields of all the objects that are visible in the mobile app:

* Name
* Description
* Reference Number
* Comments

This functionality should be released to both the iOS and Android app stores the week of February 13th.
