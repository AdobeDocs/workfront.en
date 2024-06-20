---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Final
description: 2018.3 Release Activity
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
---
# R1 Final

The following functionality is not currently available in Preview or Beta, but is releasing to the Production environment in R1:

## Make Approval Decisions for Proofs from&nbsp;the My Work Area (Workfront)

Now when a user adds you to a proof and grants either the Approver role or the Reviewer & Approver role (either from the stand-alone ProofHQ application or by using Automated Workflow within Workfront ), the approval request is displayed on the Approvals tab in your&nbsp;My Work area. You can then view the proof and make an approval decision on the proof directly from Workfront.

For information about how to&nbsp;add users&nbsp;to a proof using Automated Workflow, see [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

For information about how to make approval decisions from the My Work area, see [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Approving work](../../../../review-and-approve-work/manage-approvals/approving-work.md).&nbsp;

## Report on Proofing Approvals within the My Work Area (Workfront)

You can now create a report based on the Proof Approval object. This report enables you to report on the proof approvals from&nbsp;users' My Work areas&nbsp;where decisions have not yet been made.

Proof approval reports contain the following information:

* Document that was submitted for approval
* Name of the approver
* Proof version
* Proof ID
* Proof creation date

You access this approval when creating a report based on an object, as described in [Create a custom report](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

For more information about the Proof Approvals object report, see the [Understand objects in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) section in [Understand objects in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Automatically Generate a New Version of a Document Proof Using Drag-and-Drop (Workfront)

When you use the drag-and-drop method to add a new version of a document that requires proofing, a proof is automatically generated. The proof has the same options and workflows as the original proof or previous version.

Previously, when you added a new version of the document, the proof was not automatically generated on the new version, and you had to re-generate the proof for the new version.

When you use the Documents More Menu to upload a new version, a proof is not automatically generated.

For more information, see the&nbsp;&nbsp;section in

## Enable All Proofing Users to Access ProofHQ Directly from the Workfront Interface (Workfront)

Now you can enable all proofing users in your system to have seamless access to your ProofHQ Premium account directly from the Workfront interface. When enabled, all proofing users see a ProofHQ icon in the Global Navigation Bar that directs them to the ProofHQ site.

This option is not enabled by default. To enable this option, contact Workfront Technical Support and request this access for all proofing users in your system.

For more information, see [Access Workfront Proof from Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)&nbsp;in&nbsp; [Access Workfront Proof from Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Prior to this change, only the Workfront administrator could have direct access to the ProofHQ site from the Workfront interface.

## New Option for TLS Secure Connection for Outgoing Mail (Workfront)

When you select to manage your Workfront communication using your own email server, you can now enable your Outgoing Mail to use a TLS secure connection.

Prior to this enhancement, you could enable Outgoing Mail only through an SSL secure connection.

For more information about configuring your Outgoing Mail, see .

## New Field for Managing Emails in the Preview Sandbox Environment

Workfront now disables all email communication from the Preview Sandbox environment and the Custom Refresh environment. If you want to receive email notifications from the Preview Sandbox or Custom Refresh environments, you must enable this functionality in your user settings.

For more information, see the following information:

* [The Adobe Workfront Preview Sandbox Environment](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) in [The Adobe Workfront Preview Sandbox Environment](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* "Receiving Emails from the Custom Refresh Sandbox" in [The Adobe Workfront Custom Refresh Sandbox environment](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook for Office 365 (Workfront)

The Workfront Add-In for Outlook 365 is now available.&nbsp;

For more information about using&nbsp;the add-in, see [Using the Workfront Add-In with Outlook for Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Search in the Mobile App (Workfront)

You can now&nbsp;search for objects inside the mobile app, similarly to the way you search in the web application. The new search functionality looks for items in the Recent Items list first, as well as the objects that have previously been downloaded to your mobile device. The list of Recent Items is the same list you see in the web application.

>[!NOTE]
>
>This functionality will be available the first week of May, 2017.

For more information about the mobile app, see the "Searching in Mobile" section in&nbsp;&nbsp;

## Improved Help in the Mobile App: Tutorials (Workfront)

Starting with the mobile release in April, you will see new tutorial screens to guide you through your mobile experience. When you log into the mobile app for the first time, and you are using a feature for the first time, you will see a brief tutorial that explains how the feature works. The tutorial displays only once, the first time you are using a specific feature.

For more information about the mobile app, see .

## Search in PDF Documents (ProofHQ)

You can now perform searches within PDF documents, office documents, and static web pages.

For more information, see&nbsp; [Search content within a proof](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Updated Global Navigation Bar (ProofHQ)

ProofHQ Premium accounts that are integrated with Workfront now see the following improvements to the Global Navigation Bar within ProofHQ:

* New user profile picture&nbsp;
* Updated look and feel

## Include Additional&nbsp;Information in Custom Views (ProofHQ)

You can now include the following additional information&nbsp;in custom views:

* **Recipient-Level Data**  
  You can configure custom views to include the following columns related to recipient-level data: Role, Position, Email Alerts, My Deadline, Date Added to Proof, and Recipient Search.  
  For more information, see [Create and Manage Custom Views in Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Proofing Data**  
  You can configure custom views to include the following columns related to proofing data: Comment Count (All Versions), Size on Disk, Proof Type, Number of Files per Version, Comment Attachment Data (size on disk, filename), and Filtering by Subfolder.  
  For more information, see [Create and Manage Custom Views in Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md). 
* **Stage-Level Data Related to&nbsp;Automated Workflows**  
  You can configure custom views to include the following columns related to individual stages of&nbsp;automated workflows: SOCD Status, Stage Deadlines, Active Stage Name, Next Stage Name, Stage name, and Template.  
  For more information, see [Create and Manage Custom Views in Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).  

## Improvements to Proofing Reports (Formerly Analytics) (ProofHQ)

The reporting feature (formerly known as Analytics) contains the following improvements:

* New default report types:

   * Proof turnaround time
   * Late approval percentage
   * Proof first activity time
   * Number of comments and replies

* Print reports
* Updated look and feel

## View ProofHQ Functionality in the Preview Environment (ProofHQ)

Functionality that is released to ProofHQ will first be available to test in the Preview environment prior to releasing to the Production environment.

This new workflow of releasing functionality to Preview prior to Production will allow you to be more prepared for future updates to your ProofHQ Production environment.

For more information about the ProofHQ Preview environment, see [Preview Sandbox Testing Environment- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
