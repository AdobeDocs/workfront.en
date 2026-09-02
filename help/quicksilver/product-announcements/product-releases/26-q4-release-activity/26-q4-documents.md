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

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

## Direct proof access from approval email links

>[!NOTE]
>
>Preview: N/A
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When a document has a proof attached, the "Go to review" link in approval emails now opens the proof viewer directly, so reviewers and approvers can start their review right away. If a document has no proof, the link continues to open the Approvals section of the document, as before.

## Add teams to approvals for objects using Adobe cloud storage

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now add a Workfront Team as an approver or reviewer on a document approval or approval template, instead of adding each person individually:

* Objects on Adobe cloud storage: Workfront adds each active team member individually, so the approver list always reflects who's currently on the team.
* Objects using legacy Workfront storage: The team is added as a single participant by default, but you can now choose to add each team member as an individual participant.
* In approval templates, Workfront stores a reference to the team and expands it into active members when you apply the template to a document, not when you save the template.

For more information, see:

* [Create an approval workflow in the new Documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Create an approval workflow in the legacy documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

## Set a Frame.io workspace on project templates

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage and you have a Frame.io Enterprise license, you can now choose a Frame.io workspace in the Project Details on a project template. Projects created from the template automatically use the workspace set on the template, so projects are routed to the desired Frame.io workspace with no extra action needed at project creation.

The new field lists the Frame.io workspaces you have permission to assign projects to. The field remains editable on the template at any time; changes apply only to projects created after the update, so existing projects keep their original workspace.

Once a project is created from the template, its Frame.io workspace field is read-only and links to the workspace in Frame.io.

If you do not have a Frame.io enterprise license, projects continue to go to the default workspace for Workfront.

For more information, see [Edit project templates](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) and [Manage information in the project Overview area](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md).

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

## Custom message in email subject line

>[!NOTE]
>
>Preview: N/A
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When you set a custom message on a document approval, that message now also appears in the subject line of the approval-request email, led by the due date when one is set. This lets reviewers see what needs attention and by when directly from their inbox, without opening the email.

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Redesigned Versions panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Versions panel in the new Documents area has a new design:

* Versions are labeled V1, V2, and so on to drive consistency with Frame.io.
* Each version shows its approval status, such as "Approved" or "Withdrawn", directly in the list.
* The panel now lists only Version history — there's no longer a separate "latest file" entry at the top.

Previously, versions were timestamped instead of numbered.

For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Redesigned Approvals panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Approvals panel in the new Documents area now shows approval history across versions:

* The panel lists the approval workflow for every version that has one, not just the current version.
* Withdrawn workflows stay in the list, so you can still review their prior decisions.
* Expand any version to see its stages, approver decisions, decision rule, and due dates without leaving the panel.

Previously, the Approvals panel only showed the current version's workflow.

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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
