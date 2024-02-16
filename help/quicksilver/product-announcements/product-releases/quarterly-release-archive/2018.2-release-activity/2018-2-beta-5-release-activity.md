---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 5 release activity
description: This page describes all changes most recently available in the Preview environment with the 2018.2 Beta 5 release. The functionality will be available in the Preview environment on June 1, 2018. Proofing enhancements releasing with Beta 5 will be available in the Preview environment on Monday, June 4. It will be made available in the Production environment in July 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
---
# 2018.2 Beta 5 release activity

This page describes all changes most recently available in the Preview environment with the 2018.2 Beta 5 release.&nbsp;The functionality will be available in the Preview environment on June 1, 2018.&nbsp;Proofing enhancements releasing with Beta 5 will be available in the Preview environment on Monday, June 4. It will be made available in&nbsp;the Production environment in July 2018.

>[!IMPORTANT]
>
>&nbsp;Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2018.2, see&nbsp; [2018.2 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

The 2018.2 Beta 5 release contains the enhancements for Workfront administrators and other users:

**For Administrators**

* [View User-Triggered Changes with Audit Logs](#view-user-triggered-changes-with-audit-logs) 
* [View License Information as a group administrator](#view-license-information-as-a-group-administrator)

**For All Users**

* [Calendar View in the Home Area](#calendar-view-in-the-home-area) 
* [Additional Updates to the Work List (Left Panel) in Home](#additional-updates-to-the-work-list-left-panel-in-home) 
* [Configure Job Role Limits for Automated Resource Scheduling](#configure-job-role-limits-for-automated-resource-scheduling) 
* [Project and Role View Improvements in the Resource Planner](#project-and-role-view-improvements-in-the-resource-planner) 
* [Resize Column Widths for Project Lists](#resize-column-widths-for-project-lists) 
* [Icon Support for the New Project Lists](#icon-support-for-the-new-project-lists) 
* [Add "Large Thumbnail" Field in Document Views](#add-large-thumbnail-field-in-document-views) 
* [Increase Excel Export Limit](#increase-excel-export-limit) 
* [Quick Filters for Project Lists](#quick-filters-for-project-lists) 
* [Reference Issue Collections in Project and Task Reports](#reference-issue-collections-in-project-and-task-reports) 
* [New More Robust Version Menu When Adding New Document Versions in Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront) 
* [Mobile Improvements in the Android Beta Mobile App](#mobile-improvements-in-the-android-beta-mobile-app) 
* [proofing viewer Enhancements (Workfront and Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof) 
* [Proofing Enhancements in Workfront](#proofing-enhancements-in-workfront) 
* [Proofing Enhancements in Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Calendar View in the Home Area {#calendar-view-in-the-home-area}

Now you can manage your personal work tasks and schedules using the Workfront Home Calendar view. The Home Calendar view allows you to do the following:

* Set your own schedule for accomplishing Workfront tasks assigned to you
* Quickly see the tasks that are coming due or overdue
* View your total allocated hours for a week
* Make updates to tasks assigned you

If you use a calendar in Outlook, you can integrate your calendar to display your Outlook events in your Home Calendar view.

For more information, see [Home Calendar view](../../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## Additional Updates to the Work List (Left Panel) in Home {#additional-updates-to-the-work-list-left-panel-in-home}

The following enhancements are now available for the Work List in the Home area:

* The number of completed items are now displayed in parenthesis next to the Completed option in the Filter drop-down menu.

  Previously, the number of completed items were not displayed in the Filter menu.&nbsp;

* Completed items are shown for the previous 2 weeks.

  Previously, completed items were shown for the previous 3 months.

  For information about viewing completed work in the Home area, see [Display items in the Work List in the Home area](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) in the article [Display items in the Work List in the Home area](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Add the Duration field and Assignments field to display when items are selected in the Home area.

  Previously, the Assignments field was available by default; however, if it was deleted, it could not be re-added. The Duration field was not previously available to add.

  For information about adding fields to the Home area, see "Creating and Managing Layout Templates."

For more information about using the Home area, see [Use the Home area](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## View User-Triggered Changes with Audit Logs {#view-user-triggered-changes-with-audit-logs}

We've created the following audit logs for Workfront administrators to track user-triggered changes:

* User Audit Log
* Access Level Audit Log
* Group Audit Logs
* Login Attempt Audit Logs

Previously, there was no way to track changes within the system.

For more information, see [View and export audit logs](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## View License Information as a group administrator {#view-license-information-as-a-group-administrator}

We've created a read-only Licenses page for group administrators to view license counts for the groups they administer.

Prior to this change, group administrators could not view license information.

For more information, see [Group administrators](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Configure Job Role Limits for Automated Resource Scheduling {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

In the Automated Resource Scheduling settings, you can now assign a limit to a job role. This allows you to control the number of resources, with the same role, being assigned work.

Previously, you could not specify how many users within a certain job role could be assigned work.

For more information, see "Manually assign unassigned tasks and issues in the Scheduling areas".

## Project and Role View Improvements in the Resource Planner {#project-and-role-view-improvements-in-the-resource-planner}

The Project and Role Views of the Resource Planner now contain the following improvements:

* Improved filters which pull information from the entire database, rather than just the information on the screen.
* Full-screen mode.
* Performance is now faster and more efficient.

   * New limits for the number of projects, roles, and users that you can display.
   * Lazy loading, for faster loading of projects and roles.

* Quick access to Projects and Users directly from the Resource Planner.
* Faster drag-and-drop capability in the Project View, to prioritize your projects.

Prior to these improvements, you have reported that the Resource Planner was slow to load and that you had noticed incongruences in the data displayed. With these improvements, these should now be eliminated.

For information and to understand the new limits for the Resource Planner, see [Resource Planner display limitations](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Resize Column Widths for Project Lists {#resize-column-widths-for-project-lists}

As we have been working on improving the functionality of our lists, we had temporarily disabled the ability to resize the widths of the columns in the following project lists:

* Projects I Own
* Projects I'm On
* All Projects

With this release, we can now again resize the columns of all project lists.

We have added additional improvements to this functionality.

Now, when you drag the right border of a column to resize it, the neighboring column to the right retains its size making the list wider, rather than also being modified. Also, you can drag the border of a column to the right past the borders of the neighboring columns.

Prior to this improvement, the neighboring column to the right of the resized column would proportionally be resized as well to fit on the screen and you could not drag the border of a column past the right border of the neighboring column. &nbsp;

For information about resizing the reordering columns in lists, see [Modify column width and order](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

To participate in our beta testing program for the current list improvements, see [New Lists Study.](http://community.workfront.com/discussions/community-home/digestviewer/viewthread?GroupId=457&MessageKey=6b135c15-33dd-4fa2-8bc3-7cd7f7740c57&CommunityKey=0425cafc-f0ec-47fc-be20-a21dc073d520&tab=digestviewer&ReturnUrl=%2fdiscussions%2fcommunity-home%2fdigestviewer%3fCommunityKey%3d0425cafc-f0ec-47fc-be20-a21dc073d520) (Login required)

## Icon Support for the New Project Lists {#icon-support-for-the-new-project-lists}

As we have been working on improving the functionality of our lists, we had temporarily disabled displaying status icons in the following project lists:

* Projects I Own
* Projects I'm On
* All Projects

With this release, status icons can be displayed again in your projects lists for projects, or other objects in a project list.

For information about working in lists, see [Get started with lists in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Add "Large Thumbnail" Field in Document Views {#add-large-thumbnail-field-in-document-views}

We are adding a new field called Large Thumbnail to a document view in a list or report. When selected in a document view, this field displays a 400 pixel-wide thumbnail of the document in a list or report.

Prior to this change, you could only add the Thumbnail field to a document view, which displays a 33-66 pixel-wide thumbnail of the document.

For information about fields in lists and reports, see [Glossary of Adobe Workfront terminology](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Increase Excel Export Limit {#increase-excel-export-limit}

We have increased the limit for how many rows you can export in an Excel file. You can now export the following:

* 65,000 rows in an Excel .xls file
* 100,000 rows in an Excel .xlsx file

The new limits apply when you export the following from Workfront:

* A list or report from the web interface
* A list or report using the API
* A scheduled and delivered report

Prior to this improvement, you could only export 50,000 rows in any Excel file.

For information about exporting data from Workfront, see [Export data](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Quick Filters for Project Lists {#quick-filters-for-project-lists}

You can now apply a quick filter to lists.

The purpose of a quick filter is to help you navigate directly to those items in your large lists that are of importance to you, so you can quickly review, update, or share them with others.

Currently, quick filters are available only for the project lists in the following sub-tabs:

* Projects I'm On
* Projects I Own
* All Projects

For information about quick filters, see the "Applying Quick Filters to Lists" section in [Get started with lists in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Reference Issue Collections in Project and Task Reports {#reference-issue-collections-in-project-and-task-reports}

You can now reference a collection of issues in a project or task view and filter. You can do so only using Text Mode while building a report.

Prior to this improvement, you were able to reference only a collection of tasks in a project view or filter.

For information about how to reference a collection in a report, see [Reference collections in a report](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

For information about using text mode, see&nbsp; [Overview of common uses for Text Mode](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>In the following video, the sample text mode for issue collections was incorrect. The correct sample text mode is available in [Reference collections in a report](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## New More Robust Version Menu When Adding New Document Versions in Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Now when adding new versions to documents in Workfront, the New Version menu contains additional options and is now consistent across areas of Workfront where you can add a new version.

You can add a new document version from the following areas of Workfront:

* From the More drop-down menu in the Documents tab.
* From the Document Actions menu on the document details page.
* From the All Versions tab on the document details page.

Prior to this change, only the More drop-down menu in the Documents tab contained all options for adding a new version.

The following options are now available&nbsp;in the New Version menu for all areas where you can add a new version:

* Proof 
* Document Only 
* Linked options (From Dropbox, From Google Drive, and so forth) 
* Paste from Clipboard (this is a new option when adding versions)

For more information, see [Add documents to Adobe Workfront from your file system](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) in the article [Add documents to Adobe Workfront from your file system](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Mobile Improvements in the Android Beta Mobile App {#mobile-improvements-in-the-android-beta-mobile-app}

The following improvements will be available on the Android Beta version of the mobile app shortly after the day of this release:

* Swipe actions

  You can perform activities like volunteer to work for a task, complete a task, mark a notification as seen or new, text or call a contact by swiping various objects in the Workfront mobile app.

  The following areas have been improved with this functionality:

   * My Work and Home
   * Notifications
   * Contacts
   * Approvals

* New look and feel when viewing the Details tab of an item

  The interface has changed when viewing an item in the Android Beta version of the mobile app to make it easier to edit, complete it, or attach a document to it.   

* New experience when logging time

  Logging time is faster and easier than before, with an easier to access Log Time button, and a more streamlined interface for logging hours.

With this release, these improvements are only available for the Android Beta version of the Workfront mobile app. They are currently not available for iOS.

For more information about how to sign up to be a beta tester and download the Android Beta version of the Workfront mobile app, see .

## proofing viewer Enhancements (Workfront and Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Updated Print Summary Page](#updated-print-summary-page) 
* [Add Users to a Proof Directly from the proofing viewer](#add-users-to-a-proof-directly-from-the-proofing-viewer) 
* [Display All Markup Tools in the proofing viewer](#display-all-markup-tools-in-the-proofing-viewer) 
* [Configure Default Sorting Options in the proofing viewer](#configure-default-sorting-options-in-the-proofing-viewer) 
* [View Workfront Document Approvals in the Desktop Proofing Viewer](#view-workfront-document-approvals-in-the-desktop-proofing-viewer) 
* [Configure Links That Open New Tabs and Windows to Open within the Desktop Proofing Viewer](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer) 
* [Presence Indicator in the proofing viewer](#presence-indicator-in-the-proofing-viewer) 
* [Filter Comments to Display a Single Page for Interactive URL Proofs in the Desktop Proofing Viewer](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer) 
* [Desktop Proofing Viewer for Static and Video Content](#desktop-proofing-viewer-for-static-and-video-content) 
* [Add Custom Devices to Your System](#add-custom-devices-to-your-system)

### Updated Print Summary Page {#updated-print-summary-page}

The Print Summary page has been updated with a new look and feel and improved functionality.

For information, see [Print a proof summary within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Add Users to a Proof Directly from the proofing viewer {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Now you can add users to a proof directly from the Web Proofing Viewer and the Desktop Proofing Viewer.&nbsp;

Previously, you could not add individual users to a proof. Rather, you could only copy the public URL or embed&nbsp;code.

For more information, see [Share a proof by adding users to it](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) in the article&nbsp; [Share a proof from the proofing viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Display All Markup Tools in the proofing viewer {#display-all-markup-tools-in-the-proofing-viewer}

You can now configure the markup tool to display all the time rather than in a menu you have to open. This makes it faster to switch between tools. When configured in this way, markup tools are display horizontally at the top of the Web Proofing Viewer and Desktop Proofing Viewer.

Previously, markup tools were available only within a drop-down menu.

For more information about configuring this markup setting, see [Configure proofing viewer settings](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

For more information about using markup options when reviewing a proof, see in the article .

### Configure Default Sorting Options in the proofing viewer {#configure-default-sorting-options-in-the-proofing-viewer}

Now when you change the sorting option within the comment list in a proof, that option becomes the default sorting option the next time you open any proof within the Web Proofing Viewer or Desktop Proofing Viewer.&nbsp;

For more information, see in the article&nbsp;.

### View Workfront Document Approvals in the Desktop Proofing Viewer {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Now you can make a Workfront document approval decision in the Desktop Proofing Viewer.

Previously, only the Web Proofing Viewer allowed you to make a Workfront document approval decision.&nbsp;

For more information, see&nbsp; [Make a decision on a proof in the proofing viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)&nbsp;in the article&nbsp; [Make a decision on a proof in the proofing viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Configure Links That Open New Tabs and Windows to Open within the Desktop Proofing Viewer {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

When proofing interactive content in the Desktop Proofing Viewer, you can now configure links that open in a new tab or new window to open within the Desktop Proofing Viewer so you can continue proofing.

In the Legacy proofing viewer,&nbsp;links that opened in a new tab or new window could not be reviewed in the proofing viewer.

For more information, see [Configure proofing viewer settings](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Presence Indicator in the proofing viewer {#presence-indicator-in-the-proofing-viewer}

Now when reviewing a proof in the Web Proofing Viewer or Desktop Proofing Viewer, you can view the avatar of each user currently viewing the proof is displayed in the upper-right corner of the proofing viewer.

For more information, see [Review a proof simultaneously with multiple reviewers](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filter Comments to Display a Single Page for Interactive URL Proofs in the Desktop Proofing Viewer {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

When reviewing a URL in an interactive proof in the Desktop Proofing Viewer, you can now filter comments to display comments made only on the current page.&nbsp;

Prior to this change, this option was available only for static proofs.

For more information, see in the article .

### Desktop Proofing Viewer for Static and Video Content {#desktop-proofing-viewer-for-static-and-video-content}

The Desktop Proofing Viewer now supports static and video content.

Previously, it supported only interactive content.

For information about configuring static and video proofs to open in the Desktop Proofing Viewer, see [Configure proofing viewer settings](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

For more information about the Desktop Proofing Viewer, see [Reviewing Proofs in the Desktop Proofing Viewer.](https://support.workfront.com/hc/en-us/sections/360000686434)

### Add Custom Devices to&nbsp;Your System {#add-custom-devices-to-your-system}

You can now add any custom devices to your system, allowing users to review interactive content and simulate how it appears on a specific device when reviewing a proof in the Desktop Proofing Viewer.

Prior to this change, users could choose only from a list of standard, preconfigured devices.

For information about adding custom devices, see in

For information about how users can select devices when reviewing interactive content, see [Change interactive proof resolution in the proofing viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Proofing Enhancements in Workfront {#proofing-enhancements-in-workfront}

* [Share the Proof Link Directly from Workfront](#share-the-proof-link-directly-from-workfront) 
* [Report on Additional Proofing Data in Workfront](#report-on-additional-proofing-data-in-workfront) 
* [View Historical Data for Proof Approvals in Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Share the Proof Link Directly from Workfront {#share-the-proof-link-directly-from-workfront}

Now you can generate a link for a proof within Workfront and share it directly from Workfront. Alternatively, you can copy the URL and distribute it using an alternate method.

Prior to this change, you could only copy the proof link within Workfront and distribute it using an alternate method.

For more information, see [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in the article [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>The embed link that is currently available will be removed in a future release. The embed link will still be accessible via the Workfront API.

### Report on Additional Proofing Data in Workfront {#report-on-additional-proofing-data-in-workfront}

In reports that contain the Document Version object (such as a Document Version report and Proof Approval report),&nbsp;several fields are now available that allow you to view additional proofing information.

* Proof Deadline

  Displays the day of the week, date, time of day, and year of the proof deadline.

* Proof Decision

  Displays the decision status of the proof (pending, changes required, or approved).

* Proof Name

  Displays the proof name.

* Proof Pages

  Displays the number of pages included in the proof.

* Proof Progress

  Displays the progress status of the proof (Sent, Opened, Commented, Decision Made).

For more information about each of these fields, see&nbsp; [Glossary of Adobe Workfront terminology](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### View Historical Data for Proof Approvals in Workfront {#view-historical-data-for-proof-approvals-in-workfront}

In the Proof Approval report, you can add a field that lets you view proof approval decisions for proofs that are no longer active. You can do this by adding the Approver Decision field to your report.

Prior to this change, after a decision was made on a proof, the decision could no longer be displayed in a Workfront report.

For more information, see&nbsp; [Glossary of Adobe Workfront terminology](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Proofing Enhancements in Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Create a New Version of a Proof Directly from the proofing viewer (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof) 
* [New Proof Details Link in the proofing viewer and Desktop Proofing Viewer (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Create a New Version of a Proof Directly from the proofing viewer (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

You can now create a new version of a proof directly from the new proofing viewer and the Desktop Proofing Viewer when proofing within Workfront Proof.

Previously, this option was available only within the Legacy Flash Viewer.

For more information, see [Copying Proofs in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) in the article&nbsp; [Copying Proofs in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### New Proof Details Link in the proofing viewer and Desktop Proofing Viewer (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

When viewing a proof in the proofing viewer, Workfront Proof users can now quickly Go to the proof details page within Workfront Proof.

For more information, see "Viewing Proof Details."
