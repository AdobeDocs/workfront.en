---
product-area: documents
navigation-topic: approvals
title: Get started with unified review and approval
description: Learn more about unified review and approval powered by Workfront and Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 10962d59-284e-4c41-8523-18ea4ed78362
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
---
# Get started with unified review and approval

Unified review and approval brings together Adobe Workfront and Adobe Frame.io into a single, deeply connected experience --- closing the gaps between marketing management, creative review, and content delivery. Project coordinators manage work in Workfront while creatives, marketers, and stakeholders review and approve assets in the professional-grade Frame.io viewer, all without moving files between disconnected tools.

For more information about Frame.io, see [Getting Started with Frame.io](https://support.frame.io/en/collections/49298-getting-started).


## Overview video

>[!VIDEO](https://video.tv.adobe.com/v/3471078)

## Access requirements

* You must be on a version of Workfront that supports Adobe cloud storage. If your organization is not already on a supported version, contact your Adobe account representative.

## Work initiation and planning in Workfront

Project coordinators can create projects and plan work in Workfront. Projects created in an instance with the Frame.io integration enabled utilize Adobe cloud storage, which allows assets to be stored and managed within the Adobe ecosystem.

If your organization has a Frame.io Enterprise license, projects created in Workfront are also visible in Frame.io, allowing users to interact and upload assets in either product. In Frame.io, all Workfront-linked projects are grouped into a single Workspace called **Workfront Linked Projects**. For details on how linked projects appear and behave in Frame.io, see [Adobe Workfront Integration Overview](https://help.frame.io/en/articles/12242607-adobe-workfront-integration-overview) in the Frame.io documentation.

For information about Adobe cloud storage or projects in Frame.io, see

* [Workspace Overview: Projects](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Review and approve assets

Once an asset is finished, the project coordinator can initiate the formal review and approval process in Workfront.

After the approval workflow is created, reviewers and approvers can use the Frame.io viewer to add comments and mark up the asset. They can also make the approval decision in the Frame.io viewer.

For more information about setting up projects, see 

* [Create a project](/help/quicksilver/manage-work/projects/create-projects/create-project.md)

### Initiate formal reviews and approvals in Workfront

Project coordinators can create one-time review and approvals or reusable approval templates. They can assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the asset to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

#### Create a review and approval workflow

Reviewers and approvers can be added to a single-use approval workflow or a reusable approval template:

* **Single-use approvals**: In the project or task where the asset resides, the project coordinator can assign reviewers and approvers and set a completion deadline. Reviewers and approvers are reminded by email 72 hours before the deadline, 24 hours before the deadline, and then on the deadline itself. You can also configure multi-stage approvals and parallel paths so that multiple review tracks run at the same time.

    For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-from-the-summary-panel-in-the-new-document-area).

* **Approval templates**: In the Workfront Setup area, project coordinators can create reusable Approval Templates. Within a template, users can add reviewers and approvers and specify a completion timeframe. When the approval template is applied to an asset, the deadline is calculated from the specified timeframe. Approval templates support multi-stage approvals and parallel paths, matching the configuration options available in single-use approvals.

    Once a template is created, it can be applied to an asset to begin the formal review and approval process in Workfront.

    For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

### Review and approve assets in the Frame.io viewer

Once the review and approval workflow is initiated in Workfront, reviewers and approvers can access the Frame.io viewer to add comments, mark up the asset, and make a decision. 

For more information, see [Review and approve with the Frame.io viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md).

#### Access the Frame.io viewer

Users can access the Frame.io viewer in the following ways:

* Workfront email notifications
* The My approval widget in the Workfront Home area

>[!NOTE]
>
>External Workfront users are notified via email and will be asked to create a Frame.io login to review and approve assets.

![open the frame viewer from Home](assets/open-fio-viewwer.png)

#### Add comments and mark up assets

Comments and asset markup is visible in the Frame.io viewer. For more information on using the Frame.io viewer, see [Commenting on your media](https://help.frame.io/en/articles/9105251-commenting-on-your-media).

#### Make a decision

Once all review activity is complete, approvers must make one of the following decisions:

* **Approve**: The asset does not need changes and is ready for use.
* **Approved with changes**: The asset is mostly complete but needs minor changes before it can be used. Once the specified changes are made, the asset is ready and does not need to go through another round of approvals. 
* **Needs work**: The asset needs changes and is not ready for use. Once the specified changes are made, the asset must be uploaded as a new version and go through another round of approvals. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Reviewers can mark their review complete inside of Workfront, but this is not required for the asset to move forward in the approval process. 

For more information about decisions in Workfront, see [Document decision status overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md). 

![Frame viewer and decision](assets/decision-fio.png)


### Track review and approval metrics

Project coordinators can monitor progress on all in-flight approvals in the Workfront Home area or with customized reports in Canvas Dashboards:

* **Custom dashboard**: Create a report dashboard in the Canvas Dashboards area to display both high-level and detailed information about reviews and approvals with Unified Approvals functionality. For information on how to get started, see [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Document approval metrics Home widget**: Displays 2 charts with information about average approval time and decisions as well as list views of pending and overdue approvals.
    ![All approvals](assets/all-approvals.png)

## Send finished assets to Adobe Experience Manager

You can use the [!DNL Experience Manager Assets]​​ to manage and store your digital assets that have gone through the review and approval cycle. This integration allows you to leverage the capabilities of Adobe Experience Manager, Frame.io, and Workfront to streamline your content management and collaboration processes.

For more information, see [Use the Adobe Experience Manager with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

