---
title: Third Quarter 2025 Proofing and document management enhancements
description: Third Quarter 2025 Proofing and document management enhancements
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4829d487-7041-447f-9a68-fb1acf467734
---
# Third Quarter 2025 Proofing and document management enhancements

This page describes all document management enhancements made with the Third Quarter 2025 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Third Quarter 2025 release cycle, see [Third Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## New Proofing and GenStudio for Performance Marketing integration

>[!NOTE]
>
>* Production release for all customers: June 12, 2025

We are excited to introduce a new integration between Proofing and GenStudio for Performance Marketing. With this integration, you can 

* Use Workfront approval templates to define approval workflows

* Review draft content in the Workfront proofing viewer

* See review decisions for final approval and publishing in GenStudio for Performance Marketing

### Integration requirements 

Workfront and GenStudio for Performance Marketing must be deployed to the same IMS Org.

For more information, see [Get started with the GenStudio for Performance Marketing and Workfront Proof integration](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md).

## Desktop Proofing Viewer Update

The Desktop Proofing Viewer has been updated to version 2.1.48.

This update is an issue fix to keep the Desktop Viewer compatible with Mac operating systems. Electron was downgraded to 34.4.0 and Chromium was downgraded to 132. 

This update is for both Mac and Windows. 


## Assets in a linked Google folder must be added individually to appear in Workfront

>[!NOTE]
>
>* Preview release: June 2, 2025; Production release for all customers: June 2, 2025

Google is [enhancing security controls](https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps) for third-party applications accessing Google Drive, requiring applications to adopt a per-user consent model. As a result, individual assets must be linked one at a time to be visible in Workfront. See [Configure document integrations](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md) for more information. 

Key capabilities that remain unchanged: 

* Search and filter for assets and folders from within the Google Drive modal
* Link assets to Workfront objects from Google Drive
* Upload assets to Google Drive through the "Send To" dropdown on the documents page
* View and access folder structure in a user's My Drive area
* Link a new version of an asset from Google Drive to an existing document in Workfront
* Link folders to Workfront objects from Google Drive
* Upload assets to Google Drive by dragging and dropping documents into a linked folder
* Create a new Google Drive document from within Workfront


## New document approval decision buttons available in proofing viewer

>[!IMPORTANT]
>
>This feature is part of a phased release and are only available for specific customers.

>[!NOTE]
>
>* Preview release: April 10, 2025; Production release for all customers: April 17, 2025

The new document approval decision buttons now appear in the proofing viewer. Now, when you create a simple proof and then add approvers and reviewers from the Document summary, they can make their decision directly inside the proofing viewer.

Previously, you had to exit the proofing viewer to make a decision.

Approvals created before this release will not display the buttons in proofing viewer.

For more information, see [Use new document approvals and proofing together](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md).
