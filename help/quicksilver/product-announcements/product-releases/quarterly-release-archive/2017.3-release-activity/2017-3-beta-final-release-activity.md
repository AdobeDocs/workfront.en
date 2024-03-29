---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta Final release activity
description: This page describes all changes most recently available in the Preview environment with the 2017.3 Beta Final release. The functionality on this page was made available in the Preview environment on September 12, 2017. It will be made available in the Production environment in early November, 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
---
# 2017.3 Beta Final release activity

This page describes all changes most recently available in the Preview environment with the 2017.3 Beta Final release. The functionality on this page was made available in the Preview environment on September 12, 2017. It will be made available in&nbsp;the Production environment in early November, 2017.

>[!IMPORTANT]
>
>&nbsp;Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2017.3, see&nbsp; [2017.3 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

The 2017.3 Beta Final release contains enhancements for both for Workfront administrators and other users:

**For Administrators**

* [New Configuration for Recalling Requests in the Approval Settings Area](#new-configuration-for-recalling-requests-in-the-approval-settings-area) 
* [Configure Default Proof Roles](#configure-default-proof-roles)

**For All Users**

* [Home Area (Updated My Work Area)](#home-area-updated-my-work-area)  

* [Updated Layout Template to Support the Home Area](#updated-layout-template-to-support-the-home-area)  

* [Kanban for Agile](#kanban-for-agile) 
* [Include Issues on the Scrum Backlog for an Agile Team](#include-issues-on-the-scrum-backlog-for-an-agile-team) 
* [Include Issues on the Scrum Agile Story Board](#include-issues-on-the-scrum-agile-story-board) 
* [Apply Groupings and Filters to the Backlog for an Agile Team](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team) 
* [Enhanced @Tagging Functionality Returns in the Preview Environment](#enhanced-tagging-functionality-returns-in-the-preview-environment) 
* [Filter System Updates in the Update Stream Is Now Persistent across Objects](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects) 
* [Visualize Data in the Utilization Report](#visualize-data-in-the-utilization-report) 
* [Utilization Report Performance Improvement](#utilization-report-performance-improvement) 
* [Document Enhancements: Streamlined Interface](#document-enhancements-streamlined-interface) 
* [Proofing Enhancements within Workfront](#proofing-enhancements-within-workfront) 
* [Proofing Enhancements within Both Workfront Proof and Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront) 
* [Rich Text Formatting for Updates and Emails](#rich-text-formatting-for-updates-and-emails) 
* [New Gantt Chart Redesign](#new-gantt-chart-redesign) 
* [Built-In Reports Contain Updated Descriptions](#built-in-reports-contain-updated-descriptions) 
* [Branding in Exported Reports, Lists, and Dashboards](#branding-in-exported-reports-lists-and-dashboards) 
* [Improvements when Copying Tasks and Moving Tasks or Issues](#improvements-when-copying-tasks-and-moving-tasks-or-issues) 
* [New Grouping for Resource Budgeted Hour Reports: Allocation Date](#new-grouping-for-resource-budgeted-hour-reports-allocation-date) 
* [Resource Planner Improvements](#resource-planner-improvements) 
* [Mobile Improvements](#mobile-improvements) 
* [Workfront Integration with Slack](#workfront-integration-with-slack) 
* [Outlook 365 Improvements](#outlook-365-improvements) 
* [API Changes](#api-changes)

## Home Area (Updated My Work Area) {#home-area-updated-my-work-area}

>[!NOTE]
>
>This functionality will not be released to the Production environment with the 17.3 release; it will remain in Preview until early in 2018.

The new Home area provides an alternate, enhanced view to the same data that is currently available in the My Work area. The Home area provides the following benefits over the My Work area:

* A more streamlined and intuitive interface
* Enhanced performance

The following functionality is available in the My Work area but is not yet implemented in the Home area:

* View your personal calendar
* Update tasks and issues with rich text formatting
* Approve proofs
* View a list of work you submitted for approval 
* Create an ad hoc issue on a project 
* View only those approvals that have been delegated to you

For more information about using the new Home area, see [Use the Home area](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Updated Layout Template to Support the Home Area {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>This functionality will not be released to the Production environment with the 17.3 release; it will remain in Preview until early in 2018.

As a Workfront administrator, you can determine whether users in your organization have access to the Home area by configuring the layout template they are assigned to. Users who are not assigned a layout template can always access the Home area.

For more information, see "Customizing Home" in "Creating and Managing Layout Templates."

## Kanban for Agile&nbsp; {#kanban-for-agile}

Agile teams can now use a Kanban methodology within Workfront, in addition to the Scrum agile methodology already supported.

Scrum and Kanban agile methodologies in Workfront differ in the following ways:

**Benefits of Using Kanban in Workfront**

* Display the backlog on the Kanban agile story board.

  For more information, see in .

* Configure items on the backlog to be automatically added to the Kanban agile story board when other items are moved to a status that equates with Complete.

  For more information, see [Configure stories to be automatically added from the backlog](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)&nbsp;in [Configure Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure a Work In Progress (WIP) limit to be displayed on the Kanban agile story board.

  For more information, see [Configure the work in progress (WIP) limit](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) in [Configure Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Benefits of Using Scrum in Workfront**

* Add a set of stories to an agile iteration and create a story board for that iteration.
* Include issues on the Scrum story board.
* Include issues on the backlog&nbsp;of an agile team.

  For more information, see [Configure how dates are applied when adding work items to an iteration](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)&nbsp;in [Configure Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Subtasks can be displayed on the Scrum story board.
* View a burndown chart to see progress against stories during the iteration.

  For more information, see [Agile burndown chart overview](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

For more information about enabling and configuring Kanban for an agile team, see [Decide on an agile methodology](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) in [Create an agile team](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Include Issues on the Scrum Backlog for an Agile Team {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>This functionality was removed from the Production environment on November 14, 2017. It is planned to be reintroduced to the Preview environment early in 2018 with an enhanced design and increased stability. It will be available in the Production environment with the 2018.1 release.

You can now include issues on the backlog of your agile team when using the Scrum agile methodology (issues are not displayed on the backlog of an agile team when using the Kanban methodology). Existing Scrum agile teams must enable this functionality in order for issues to be included. Issues are automatically included on the backlog for Scrum agile teams that are created after the 2017.3 release.

Prior to this change, only tasks could be added to&nbsp;the backlog. If you wanted to add an issue, you first had to convert the issue to a task before it could be added.

Because you now have access to more than just tasks on the backlog, any custom task views previously available on the backlog are copied and added to the backlog as custom Backlog Work Item views.

For information about using issues on the backlog, see&nbsp; [Manage the agile backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

For information about enabling issues to be available on the backlog of an agile Scrum team, see&nbsp; [Configure how dates are applied when adding work items to an iteration](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)&nbsp;in [Configure Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Include Issues on the Scrum Agile Story Board {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>This functionality was removed from the Production environment on November 14, 2017. It is planned to be reintroduced to the Preview environment early in 2018 with an enhanced design and increased stability. It will be available in the Production environment with the 2018.1 release.

You can now include issues on the story board when using the Scrum agile methodology.

For more information, see [Configure status columns on the agile story board](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) in [Configure Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Apply Groupings and Filters to the Backlog for an Agile Team {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>This functionality was removed from the Production environment on November 14, 2017. It is planned to be reintroduced to the Preview environment early in 2018 with an enhanced design and increased stability. It will be available in the Production environment with the 2018.1 release.

The Grouping and Filter options are now available on the agile backlog, allowing you to organize your backlog by groupings, as well as filter for specific tasks and issues.

Prior to this change, you could apply on views to the agile backlog.

For more information,&nbsp;see&nbsp; [Manage the agile backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in&nbsp; [Manage the agile backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Rich Text Formatting for Updates and Emails {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>Formatting changes you make within the Preview environment might be reverted back to the unformatted state.

Now you can emphasize important information by formatting the comments and updates you make to Workfront objects.&nbsp;

Using the Rich Text tools, you can apply formatting attributes to text, make bulleted and numbered lists, and add hyperlinks to additional resources.

Formatting applied to comments in the Update Stream also displays in the Update email notifications. To learn more about formatting your comments, See [Update work](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Enhanced @Tagging Functionality Returns in the Preview Environment {#enhanced-tagging-functionality-returns-in-the-preview-environment}

You can once again use the @ symbol to tag other users in the Update Stream of all objects in the Preview environment.&nbsp;In the past @tagging placed the tagged user's first and last name in the Update Stream. Now, enhanced @tagging functionality displays only&nbsp;the user's first name. To learn more about tagging users in updates, see [Tag others on updates](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Filter System Updates in the Update Stream Is Now Persistent across Objects {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

The Filter System Updates option is now persistent across objects throughout the Workfront site. This allows you to hide system updates and view only user comments in the Update Stream on one object, and have that setting remain as you browse to other objects.

Prior to this change, you had to choose to filter out system updates for each object as you browsed the Workfront site.

For more information, see [Update work](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visualize Data in the Utilization Report {#visualize-data-in-the-utilization-report}

&nbsp;You can now view Utilization information in a chart view.&nbsp;

For more information, see [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Utilization Report Performance Improvement {#utilization-report-performance-improvement}

>[!NOTE]
>
>This feature was released in a patch after the Beta Final release.

Now when running a Utilization report, you are prompted to apply a filter prior to the report running. This change ensures that the most pertinent information is generated in the Utilization report as quickly as possible.

For more information about running a Utilization report, see [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Document Enhancements: Streamlined Interface {#document-enhancements-streamlined-interface}

The user experience for adding documents to Workfront is now more streamlined and intuitive. Now you can upload a document from your file system, request a document, or link a file from a third-party application (such as Google or Dropbox), all from a simple drop-down menu.&nbsp;

Previously, these options were available by launching the Add Documents dialog box.&nbsp;

For more information, see the following information:

* [Add documents to Adobe Workfront from your file system](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) 
* [Request a Document](../../../../documents/adding-documents-to-workfront/request-a-document.md) 
* [Link documents from external applications](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)&nbsp;

>[!NOTE]
>
>With this change, the option to paste an image or document from the clipboard is no longer available.

## Proofing Enhancements within Workfront {#proofing-enhancements-within-workfront}

* [Improved User Experience and Additional Functionality](#improved-user-experience-and-additional-functionality) 
* [Share Directly from the proofing viewer](#share-directly-from-the-proofing-viewer) 
* [Configure Default Proof Roles](#configure-default-proof-roles)

### Improved&nbsp;User Experience&nbsp;and Additional Functionality {#improved-user-experience-and-additional-functionality}

In addition to an improved&nbsp;user experience when creating proofs in Workfront, the following additional functionality is now available:

* Merge multiple images&nbsp;into a single proof.
* Proof websites in multiple resolutions (multiple resolutions can be created as individual proofs or can be combined into a single proof).
* Edit the file name during the upload process.
* Include custom fields on the proof creation form.
* Add a custom message to proof email notifications.
* Additional proof settings&nbsp;
* Real-time error validation when proofing a URL (Previously, you had to wait several minutes prior to an error being displayed)

For more information, see .

>[!NOTE]
>
>&nbsp;When creating a new proof with automated workflow, drag-and-drop is not supported for moving users from one stage to another. Instead, remove the user from one step, and add them to another.

*The option to move users from one step to another using drag-and-drop will be reintroduced with the 2018.1 release.*

### Share Directly from the proofing viewer {#share-directly-from-the-proofing-viewer}

Now you can share with specific Workfront users directly from the proofing viewer.

>[!NOTE]
>
>This functionality is available only for new proofs (proofs that are created after the 2017.3 release) and only for Workfront instances that are integrated with a Workfront Proof Premium account.

Prior to this change, you could share only by creating a link, then sharing that link with a user.&nbsp;

For more information, see [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Configure Default Proof Roles {#configure-default-proof-roles}

You can now configure the default proof roles that new users and guest users have to new proofs within the Workfront system.&nbsp;

This is the default role users are assigned to on a proof when the proof is shared with them.&nbsp;

## Proofing Enhancements within Both Workfront Proof and Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Restart and Skip in HTML5 Video proofing viewer (Keyboard Shortcuts)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts) 
* [HTML5 proofing viewer Updates](#html5-proofing-viewer-updates)

### Restart and Skip in HTML5 Video proofing viewer (Keyboard Shortcuts) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

There are now keyboard shortcuts within the HTML5 proofing viewer for video that allow you to restart the video from the beginning and to skip to the end of the video.

For more information about the available keyboard shortcuts, see [Keyboard shortcuts in the Workfront Proof proofing viewer](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### HTML5 proofing viewer Updates {#html5-proofing-viewer-updates}

The HTML5 viewer now supports static proofs.

Prior to this change, the HTML5 viewer supported only video proofs.&nbsp;

The HTML viewer includes the following new functionality when proofing static content:

* Make a single comment with markups on multiple pages when in Single view

  This was previously possible only when in Continuous view or Magazine view 

* Navigate proofs via the proof thumbnails

   * Easily identify the part of the proof which is being reviewed. This is important, especially when users work with bigger format proofs and long webpages, or any time the &nbsp;bigger zoom level is needed in order to see the details.
   * Change the zoom level
   * Pan the content

* Specify custom values in the Measurement tool 
* When annotating text within a proof in the proofing viewer in Workfront Proof, you can include options for indicating that the text should be bolded, italicized, and underlined.

The HTML5 viewer does not yet support all functionality currently available in the existing Flash viewer. The following functionality is not currently available but will be included in a future release:

* Rich media file support
* Compare mode (Video and static)
* Filter comments (video and static)
* Review hyperlinks in documents&nbsp;(static)
* Translations (video and static)
* Presence indicator that displays users who are currently working on the proof
* Share proofs

For more information about proofing static proofs in the HTML5 viewer, see .

As the Workfront administrator in Workfront Proof, you can determine whether users in your organization have access to the new HTML5 proofing viewer for video proofs.

## New Gantt Chart Redesign {#new-gantt-chart-redesign}

The new Gantt chart includes the following improvements:

* New icons and markers
* New option to zoom in and out of a specific time frame
* Smaller task cells in the list portion of the chart
* Redesigned options for settings, printing and switching to Projected Dates.

For more information about configuring options in the Gantt chart, see [Configure how information displays on the Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).&nbsp;

## Built-In Reports Contain Updated Descriptions {#built-in-reports-contain-updated-descriptions}

We have updated the descriptions for our system reports in Workfront, to include information about the type of report and the fields included. &nbsp;

Prior to this change, most of our built-in reports had no descriptions or a very limited one.

For more information about built-in reports, see [Use Adobe Workfront built-in reports](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Branding in Exported Reports, Lists, and Dashboards {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>This feature is not currently available on all clusters in the Preview environment.

If you are leveraging branding in Workfront, the logo that you are using in your Global Navigation Bar is now included in the .pdf files that you export from Workfront.

The following .pdf files will include the logo of your organization on the exported document:

* Exported lists
* Exported and delivered Reports
* Printed Dashboards

For more information about exporting data from Workfront, see [Export data](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Improvements when Copying Tasks and Moving Tasks or Issues {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

We have improved the way you copy a task or move a task or an issue, to make it easier to select a parent for the copied or moved task or issue. When selecting a parent while copying a task, for example, you can now see a hierarchy of tasks, with their parent - child relationship, as well as search for a parent in projects with a lot of tasks.

Prior to this change, there was no Search field in the **Select a Parent** step, and the hierarchy of tasks was not visible in the task list.

For more information about copying tasks, see [Copy and duplicate tasks](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

For more information about moving issues, see [Move issues](../../../../manage-work/issues/manage-issues/move-issues.md).

## New Configuration for Recalling Requests in the Approval Settings Area {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

We have introduced a new setting in the Approval Settings area at the system level, to allow Workfront administrators to decide whether they should allow users to recall an issue or request whose first status is pending approval. If the recall is allowed, the issue is deleted; if the recall is not allowed, users cannot see a Recall button when the first status of an issue is pending approval.

Prior to this change, a recall of the issue was always allowed. When the approval was recalled, the approval was bypassed completely, placing the issue in its first status, with no approval attached.

For more information about approval settings, see [Configure global approval settings](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).&nbsp;

>[!NOTE]
>
>This option will be disabled by default, when this feature releases. Currently recalling issues is enabled by default for all organizations. When this feature releases, the Workfront administrator must manually enable this setting to keep the functionality as is in Workfront.

## New Grouping for Resource Budgeted Hour Reports: Allocation Date {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

We have added the ability to group your results by Allocation Date when you are building a Resource Budgeted Hour report.

Prior to this change, you were able to display the Allocation Date in the view of the report, as well as use it in a filter, but you could not use this field in a grouping.

For more information about the Allocation Date, see [Glossary of Adobe Workfront terminology](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

For more information about building a report, see [Create a custom report](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Resource Planner Improvements {#resource-planner-improvements}

* [Resource Planner: Show Data by FTE](#resource-planner-show-data-by-fte) 
* [Resource Planner: Show Data by Week and Quarter](#resource-planner-show-data-by-week-and-quarter) 
* [Resource Planner: View by User](#resource-planner-view-by-user) 
* [Resource Planner: Drag and Drop Projects to Establish Priority](#resource-planner-drag-and-drop-projects-to-establish-priority) 
* [Resource Planner: Export the data in the Resource Planner to Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Resource Planner:&nbsp;Show Data by FTE {#resource-planner-show-data-by-fte}

You can now display the allocation and availability of your resources by FTE in the Resource Planner. Prior to this change, you could only display the values in hours.

For more information about using the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resource Planner:&nbsp;Show Data by Week and Quarter {#resource-planner-show-data-by-week-and-quarter}

You can now change the time frame interval for your Resource Planner to view it by week or quarter. Prior to this change, you could view the allocation and availability of your resources and budget them only by month.

For more information about using the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resource Planner: View by User {#resource-planner-view-by-user}

You can now display the information in the Resource Planner by user, first, then by projects, roles, and tasks. You can also display a difference between the Planned and Available Hours or FTE for users. Prior to this change, you could display the information in the Resource Planner by projects and roles.

For more information about using the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resource Planner:&nbsp;Drag and Drop Projects to Establish Priority {#resource-planner-drag-and-drop-projects-to-establish-priority}

You can now drag and drop projects in your desired order of priority. Prior to this change, you could establish the priority of projects only by manually assigning them a number.

For more information about using the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resource Planner:&nbsp;Export the data in the Resource Planner to Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

You can now export the information in the Resource Planner to an Excel file.

For more information about using the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Mobile Improvements {#mobile-improvements}

We have added the ability to access your projects and manage them from the Workfront Mobile App. You can now do the following using the Workfront mobile app:

* Access a list of your projects
* Access a list of tasks and subtasks on a project
* Access a list of issues on a project
* Log a new issue on a project

You can install this functionality when you update your Workfront mobile app. The update will be available in both the Apple and Android mobile stores in November 2017.

## Workfront Integration with Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>The Slack integration is not currently available. It will be available to use with your Production environment in November, 2017.

We are launching a new integration between Workfront and Slack. If your organization has already been using Slack for your communication, you can now integrate it with Workfront and perform common Workfront actions without leaving your communication channels in Slack. You can now perform the following actions from your Slack account:

* Search for an item in Workfront
* Access your work and approvals lists
* Create a task
* Create an issue
* Subscribe to any item from a link that is shared with you to that item
* Assign tasks and issues from a link shared with you to them
* Approve your work
* Access your Favorites and your Recent Items lists

For more information about accessing Workfront from Slack, see [Using Workfront with Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Outlook 365 Improvements {#outlook-365-improvements}

We have made the following improvements to the Workfront add-in for&nbsp; Outlook 365:

* Add a task or an issue to a project in Workfront: You can now convert an email to a task or an issue in Workfront, using the Outlook 365 add-in. In this process, you can specify a project you want the task or the issue to be added to, as well as an assignee and a due date. Prior to this enhancement, you could only submit a request to a request queue or add a personal task to your Working On list from Outlook 365.&nbsp;
* Preserve a link to Workfront objects in the original email converted to tasks, issues, or requests: When you convert an email from Outlook 365 to a task, an issue, or a request, Outlook 365 preserves a link to the task or issue that was converted from that email inside the original email. Prior to this change, there was no indication in Outlook whether an email had been converted to a task or submitted as a request.&nbsp;

  For more information about converting an email to a task or an issue from Outlook 365, see [Add an Outlook email to a project as a task or an issue](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

## API Changes {#api-changes}

* [API 8 Now Available](#api-8-now-available) 
* [Removed and Deprecated Versions of the API](#removed-and-deprecated-versions-of-the-api) 
* [2017.3 Beta Final release activity](#updated-message-format-for-event-subscriptions) 
* [Event Subscription Retries for Undeliverable Messages](#event-subscription-retries-for-undeliverable-messages)

### API 8 Now Available {#api-8-now-available}

Workfront API Version 8 is now available and offers you new and updated resources for your Workfront integrations.

For a listing of changes made to the Workfront API, see [Updates to API Version 8](../../../../wf-api/api/new-api-version-8-updates.md).

### Removed and Deprecated Versions of the API {#removed-and-deprecated-versions-of-the-api}

### Updated Message Format for Event Subscriptions

In order to provide more useful information for your integrations that include the Workfront Event Subscriptions API, we've changed the outbound message format for supported resources by including the old and new values associated with those resources. In order to avoid failure, any integrations you have using the Workfront Event Subscriptions API will need to be updated the new format, as described in [Event Subscription API](../../../../wf-api/general/event-subs-api.md).

### Event Subscription Retries for Undeliverable Messages {#event-subscription-retries-for-undeliverable-messages}

The&nbsp;Workfront Event Subscription framework now provides a mechanism for handling event-triggered outbound messages that fail to deliver to customer endpoints. In order to&nbsp;ensure continued message delivery,&nbsp;Customers should make certain that any endpoints consuming outbound messages from event subscriptions are setup properly. For more information, see [Event subscription retries](../../../../wf-api/api/event-sub-retries.md).
