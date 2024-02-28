---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 3 release activity
description: This page describes all changes available in the Preview environment with the 2017.2 Beta 2 release. The functionality on this page was made available in the Preview environment on May 24, 2017. It will be made available in the Production environment between late July and early August, 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
---
# 2017.2 Beta 3 release activity

This page describes all changes available in the Preview environment with the 2017.2&nbsp;Beta 2 release. The functionality on this page was made available in the Preview environment on May 24, 2017. It will be made available in&nbsp;the Production environment between late&nbsp;July and early August,&nbsp;2017.

>[!IMPORTANT]
>
>Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2017.2, see [2017.2 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

The 2017.2 Beta 2 release contains enhancements both for Workfront administrators and other users:

**For Administrators:**

* [Restoring Items in Bulk from the Recycle Bin](#restoring-items-in-bulk-from-the-recycle-bin) 
* [User Information Is Synchronized from Workfront to ProofHQ (ProofHQ and Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**For All Users:**&nbsp;

* [View Subscribed Users](#view-subscribed-users) 
* [Configure How Milestones Are Displayed on the Gantt Chart](#configure-how-milestones-are-displayed-on-the-gantt-chart) 
* [Include the Gantt Chart Legend When Exporting to PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf) 
* [View Proof Approvals in the My Work Area (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront) 
* [View User Names when Addressing Proofing Approval Requests from the My Work Area (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront) 
* [Improved proofing viewer for Video Proofs (ProofHQ and Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront) 
* [View Rich Media Proofs in Alternate Resolutions (ProofHQ and Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront) 
* [New 'Proof Creator' Object in Document Version Report (Workfront)](#new-proof-creator-object-in-document-version-report-workfront) 
* [New Resource Pool Functionality Temporarily Removed from Preview](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Restoring Items&nbsp;in Bulk from the Recycle Bin {#restoring-items-in-bulk-from-the-recycle-bin}

You can now restore up to 10 deleted projects, tasks, issues, or&nbsp;documents at a time.

Prior to this change, you could restore only one deleted item at a time.

For more information about restoring items, see [Restore deleted items](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## View Subscribed Users {#view-subscribed-users}

You can now see who subscribes to an item by expanding the number of subscribers which displays next to the subscription link.

Prior to this enhancement, you had no visibility into who is subscribed to any items.

For more information about subscribing to items, see [Subscribe to items in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).&nbsp;

## Configure How Milestones Are Displayed on the Gantt Chart {#configure-how-milestones-are-displayed-on-the-gantt-chart}

There are now two options for viewing milestone information in a Gantt chart. You can configure either or both&nbsp;of the following milestone indicators:

* Milestone Diamonds (icon)

  This icon displays in the Gantt chart after any task that is associated with a milestone.

* Milestone Lines

  A line displays after any task associated with the milestone, spanning all tasks in the Gantt chart.

Prior to this change, there was only one option to enable&nbsp;Milestones to display on a Gantt chart, called "Milestones." This option enabled&nbsp;both the milestone diamond icon and the milestone line. These indicators could not be separated.

For more information about configuring how information displays in the Gantt chart, see [Configure how information displays on the Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Include&nbsp;the Gantt Chart Legend When Exporting to PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

When you export the Gantt chart to a PDF, you can now select whether you want to also export the legend of the chart along with the chart itself. The items included in the legend are only those options you have enabled to be displayed in the Gantt chart in the UI. These options are included in the legend if they exist on the tasks on the project. For example, if you enable to show Milestones in the Gantt chart, the legend displays them as well, but only if there is at least one task associated with a milestone.

Prior to this change, you could not exclude the legend from the exported PDF, and the legend included all possible options and markers of the Gantt, regardless whether they were enabled or existed in the UI.

For more information about exporting the Gantt chart, see [Export the Gantt Chart to PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## User Information Is&nbsp;Synchronized from&nbsp;Workfront to&nbsp;ProofHQ (ProofHQ and Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

User information (name and email) is now synchronized from Workfront to ProofHQ when users are created or updated in Workfront.&nbsp;

For more information about user synchronization from Workfront to ProofHQ&nbsp;, see .

## New 'Proof Creator'&nbsp;Object in Document Version&nbsp;Report (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Now when creating a Document Version&nbsp;report, there is a new Proof Creator&nbsp;object. This object enables you to report on information regarding the user who created the proof.&nbsp;

The new Proof Creator&nbsp;object in the Document Version&nbsp;report contains all of the fields available with the existing User object in other types of object reports.

>[!NOTE]
>
>&nbsp;This information is available in the report only from the time this feature was first introduced to the respective Preview or Production environments; information in reports regarding&nbsp;the Requester object prior to the time this functionality was introduced&nbsp;is not available.

You access the Proof Creator&nbsp;object when creating a Document Version&nbsp;report,&nbsp;as described in [Create a custom report](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

For more information about the Document Version&nbsp;object report, see the [Understand objects in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) section in [Understand objects in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## View Proof Approvals in the My Work Area (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

All proof approvals you have submitted for approval are now displayed in the My Work area, in the **Work I've Submitted for Approval** tab.

Prior to this change, the **Work I've Submitted for Approval** tab did not include proof approvals.

Proof approvals are displayed only when the following criteria are met:

* The approval is currently Pending Approval
* The approval process is assigned to a user who is a licensed Workfront user (Approval processes that are assigned to users who are not licensed Workfront users are not displayed)
* The approval processes was instigated after this functionality was released (Approval processes that were instigated prior to this functionality being released are not displayed)

For more information, see [View approvals](../../../../review-and-approve-work/manage-approvals/view-approvals.md) in [View approvals](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## View User Names when Addressing Proofing Approval Requests from&nbsp;the My Work Area (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Now when approving proofing approvals from the My Work area, the name of the user who requested the approval is now displayed.

For more information, see [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md).&nbsp;

## Improved proofing viewer for Video Proofs (ProofHQ and Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

The proofing viewer in both Workfront and&nbsp;ProofHQ is being updated&nbsp;with a new look and feel,&nbsp;HTML5 architecture for better performance, and support for new functionality.

The new proofing viewer contains the following improvements:

* Frame-by-frame proofing
* Video buffering
* Search functionality in the Comment List
* Any actions set on the comment are displayed on each comment in the Comment List
* Full-screen mode
* Review content faster or slower
* Spell checker when adding comments and replies

### Preview

The new proofing viewer is available to test in the following Preview environments:

* ProofHQ Preview environment

  For more information about the ProofHQ Preview environment, see [Preview Sandbox Testing Environment- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Workfront Preview environment, when your account is enabled with proofing

  For more information about the Workfront Preview environment, see&nbsp; [The Adobe Workfront Preview Sandbox Environment](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

In this release, the new proofing viewer supports only video proofing. This means that all video proofs leverage the new proofing viewer, while all static and rich media proofs continue to leverage the existing proofing viewer.

### Production

When released to the Production environment with the 17.2 release, administrators&nbsp;can choose whether the new or legacy proofing viewer is right for the users in their organization. By default, the legacy proofing viewer will be&nbsp;used.

For information about how to use the new video proofing viewer, see&nbsp;&nbsp;

## View Rich Media Proofs in Alternate Resolutions (ProofHQ and Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

You can now adjust the resolution of Rich Media proofs either by specifying a custom resolution, or by dragging the image to the desired resolution.

Prior to this change, you could review&nbsp;proofs using only&nbsp;the&nbsp;resolution inherent to the screen or device where you were reviewing the content.

You can use Compare mode to compare different resolutions of proofs.

For more information, see [Open proofs in the Desktop Proofing Viewer](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md).&nbsp;

## New Resource Pool Functionality Temporarily Removed from Preview {#new-resource-pool-functionality-temporarily-removed-from-preview}

Due to development challenges, we have decided to remove the new Resource Planning tab and rename the Legacy Resource Planning tab back to its original name of “Resource Planning.”

The new Resource Pools functionality has also been removed with this change. The new tab of Resource Planning and the functionality of the Resource Pools will return to the Preview Sandbox environment at the end of June, 2017.
