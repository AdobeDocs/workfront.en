---
title: Fourth Quarter 2026 Documents enhancements
description: Fourth Quarter 2026 Documents enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Fourth Quarter 2026 Documents enhancements

This page describes Documents enhancements made with the Fourth Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Fourth Quarter 2026 release cycle, see [Fourth Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Control who can see and use approval templates

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Approval templates are now private by default. Previously, every approval requester could see every template in the system, which made template lists long and hard to navigate. Now, a template is visible only to the user who created it, unless the creator shares it.

Template creators can share a template with specific users or with everyone in their organization from the Approval Templates list in Workfront Setup. When requesting an approval, users only see templates they created or that were shared with them.

This change applies to both new and existing templates, and access is enforced consistently no matter how a template is requested.

For more information, see:

* [Share a template](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md#share-a-template) in Create an approval workflow template for documents
* [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

<!--

## Add teams to approvals for objects using Adobe cloud storage

>[!NOTE]
>
>Preview: August 27, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now add a Workfront Team as an approver or reviewer on a document approval or approval template, instead of adding each person individually:

* Objects on Adobe cloud storage: Workfront adds each active team member individually, so the approver list always reflects who's currently on the team.
* Objects using legacy Workfront storage: The team is added as a single participant by default, but you can now choose to add each team member as an individual participant.
* In approval templates, Workfront stores a reference to the team and expands it into active members when you apply the template to a document, not when you save the template.

For more information, see:

* [Create an approval workflow in the new Documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area) in Create a document approval workflow
* [Create an approval workflow in the legacy documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area) in Create a document approval workflow
* [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

-->

## Attach images to comments on Adobe cloud storage objects

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: July 30, 2026
>Production for everyone: July 30, 2026
>[!BADGE Off schedule]{type=Neutral}

Organizations using Adobe cloud storage as part of Unified review and approval can now attach image files directly to comments, keeping feedback, context, and supporting visuals together in a single, traceable comment thread. This closes a previous gap where only organizations on legacy Workfront storage could attach images to comments.

All media type image formats are now supported for Adobe cloud storage organizations. (Legacy object comments continue to support .jpg, .gif, and .png files only.) Non-image files are not supported on comments for either legacy or Adobe cloud storage objects.

For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Link assets from Experience Manager Assets with Adobe cloud storage

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, you can link individual assets from Experience Manager Assets to any Workfront object that supports documents. Linked content stays in sync automatically: changes made in Experience Manager Assets appear in Workfront, and you can pull in new asset versions without leaving Workfront.

Linking is powered by Content Advisor, so you also get AI Search, smart suggestions, campaign brief analysis and more while selecting content.

For more information, see [Link content from Experience Manager Assets with Adobe cloud storage](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md).
