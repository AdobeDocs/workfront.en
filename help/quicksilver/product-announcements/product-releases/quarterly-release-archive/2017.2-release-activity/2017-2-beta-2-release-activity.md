---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 2 release activity
description: This page describes all changes available in the Preview environment with the 2017.2 Beta 2 release. The functionality on this page was made available in the Preview environment on May 24, 2017. It will be made available in the Production environment between late July and early August, 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
---
# 2017.2 Beta 2 release activity

This page describes all changes available in the Preview environment with the 2017.2&nbsp;Beta 2 release. The functionality on this page was made available in the Preview environment on May 24, 2017. It will be made available in&nbsp;the Production environment between late&nbsp;July and early August,&nbsp;2017.

>[!IMPORTANT]
>
>Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2017.2, see [2017.2 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

The 2017.2 Beta 2 release contains enhancements both for Workfront administrators and other users:

**For Administrators:**

* [API Enhancement: Event Subscriptions](#api-enhancement-event-subscriptions)

**For All Users:**

* [Subscribe to Projects](#subscribe-to-projects) 
* [Unsubscribe from Items from Email](#unsubscribe-from-items-from-email) 
* [Configure How Milestones Are Displayed on the Gantt Chart](#configure-how-milestones-are-displayed-on-the-gantt-chart) 
* [Resource Pools Templates](#resource-pools-templates) 
* [View Versions of Proofed Documents within Workfront](#view-versions-of-proofed-documents-within-workfront) 
* [New Requester Object in Proof Approval Report](#new-requester-object-in-proof-approval-report)

## API Enhancement: Event Subscriptions {#api-enhancement-event-subscriptions}

When an action occurs on a Workfront object that is supported by event subscriptions, you can now configure Workfront to send a response to your desired endpoint. This means your integrations can interact with the Workfront API in real time.

For more information, see [Event Subscription API](../../../../wf-api/general/event-subs-api.md).&nbsp;

## Subscribe to Projects {#subscribe-to-projects}

You&nbsp;can now subscribe to new comments on projects for which you are not part of the project team. Prior to this release, you could only subscribe to comments on issues and tasks.

For more information about subscribing to items, see [Subscribe to items in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Unsubscribe from Items from Email {#unsubscribe-from-items-from-email}

You can unsubscribe from items using the “Unsubscribe” link inside the subscription email. Previously, you could only unsubscribe from an item from the Workfront interface.

For more information about unsubscribing to subscription emails, see the “Opting out of Email Notification” section in [Adobe Workfront notifications](../../../../workfront-basics/using-notifications/wf-notifications.md)&nbsp;

## Configure How Milestones Are Displayed on the Gantt Chart {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORRECTION**: This feature is not currently in the Preview Sandbox environment. It is planned to&nbsp;be released at a later date, during the month of June 2017.*

There are now two options for viewing milestone information in a Gantt chart. You can configure either or both&nbsp;of the following milestone indicators:

* Milestone Diamonds (icon)

  This icon displays in the Gantt chart after any task that is associated with a milestone. 

* Milestone Lines

  A line displays after any task associated with the milestone, across all tasks in the Gantt chart.

Prior to this change, there was only one option to enable&nbsp;Milestones to display on a Gantt chart, called "Milestones." This option enabled&nbsp;both the milestone diamond icon and the milestone line. These indicators could not be separated. The two options are now available on all Gantt charts,&nbsp;including all project lists and reports.&nbsp;

For more information about configuring how information displays in the Gantt chart, see [Configure how information displays on the Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Resource Pools Templates {#resource-pools-templates}

You can now specify Resource Pools for templates. Prior to this release, you could associate Resource Pools only with users and projects.

For more information about Resource Pools, see [Resource pools overview](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## View Versions of Proofed Documents within Workfront {#view-versions-of-proofed-documents-within-workfront}

You can now view proofs from all versions of a proofed document within the Workfront interface.&nbsp;

Prior to this change, you could view only the latest version of the proofed document.

Users without a proofing license can:

* Open a proof on a previous version of a proofed document

Users with a proofing license can do any&nbsp;of the following:

* Open a proof on a previous version of a proofed document
* View the proof details on a previous version of a proofed document

For more information, see [Manage document versions](../../../../documents/managing-documents/manage-document-versions.md) in [Manage document versions](../../../../documents/managing-documents/manage-document-versions.md).

## New Requester Object in Proof Approval Report {#new-requester-object-in-proof-approval-report}

Now when creating a Proof Approval report, there is a new Requester object. This object enables you to report on information regarding the user who requested&nbsp;the proof approval.&nbsp;

The new Requester object in the Proof Approval report contains all of the fields available with the existing User object in other types of object reports.

>[!NOTE]
>
>&nbsp;This information is available in the report only from the time this feature was first introduced to the respective Preview or Production environments; information in reports regarding&nbsp;the Requester object prior to the time this functionality was introduced&nbsp;is not available.

You access the Requester object when creating a Proof Approval report,&nbsp;as described in [Create a custom report](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

For more information about the Proof Approvals object report, see the [Understand objects in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) section in [Understand objects in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
