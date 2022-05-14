---
filename: faq-review-proofs
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: FAQ - Review proofs
description: Guest reviewers, who don’t have their own logins to ProofHQ, access their proofs using the Go to proof link in the emails they receive. Users can access their proofs from the emails and also have the advantage of using their dashboard in the account. From the dashboard view, they can take a look at a list of proofs that require their decision and access them with one click by clicking on the blue Go to proof icon.
---

# FAQ - Review proofs

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## How can I access a proof that was shared with me

Guest reviewers, who don’t have their own logins to ProofHQ, access their proofs using the *Go to proof* link in the emails they receive. Users can access their proofs from the emails and also have the advantage of using their dashboard in the account. From the dashboard view, they can take a look at a list of proofs that require their decision and access them with one click by clicking on the blue *Go to proof* icon.

## How do I add comments to a proof?

To add a comment to a proof, click on the *Add a comment* button available at the top of the page. If you don’t see that button, please contact the owner of the proof, it is possible that you were assigned the wrong proof role (for more information about proof roles, see [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

A comment box will open to the right of the screen, here you can type your comment and save it on the proof. This will leave a general comment on the proof, not connected to any specific area of the proof. If you would like to comment on something specific, use the markup tools available at the top of the page.

To reply to someone’s comment on the proof, click on that comment in the list of comments and type your reply in the reply box. When you save, the reply will be posted on the proof.

All comments and decisions appear on the proof almost immediately, so if anyone else is looking at the proof at the same time as you, they will see your comments straight away.

These are very basic instructions to get you started with ProofHQ. If you would like to find out more about reviewing proofs, please go to the&nbsp; [Reviewing proofs](https://support.workfront.com/hc/en-us/sections/200054044-Reviewing-proofs)&nbsp;section of the Help Center for more detailed help articles.

## How do I mark up a proof?

ProofHQ offers a set of drawing tools that will help you leave precise feedback on your proofs. You can choose the color and the opacity of each markup you leave on the proof, and for line tools you can also change the thickness of the line.

To view the available tools, click on the Add a comment button at the top of the page. Drawing tools available in the toolbar are:

* rectangle&nbsp;
* freehand line
* straight line
* connected lines
* arrow
* highlight
* mask shape

To draw, simply pick the tool you want to use, the color of the markup and the thickness of the line (for line tools). You can have multiple markups attached to a comment. When you save the comment, a pin with the number of the comment will be dropped in the middle of the group of markups. Pins allow you to quickly view markups left on the proof, if you click on it, the markup and the comment connected to the markup will show.

## What tools could I use to markup text in a proof?

The text annotation tool available in the Proof Viewer allows you to quickly markup text in your proof. To access it, you click on the *Add a comment* button at the top of the page. The annotation tool is the first icon to the left in the toolbar. It allows you to select text in your proof. You have 4 options to choose from:

* highlight - it highlights the text and copies it into the comment box
* replace - copies the text and adds [REPLACE] and [WITH] in the comment box, so that you can easily suggest replacement text
* delete - strikes through the text and adds [DELETE] to the comment box
* insert after - lets you easily suggest text that needs to be inserted after the highlighted phrase

If the text you’d like to use is saved in a separate document, you can use the keyboard shortcuts (ctrl+c and ctrl+v on a PC, cmd+c and cmd+v on a Mac) to copy and paste it into the comment box.

## What does it mean to make a decision on a proof?

Making a decision on a proof can have two meanings in ProofHQ. On one hand, it can be a formal approval when somebody needs to sign off on a proof. Another approach is using the action of making a decision to notify other reviewers that you are done making comments on the proof.

Standard decision options available in ProofHQ are *Approved*, *Approved with changes*, *Changes required* and *Not relevant*. Administrators in Enterprise and Unlimited accounts can customize these options (rename or even hide them). To learn more, see [Configure approval decision options in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Does everyone have to make a decision on a proof?

No, it depends on what proof role each reviewer was assigned on a proof (for more information about proof roles, see [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)). *Approver*, *Reviewer and Approver*, *Moderator* and *Author* are roles that require a decision on the proof.

Usually the person who creates the proof doesn’t need to make a decision, however this depends on the workflow in your organization. If a reviewer doesn’t need to make a decision on a proof, make sure that their role is set to reviewer, otherwise the system will wait for their decision before the overall status of the proof is updated.

If you are sending a proof to a group of reviewers, but you only need one person to sign off on the proof and it doesn’t matter who makes the decision, you can enable Only one decision required. The overall proof progress will be updated after the first decision on the proof is made, regardless of who makes the decision.

## Can I generate a list of all comments that were made on a proof?

Yes, you can generate a *Print summar*y of the comments left on the proof. This document can be generated either for a single version or across all versions that were shared with this reviewer. It shows you a list of all comments, markups and decisions that were made on the proof. For more information about this feature, please visit [Print and Export Comments in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).
