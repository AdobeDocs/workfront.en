---
filename: r1-peview-1-and-2
content-type: release-notes
navigation-topic: product-releases-archive
---




# R1 Preview 1 and 2 {#r-preview-and}

This page describes all changes available in the Preview environment with the R1.1 and R1.2 releases. The functionality on this page was made available in the Preview environment on January 19, 2017.


For a list of all changes made in R1, see [R1 release activity overview](r1-release-activity-overview.md).&nbsp;


## Restore Projects, Tasks, and Issues from the Recycle Bin&nbsp; {#restore-projects-tasks-and-issues-from-the-recycle-bin}

`Workfront` administrators can now restore projects, tasks, and issues that have been deleted within the past 30 days. All information associated with the project, task, or issue is restored, including documents and custom data.


New options are also available for configuring what happens to hours that are logged against a project, task, or issue that is deleted. For more information, see [Configure affect on hours when an object is deleted and restored](configure-how-hours-affected-when-obj-deleted-restored.md).


For more information about restoring objects in `Workfront`, see [Restore deleted items](restore-deleted-items.md).


For information about how to view projects, tasks, and issues that have been recently restored, see [View restored items](view-restored-items.md).


`<iframe class="mt-media" src="assets/197926164?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Approval Diagram Shows Visual Representation of Previous, Current, and Future Approval Steps {#approval-diagram-shows-visual-representation-of-previous-current-and-future-approval-steps}

Now when an approval is pending on a project, task, or issue, a diagram is displayed. The approval diagram shows&nbsp;the current step in the approval process&nbsp;(which is pending), and also allows you to&nbsp;quickly view previous and future approval steps without navigating to the Approvals tab.


Prior to this change, information about approval steps was available only on the Approvals tab within the project, task, or issue, and it was displayed only in a list view rather than a diagram view. (This information is still available and unchanged in the Approvals tab.)


On projects, the approval information is displayed in the header next to the project title. On tasks and issues, the approval information is displayed in the right panel.


For more information, see [Approving work](approving-work.md) in&nbsp; [Approving work](approving-work.md).


`<iframe class="mt-media" src="assets/197945794?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Configure Objects to Be Updated That Are Pending Approval {#configure-objects-to-be-updated-that-are-pending-approval}

When a project, task, or issue is pending approval, you can now configure whether users can:



* Edit the custom form of a project, task, or issue that is pending approval.  
  For information&nbsp;about how to configure projects, tasks, and issues to be edited when pending approval, see [Establish approval settings](establish-approval-settings.md)

* Add issues to a project that is pending approval.  
  For information about how to configure projects to allow users to add issues when the project is pending approval, see [Set project preferences](set-project-preferences.md).

* Edit tasks and issues within a project that is pending approval.  
  For information about how to configure projects to allow users to edit tasks and&nbsp;issues when the project is pending approval, see [Set project preferences](set-project-preferences.md).



Prior to this change, projects, tasks, and issues&nbsp;that were pending approval could not be edited; also, issues could not be added to projects that were pending approval, and tasks and issues could not be edited within projects that were pending approval.


`<iframe class="mt-media" src="assets/200189960?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Assign Layout Templates to Groups {#assign-layout-templates-to-groups}

You can now assign layout templates to groups. 


Prior to this change, you could assign layout templates to users, teams and job roles. Assigning a layout template to groups bears the lowest rank in layout template assignment priority.&nbsp; 


For more information, see "Creating and Managing Layout Templates."


`<iframe class="mt-media" src="assets/199878572?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Changes to Bulk Editing User Notifications {#changes-to-bulk-editing-user-notifications}

The functionality has changed around editing user email notification settings in bulk. When you select multiple users to edit their notification email settings, only the specific notifications that you are updating are changed for all the users selected. All the unchanged email notification settings remain the same for all the users selected, even if they are different from user to user.&nbsp; 


Prior to this change, the email notification settings you selected were saved, and all the other unchanged notification settings were deselected when you saved your changes.&nbsp; 


For more information, see the "Modifying User Notification Settings in Bulk" in [Configure email notifications](configure-email-notifications.md).


`<iframe class="mt-media" src="assets/200095138?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Updated&nbsp;Look and Feel of Several Email Notifications {#updated-look-and-feel-of-several-email-notifications}

The look and feel of the following email notifications has been updated with a new UI: 


* Issue assignment
* Commit date changes
* A project I’m on becomes active
* Approval decision to interested parties
* A predecessor task completion to task dependents
* Pending approval (project, task, issues)
* Status change on projects, tasks, issues


Remember&nbsp;to update the email address associated with your account to be able to test this functionality, as the Preview Sandbox clears the email addresses on all users.&nbsp; &nbsp; For more information about email notifications, see [Email notifications](email-notifications.md). &nbsp; 

## New Email Digest Options for Several Notifications Areas {#new-email-digest-options-for-several-notifications-areas}

The following notifications areas have had the "Daily Digest" option added:



* Information about Projects I’m on
* Information about Projects I Sponsor
* Approval Information
* Information about Work Assigned to Me
* Communication


For more information, see [Email notifications](email-notifications.md).&nbsp; Remember&nbsp;to update the email address associated with your account to be able to test this functionality, as the Preview Sandbox clears the email addresses on all users.&nbsp; 


`<iframe class="mt-media" src="assets/200094754?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;  


## Make a Group Public {#make-a-group-public}




When you make a group public, you can now add that group to users without being a group owner. You will have to have user administrative access to be able to edit users.


For more information about making a group public, see the [Create and manage groups](create-manage-groups.md#making-a-group-public)&nbsp;section in [Create and manage groups](create-manage-groups.md).


`<iframe class="mt-media" src="assets/197949010?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Share the&nbsp;URL of an Object in the Mobile App&nbsp; {#share-the-url-of-an-object-in-the-mobile-app}

You can now share the URL on the following objects on the `Workfront` mobile app: 


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


For more information, see the "Sharing a URL in the Mobile App" section on .


`<iframe class="mt-media" src="assets/200086398?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Context-Sensitive Help in Setup {#context-sensitive-help-in-setup}

All the areas under the Setup menu have been updated with a Help icon in the top upper-right corner of the area. This icon provides a link to a Help Site article about that area. Some sections inside the Setup areas have also been updated with the Help icon.&nbsp;


`<iframe class="mt-media" src="assets/197949016?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;&nbsp;


## Add More Precise Expense Rates {#add-more-precise-expense-rates}

Now you can add more exact&nbsp;expense rates when creating expense types. Expense rates can contain up to 4 characters after the decimal (for example, 1.0375). This means that any fields that use this rate can be more precise.


Prior to this change, expense rates could contain only up to 2 characters after the decimal (for example, 1.03).


For more information about creating expense rates, see [Create custom expense types](create-custom-expense-types.md).


## Updated Look and Improved Performance in the Tasks&nbsp;List (by request only) {#updated-look-and-improved-performance-in-the-tasks-list-by-request-only}

This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta). &nbsp; 

## R1 Preview 1 and 2 Release Webinar Recording {#r-preview-and-release-webinar-recording}

This Webinar was presented by the `Workfront` Release Readiness team on January&nbsp;19, 2017.&nbsp;This webinar was&nbsp;focused on the release changes in 2017 and covered new functionality that is available to test in Preview.


The webinar recording is available below.


`<iframe class="mt-media" src="assets/200216498?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`&nbsp;
&nbsp; 