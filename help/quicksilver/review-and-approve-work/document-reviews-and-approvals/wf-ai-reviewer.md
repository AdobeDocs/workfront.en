---
product-area: documents
navigation-topic: approvals
title: Get started with the Workfront Content Reviewer
description: Workfront Content Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
---
# Get started with the Workfront Content Reviewer

Content Reviewer is an AI Collaborator—a type of AI agent that can be added to your projects, tasks and documents. AI Collaborators can be configured in the Setup area and assigned just like users.

In Workfront, Content Reviewer helps increase content velocity and improve brand compliance throughout the review and approval process. You can add Content Reviewers to approval templates or include them in individual review and approval requests.

## Access requirements

To set up Content Reviewers in Workfront, you must be a system administrator. 

Any user can add the Content Reviewer to a review and approval request.

## Requirements 

* Your Workfront instance must have Unified Approvals enabled. 
* Your organization must have GenStudio Foundation.
     * Content Reviewer in Workfront provides the functionality available in GenStudio Foundations for asset review and approval workflows.  You do not need to access GenStudio Foundations directly to complete your work. Your access to GenStudio Foundations functionality through Content Reviewer falls under the terms of your Workfront contract.
* Adobe must have a signed Adobe Gen AI agreement on file.
    For more information on signing the agreement, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Supported file types {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Unsupported file type"
>abstract="This Content Reviewer doesn't support the selected file type. Upload a supported file type, or remove the Content Reviewer to submit the request."

The Content Reviewer can review the following file types:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* Non-animated GIF (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

If you upload an unsupported file type, the Content Reviewer option will not be available when creating an approval workflow. 

## Set up brand guidelines

The Workfront Content Reviewer uses the brand guidelines when reviewing your content. Workfront administrators can set up brand guidelines in the Workfront Setup area. Brands created in GenStudio Foundation are also available in Workfront.

To set up brand guidelines, system administrators must

1. [Grant access to brand permissions](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Create and manage brands for the Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Create Content Reviewers

Once there is at least one brand set up, Workfront administrators can begin creating Content Reviewers in the Setup area. You can create muultiple Content Reviewers focused on different guidelines:

* **Image**: This Content Reviewer will review the asset against the image brand guidelines you set up in Workfront. [!BADGE Beta]{type=Positive tooltip="This feature is currently in beta."}
* **Brand voice**: The Content Reviewer will review the asset against brand voice guidelines you set up in Workfront.

Content Reviewers can then be assigned to approval templates and individual review and approval requests.

For more information, see [Configure AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Add Content Reviewers to review and approval requests

Users can add Content Reviewers to an existing approval templates or to individual review and approval requests. 

### Approval templates

If your organization often adds the same people to review and approval requests, Standard license users can create approval templates in the Workfront Setup area.

Users can add Content Reviewers to approval templates to automatically check for brand compliance when a template is used to create a request. 

Once created, approval templates can be applied to assets in the Documents area of a project, task, or issue.

For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![template list showing AI reviewwers](assets/ai-review-templates.png)

### Individual review and approval request 

When users create individual review and approval requests, they can add a Content Reviewer in with other participants or they can create a single request with only the Content Reviewer to check for brand compliance. 

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Content reviewer added to individual approval request](assets/new-stage.png)

## View Content Reviewer score and feedback 

Seconds after the review and approval request with a Content Reviewer is submitted, the score and feedback from the Content Reviewer is available in the Document Summary panel--even if other participants are still reviewing and making decisions. 

Approval owners also receive an email notifying them that a review has been completed on the asset. From the email, click **Go to review** and see the score and feedback in Workfront. 

The Content Reviewer is not designed to be a decision-maker in the review and approval workflow. It only provides a score and recommendations to align the asset with the specified brand requirements. 

If the asset does not meet brand guidelines, the creative can upload a new version and the approval owner can create a second review and approval request with the Content Reviewer.

For more information on viewing scores and feedback, see [View Content Reviewer score and feedback](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).


![Content reviewer feedback](assets/ai-reviewer-output.png)