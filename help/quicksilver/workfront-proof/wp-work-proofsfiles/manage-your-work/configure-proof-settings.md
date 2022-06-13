---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Configure Proof Settings in Workfront Proof
description: You can configure a proof you are creating or editing in any of the following ways - EDIT ME.
feature: "Workfront Proof, Digital Content and Documents"
---

# Configure Proof Settings in Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

You can configure a proof you are creating or editing in any of the following ways:

>[!NOTE]
>
>&nbsp;You can configure these settings for all new proofs you create. For more information, see .

## Lock the Proof When Last Decision Is Made

You can set a proof state to lock when the final Approver makes their decision. This is useful if you want to make sure that your reviewers won't be able to go back to the proof and add additional comments or change their decisions.

1. Create a new proof, as described in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).  
   Or  
   Open the Proof details page for an existing proof, as described in [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. For a new proof, under **Proof settings**, select **Lock proof when all required decisions are made**.  
   Or  
   For an existing proof, under **Settings**, select **Lock the proof when all decisions are made**.

For information about decisions, see [Make a decision on a proof in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Require Login for All Users Who Review the Proof

One of the great things about Workfront Proof is that anybody can review a proof, you don't need to have your own Workfront Proof to do so. Recipients receive an email with a Personal URL that takes them straight to the proof page, without them having to log into Workfront Proof.

However, if you require higher levels of security for your review and approval process, you can use require login to the proof. This means that only Workfront Proof&nbsp;users can be added to the proof. And they must enter their email and password before they can access it.

>[!NOTE]
>
>* *In order for somebody to sign in to the proof (when Login required has been enabled), they must have been added to the proof.* 
>* *If Login required is enabled, Subscriptions cannot be enabled.* 
>

To require login for all users who review the proof:&nbsp;

1. Create a new proof, as described in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).  
   Or  
   Open the Proof details page for an existing proof, as described in [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. For a new proof, under **Proof settings**, select **Require login**.  
   Or  
   For an existing proof, under **Settings**, select **Login required**.

## Require Only One Decision for the Proof

This setting is useful in cases when you just need one person out of a group, department, or company to make a decision on the proof.

Even if you assign the role of Approver or Reviewer and Approver to multiple people, once one person makes a decision on a proof, the status of the proof will be updated (as per the decision made). For more information about proof status, see [View the Progress and Status of a Proof in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Create a new proof, as described in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).  
   Or  
   Open the Proof details page for an existing proof, as described in [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. For a new proof, under **Workflow**, select **Require only one decision for this stage**.  
   Or  
   For an existing proof, under **Settings**, select **Only one decision required**.

For information about decisions, see [Make a decision on a proof in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Require Decisions to Be Electronically Signed

You can require an electronic signature of any reviewer who makes a decision on the proof to provide their email and password. When&nbsp;a reviewer makes a decision prompt appears asking them to input their email and password and to confirm their decision. For more information, see [Understanding electronic signatures in Workfront Proof](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Create a new proof, as described in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).  
   Or  
   Open the Proof details page for an existing proof, as described in [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. For a new proof, under **Proof settings**, select **Require decisions to be electronically signed**.  
   Or  
   For an existing proof, under **Settings**, select **Require decisions to be electronically signed**.

For information about decisions, see [Configure approval decision options in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Disallow Users to Download the Original File

You can keep reviewers on a proof from downloading the original file from which a proof was created.

1. Create a new proof, as described in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).  
   Or  
   Open the Proof details page for an existing proof, as described in [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. For a new proof, under **Proof settings**, deselect **Download original file**.  
   Or  
   For an existing proof, under **Settings**, select **Download of original file**.

## Allow Other Users to Subscribe to the Proof

Subscription is an advanced setting that works with the Proof URL and Mini proof.

By default people who have not been specifically added to the proof and are using the Proof URL or the Mini proof to access it can only view the proof in Read Only mode. People who are already reviewers on the proof can sign in using their email address. For more information, see [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

Enabling subscription on the proof allows people who have not been added explicitly to the proof to subscribe themselves to the proof (i.e. add themselves to the proof). They will then be assigned the role and email alert that you select for them in the Subscription settings.

If Subscription has been enabled on a proof, the fields below will become active:

* **Subscriber validation required** - Subscriber must click a link in an email to access a proof  
  Selecting this option means that the person subscribing will not get immediate access to the proof, but will get a link to the proof in an email. The purpose of subscriber validation is to ensure that the person has entered a correct email address to which they have access.

* **Default role for new subscribers -** This is the default proof role that will be assigned to all reviewers that subscribe themselves to the proof.
* **Default email alert for new subscribers**&nbsp;- This the default email alert that will be assigned to all reviewers that subscribe themselves to the proof.

See also&nbsp; [Subscribe to a Proof in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

To allow other users to subscribe to a proof:

1. Create a new proof, as described in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).  
   Or  
   Open the Proof details page for an existing proof, as described in [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. For a new proof, under **Proof settings**, deselect **Subscribe to proof via public URL or embed code**.  
   Or  
   For an existing proof, under **Settings**, select **Subscription**.

