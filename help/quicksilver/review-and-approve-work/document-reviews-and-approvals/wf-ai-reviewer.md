---
product-area: documents
navigation-topic: approvals
title: Get started with the Workfront AI Reviewer
description: Workfront AI Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: yes
hidefromtoc: yes
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
---
# Get started with the Workfront AI Reviewer

Increase content velocity and optimize brand compliance with AI Reviewers. You can add AI reviewers to approval templates or ad-hoc approvals in Workfront. 


<!--## Access requirements

Set up:

Add and use: -->


## Prerequisites 

* Your organization must have migrated to Adobe IMS (Identity Management System)
* Your Workfront instance must have Unified Approvals enabled 
* Adobe must have a signed Adobe Gen AI agreement on file
    For more information on signing the agreement, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Supported file types {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Unsupported file type"
>abstract="This AI reviewer doesn't support the selected file type. Upload a supported file type, or remove the AI reviewer to submit the request."

The AI Reviewer is able to review the following file types:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* Non-animated GIF (.gif)

## Set up brand guidelines

The Workfront AI Reviewer uses the brand guildelines set up in Genstudio for Performance Marketing when reviewing your content. 

To learn more about brand guildelines, see

* [GenStudio for Performance Marketing Brands](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/guidelines/brands)
* [Add guidelines](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/guidelines/add-guidelines)


## Set up AI Reviewers

Once you have at least one brand set up in GenStudio for Peformance Marketing, you can create multiple AI Reviewers, which you can then assign to approval templates and ad-hoc approval workflows. 

For more information, see [Set up AI Reviewers](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/set-up-ai-reviewer.md).

## Add AI reviewers to approval workflows

You can add AI reviewers to a existing approval workflow templates or to an individual review and approval request. 

### Approval Templates

If you often add the same people to approval requests, you can createa an approval template in the Workfront Setup area.  

Now, you can add AI reviewers to approval templates to automaticlly check for brand compliance when a template is used to create a request. 

Once created, Approval Templates can be applied to assets in the Documents area of a project, task, or issue.

For more information, see [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

![template list showing AI reviewwers](assets/ai-review-templates.png)

### Individual review and approval request 

If you create individual review and approval requests, you can add AI Reviewers as you create the request. For more information, see [Create a document review or approval request](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)


![AI reviewer added to individual approval request](assets/ad-ai-reviewer-to-request.png)

## View AI Reviewer score and feedback 

Seconds after you submit the approval request, you can view the score and feedback from the AI Reviewer in the Document Summary panel. 

You'll also receive an email notifying you that a review has been completed on the asset. You can click **Go to review** and see the score and feedback in Workfront. 

The AI Reviewer does not produce an approval or rejection. It only provides a score and recommendations to align the asset with the specified brand requiremets. 

if you need to update the image because it does not pass the brand check, you can upload as a new version. 

For more information on viewing scores and feedback, see [View AI Reviewer score and feedbak](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).


![AI reviewer feedback](assets/ai-reviewer-feedback.png)


