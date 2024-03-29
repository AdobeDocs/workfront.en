---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta Final
description: This page describes all changes most recently available in the Preview environment with the 2017.2 release. The functionality on this page was made available in the Preview environment on June 28, 2017. It will be made available in the Production environment on July 26, 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
---
# 2017.2 Beta Final

This page describes all changes most recently available in the Preview environment with the 2017.2 release. The functionality on this page was made available in the Preview environment on June 28, 2017. It will be made available in&nbsp;the Production environment on July 26,&nbsp;2017.

>[!IMPORTANT]
>
>Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2017.2, see [2017.2 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

The 2017.2 Beta Final release contains enhancements both for Workfront administrators and other users:

**For Administrators:**

* [Determine the Availability of the HTML5 Video proofing viewer (ProofHQ and Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront) 
* [Support SHA-256 certificates for SAML 2.0](#support-sha-256-certificates-for-saml-2-0) 
* [Type-Ahead for Mapping Attributes](#type-ahead-for-mapping-attributes) 
* [API Enhancement: Access User Allocations](#api-enhancement-access-user-allocations)

**For All Users:**

* [Resource Planner](#resource-planner) 
* [New Scheduling Area in a Project (Team Builder)](#new-scheduling-area-in-a-project-team-builder) 
* [Resource Scheduling: Show Fewer Items by Default](#resource-scheduling-show-fewer-items-by-default) 
* [Resource Scheduling: Display Drop Indicator and Over-Allocation When Dragging Tasks and Issues](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues) 
* [Resource Scheduling: User Allocations Are No Longer Rounded to the Nearest Half Hour](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour) 
* [Export the Utilization Report in TSV and PDF Formats](#export-the-utilization-report-in-tsv-and-pdf-formats) 
* [2017.2 Beta Final](#user-calendar-enhancements-in-the-my-work-area%22) 
* [2017.2 Beta Final](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area) 
* [Proof Decision Displays in the My Work Area (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront) 
* [View Rich Media Proofs in Preset Resolutions (ProofHQ and Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront) 
* [View URL to Sub-Pages in Comments on Rich Media Proofs (ProofHQ and Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront) 
* [Create Custom Views Based on Existing Standard Views (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq) 
* [Filter the Reporting Area (ProofHQ)](#filter-the-reporting-area-proofhq) 
* [Display Minimum and Maximum Values in Reports (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq) 
* [In-App Notification for Proof Approval](#in-app-notification-for-proof-approval) 
* [Mobile Improvements](#mobile-improvements) 
* [Slash Added to Filter Statements for Field Values that Contain Commas](#slash-added-to-filter-statements-for-field-values-that-contain-commas) 
* [Multiple Billing Rates](#multiple-billing-rates) 
* [New Resource Budgeted Hour Field](#new-resource-budgeted-hour-field) 
* [Show User Job Role in 'Assigned To' Area on the Details Page for Tasks and Issues](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>The Resource Scheduling tools have been deprecated and removed from Workfront with the 23.1 release. For information about scheduling resources using the Workload Balancer, see [Overview of the Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## New Scheduling Area in a Project (Team Builder) {#new-scheduling-area-in-a-project-team-builder}

The Scheduling area in a project (formerly known as Team Builder) has been redesigned with an updated and&nbsp;more intuitive user interface. The new Scheduling functionality now more closely matches&nbsp;the Resource Scheduling functionality currently&nbsp;available in other areas of Workfront.

Improvements include:

* View current resource allocations for members of the project team, allowing you to make more informed decisions when making assignments
* Visual representation of task durations on the scheduling timeline
* Filter the&nbsp;information displayed on the scheduling timeline
* Easily add and remove users from the project team, directly from the scheduling timeline

The following functionality is available in other areas of the tool when scheduling resources, but is not available when scheduling resources in the Team Scheduling area:

* Configure parent tasks to display on the scheduling timeline
* Configure project names&nbsp;to display on the scheduling timeline
* Modify user assignments by using the Swap tool
* Filter by portfolio, programs, and projects

For more information about functionality available in the Team Scheduling area, see "Get started with Resource Scheduling".

## Resource Scheduling: Show Fewer Items&nbsp;by Default {#resource-scheduling-show-fewer-items-by-default}

By default, a maximum of 10 work items per day are now displayed on the scheduling timeline for a given user. You can expand the list to view all tasks and issues currently assigned to that user.

This enables you to more easily browse the scheduling timeline when users are assigned many tasks and issues.

Prior to this change, all tasks and issues were always displayed for all users.

For more information about assigning tasks and issues to users on the scheduling timeline, see "Manually assign unassigned tasks and issues in the Scheduling areas".

## Resource Scheduling: Display Drop Indicator and Over-Allocation When Dragging Tasks and Issues {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

When assigning&nbsp;a task or issue to a user on the scheduling timeline via drag-and-drop,&nbsp;the following information is now displayed prior to releasing the task or issue and completing the assignment:

* A drop indicator is displayed in the row of the user. This enables&nbsp;you to see where an item is being assigned prior to making the assignment.
* If user allocations are enabled&nbsp;on the scheduling timeline, the red over-allocation indicators are displayed if completing the assignment will result in the user being over-allocated.

Prior to these changes, no information was displayed prior to releasing the task or issue.

For more information about assigning tasks and issues to users on the scheduling timeline, see "Manually assign unassigned tasks and issues in the Scheduling areas".

## Resource Scheduling: User Allocations Are No Longer Rounded to the Nearest Half Hour {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

When multiple users are assigned to a task or issue, or when a task or issue spans multiple days, Workfront&nbsp;attempts to distribute planned hours evenly among the assigned users and days. Hours are rounded to the nearest&nbsp;hundredth by default (for example, 1.33).

Previously, when you manually modified distributed hours, hours are adjusted and rounded to the nearest half hour (for example, 1.33 is rounded to 1.5).

Now, hours are no longer adjusted and rounded to the nearest half hour (for example, 1.33 remains 1.33).

## API Enhancement: Access User Allocations {#api-enhancement-access-user-allocations}

You can now access user allocation shading via the Workfront API.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Export the Utilization Report in TSV and PDF Formats {#export-the-utilization-report-in-tsv-and-pdf-formats}

You can now export the Utilization report on a project in TSV and PDF formats, in addition to the XLSX format.

Prior to this change, you could export the Utilization report only in XLSX format.

For more information about exporting the Utilization report, see [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Overview of the Resource Utilization report](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Proof Decision Displays in the My Work Area (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Now when viewing proofing approvals in the My Approvals tab in your My Work area, the proof decision is displayed in your My Work area and remains until you click the new Refresh button within Workfront or until the next time you refresh the browser page.

Prior to this change, there was no indication that a decision was already made on the proof, and the proof remained on the My Approvals tab&nbsp;until you refreshed the browser.

For more information, see [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## View Rich Media Proofs in Preset Resolutions (ProofHQ and Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

In an earlier release to the Preview environment, we introduced the ability to&nbsp;adjust the resolution of Rich Media proofs either by specifying a custom resolution, or by dragging the image to the desired resolution.

You can now select from preset resolution options of various phones, tablets, notebooks, and desktops.

For more information, see "Viewing a Preset Resolution" in [Change interactive proof resolution in the proofing viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md). 

## View URL to Sub-Pages in Comments on Rich Media Proofs (ProofHQ and Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>This feature is currently available in the Production environment.

Now when you comment on a sub-page in a Rich Media proof, the URL to the sub-page is displayed on the comment.

Prior to this change, it was not clear&nbsp;which sub-page the comment was referring to.

For more information, see

## Determine the Availability of the HTML5 Video proofing viewer (ProofHQ and Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

As the Workfront administrator in ProofHQ, you can determine whether users in your organization have access to the new HTML5 proofing viewer for video proofs.

For more information about configuring this option in Workfront, see in .

## Create Custom Views Based on Existing Standard Views (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Now you can create a custom view based on a standard view.&nbsp;Columns, Sorting, and Filters options from the standard view are included in the new view by default.

Prior to this change, in order to create a custom view, you had to create the view from scratch.&nbsp;

For more information, see [Creating a Custom View](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) in [Create and Manage Custom Views in Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filter the Reporting&nbsp;Area (ProofHQ) {#filter-the-reporting-area-proofhq}

By default, data displayed on the Reports tab includes all information from your ProofHQ system. You can now use filters to show only information that is relevant to your needs.&nbsp;

For more information, see [Filtering Reports](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) in&nbsp; [Run Reports in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Display Minimum and Maximum Values in Reports (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

You can now configure&nbsp;whether minimum and maximum values are displayed in the graph when viewing reports.

For more information, see [Viewing Reports](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) in&nbsp; [Run Reports in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Support SHA-256 certificates for SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

We now support&nbsp;Secure Hash Algorithm 256 (SHA-256) when configuring Workfront for SSO with SAML 2.0. Prior to this release, we supported only Secure Hash Algorithm 1 (SHA-1).

For more information about configuring Workfront with SAML 2.0, see [Configure Adobe Workfront with SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Type-Ahead for Mapping Attributes {#type-ahead-for-mapping-attributes}

The Default Value field type in the Attribute Mapping dialog box has been updated to a type-ahead field. Prior to this change, the type of the Default Value field was a dropdown.

This change applies for the following SSO protocols:

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 does not support Attribute Mapping.

## Mobile Improvements {#mobile-improvements}

>[!NOTE]
>
>&nbsp;The mobile application releases&nbsp;independently from the main Workfront application. The functionality described in this section releases in early August.

You will see the following added functionality on the mobile apps, for both the Android and the iOS platforms:

* Submit Requests from the mobile app
* Timesheet New Entry on the mobile app
* Custom Form Editing from the mobile app
* Proof Approval Requests on the mobile app

There will be a public beta program for some of these features for the Android platform.

For more information about the upcoming beta program for mobile, see the&nbsp; ["Betas"](https://support.workfront.com/hc/en-us/sections/115000743248) page.

For more information about using the Workfront mobile app, see .&nbsp;&nbsp;

## Slash Added to Filter Statements for Field Values that Contain Commas {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

When building a filter in text mode and filtering for field values that contain commas, you must add a slash ("/") before the commas separating the values, to ensure that the value is read as one filter option. This only applies for the following field types:

* Dropdowns
* Radio Buttons
* Checkboxes

Prior to this change, you could not filter for fields that had options that contained commas.

For more information about this change, see [Filters overview](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Multiple Billing Rates {#multiple-billing-rates}

You can now add multiple billing rate overrides for the same job role at the project level. With this new functionality, you can define date ranges for each billing rate override. During the date range specified, a different billing rate is applied to the job role assigned to tasks on a project. Billing rates are multiplied by hours on the project to calculate revenue. Revenue calculated within the date range of a billing rate stays locked at that rate and does not update as the rates of the job roles on the project update. In the case of Actual Revenue, no hours logged before overriding the billing rate will be recalculated to reflect the current billing rate. The hours logged before the billing rate override was added to the project will be associated with the billing rate of the job role at that time.

Prior to this change, you could override the billing rate of a job role only once, and Actual Revenue would recalculate to reflect the current billing rate for all the hours logged before the billing rate was changed.

For more information about Billing Rates and Revenue, see [Overview of Billing and Revenue](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

For more information about overriding billing rates for job roles at the project level, see [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Resource Planner {#resource-planner}

With this release, we are introducing the first phase of the Resource Planner, which is part of the redesign of the new Planning tab in the People area. By using the Resource Planner, you can budget the amount of hours the users in your Resource Pools are allocated in all the current projects for which you are the Resource Manager. You can see the following allocation numbers by project, job role, and by user, in the Resource Planner:

* Available Hours
* Planned Hours
* Budgeted Hours
* Hour Variance (between the Budgeted and the Planned Hours)
* Net Hour difference (between the Available and the Budgeted Hours)

For more information about using the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## New Resource Budgeted Hour Field {#new-resource-budgeted-hour-field}

To support the new Planning functionality and the Resource Planner, a new field has been added to the Report builder, that allows you to report on the Resource Budgeted Hours. This field captures the amount of hours that a resource is budgeted for in a project. This field is not available when budgeting resources using the Legacy Resource Planning functionality.

For more information about using Budgeted Hours in the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## In-App Notification for Proof Approval {#in-app-notification-for-proof-approval}

When you are designated as an approver for a proof, you receive an in-app notification about the proof approval waiting for your decision. The notification displays the following text: `<User name>` wants you to approve this proof". If the user information is not available, the notification changes to "This proof requires your approval."

Prior to this enhancement, the only visual indication that you were designated as an approver on a proof was a new proof request in your My Work area.

For more information about in-app notifications, see [View and manage in-app notifications](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Show User Job Role in 'Assigned To' Area on the Details Page for Tasks and Issues {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Now when viewing the details page of a task or issue, a&nbsp;job role is displayed below the assignee's name in the Assigned To area. This job role represents the job role of the user that matches the job role assignment of the task or issue. If the task or issue is not assigned to a job role, the primary job role of the assigned user is displayed.

Prior to this change, only the title of the user was displayed below the user's name in the Assigned To area.&nbsp;
