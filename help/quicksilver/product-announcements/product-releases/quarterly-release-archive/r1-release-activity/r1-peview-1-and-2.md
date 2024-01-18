---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 1 and 2
description: This page describes all changes available in the Preview environment with the R1.1 and R1.2 releases. The functionality on this page was made available in the Preview environment on January 19, 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
---
# R1 Preview 1 and 2

This page describes all changes available in the Preview environment with the R1.1 and R1.2 releases. The functionality on this page was made available in the Preview environment on January 19, 2017.

For a list of all changes made in R1, see [R1 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).&nbsp;

## Restore Projects, Tasks, and Issues from the Recycle Bin&nbsp;

Workfront administrators can now restore projects, tasks, and issues that have been deleted within the past 30 days. All information associated with the project, task, or issue is restored, including documents and custom data.

New options are also available for configuring what happens to hours that are logged against a project, task, or issue that is deleted. For more information, see [Configure affect on hours when an object is deleted and restored](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

For more information about restoring objects in Workfront, see [Restore deleted items](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

For information about how to view projects, tasks, and issues that have been recently restored, see [View restored item](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Approval Diagram Shows Visual Representation of Previous, Current, and Future Approval Steps

Now when an approval is pending on a project, task, or issue, a diagram is displayed. The approval diagram shows&nbsp;the current step in the approval process&nbsp;(which is pending), and also allows you to&nbsp;quickly view previous and future approval steps without navigating to the Approvals tab.

Prior to this change, information about approval steps was available only on the Approvals tab within the project, task, or issue, and it was displayed only in a list view rather than a diagram view. (This information is still available and unchanged in the Approvals tab.)

On projects, the approval information is displayed in the header next to the project title. On tasks and issues, the approval information is displayed in the right panel.

For more information, see [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md) in&nbsp; [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configure Objects to Be Updated That Are Pending Approval

When a project, task, or issue is pending approval, you can now configure whether users can:

* Edit the custom form of a project, task, or issue that is pending approval.  
  For information&nbsp;about how to configure projects, tasks, and issues to be edited when pending approval, see [Configure global approval settings](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Add issues to a project that is pending approval.  
  For information about how to configure projects to allow users to add issues when the project is pending approval, see [Configure system-wide project preferences](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Edit tasks and issues within a project that is pending approval.  
  For information about how to configure projects to allow users to edit tasks and&nbsp;issues when the project is pending approval, see [Configure system-wide project preferences](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Prior to this change, projects, tasks, and issues&nbsp;that were pending approval could not be edited; also, issues could not be added to projects that were pending approval, and tasks and issues could not be edited within projects that were pending approval.

## Assign Layout Templates to Groups

You can now assign layout templates to groups.

Prior to this change, you could assign layout templates to users, teams and job roles. Assigning a layout template to groups bears the lowest rank in layout template assignment priority.&nbsp;

For more information, see "Creating and Managing Layout Templates."

## Changes to Bulk Editing User Notifications

The functionality has changed around editing user email notification settings in bulk. When you select multiple users to edit their notification email settings, only the specific notifications that you are updating are changed for all the users selected. All the unchanged email notification settings remain the same for all the users selected, even if they are different from user to user.&nbsp;

Prior to this change, the email notification settings you selected were saved, and all the other unchanged notification settings were deselected when you saved your changes.&nbsp;

For more information, see the "Modifying User Notification Settings in Bulk" in [Modify your own email notifications](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Updated&nbsp;Look and Feel of Several Email Notifications

The look and feel of the following email notifications has been updated with a new UI:

* Issue assignment
* Commit date changes
* A project I'm on becomes active
* Approval decision to interested parties
* A predecessor task completion to task dependents
* Pending approval (project, task, issues)
* Status change on projects, tasks, issues

Remember&nbsp;to update the email address associated with your account to be able to test this functionality, as the Preview Sandbox clears the email addresses on all users.&nbsp; &nbsp; For more information about email notifications, see [Adobe Workfront notifications](../../../../workfront-basics/using-notifications/wf-notifications.md). &nbsp; 

## New Email Digest Options for Several Notifications Areas

The following notifications areas have had the "Daily Digest" option added:

* Information about Projects I'm on
* Information about Projects I Sponsor
* Approval Information
* Information about Work Assigned to Me
* Communication

For more information, see [Adobe Workfront notifications](../../../../workfront-basics/using-notifications/wf-notifications.md).&nbsp; Remember&nbsp;to update the email address associated with your account to be able to test this functionality, as the Preview Sandbox clears the email addresses on all users.&nbsp;

## Make a Group Public

When you make a group public, you can now add that group to users without being a group owner. You will have to have user administrative access to be able to edit users.

For more information about making a group public, see the [Create a group](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public)&nbsp;section in [Create a group](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Share the&nbsp;URL of an Object in the Mobile App&nbsp;

You can now share the URL on the following objects on the Workfront mobile app:

* Projects
* Tasks
* Issues
* Timesheets
* Documents

You can share a&nbsp;URL of an&nbsp;object in the following applications:

* Text Message
* Email
* Storage Drive (for example iCloud Drive)
* Another installed application (for example, Notes, Facebook)
* You can copy a link to the object to your clipboard and paste it later in any other application.&nbsp;

## Context-Sensitive Help in Setup

All the areas under the Setup menu have been updated with a Help icon in the top upper-right corner of the area. This icon provides a link to a Help Site article about that area. Some sections inside the Setup areas have also been updated with the Help icon.&nbsp;

## Add More Precise Expense Rates

Now you can add more exact&nbsp;expense rates when creating expense types. Expense rates can contain up to 4 characters after the decimal (for example, 1.0375). This means that any fields that use this rate can be more precise.

Prior to this change, expense rates could contain only up to 2 characters after the decimal (for example, 1.03).

For more information about creating expense rates, see [Create custom expense types](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

&nbsp; 

## R1 Preview 1 and 2 Release Webinar Recording

This Webinar was&nbsp;presented by the Workfront Release Readiness team on January&nbsp;19, 2017.&nbsp;This webinar was&nbsp;focused on the release changes in 2017 and covered new functionality that is available to test in Preview.
