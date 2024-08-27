---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Tag users to share a proof
description: When you are commenting on a proof in the proofing viewer, you can tag other users to bring their attention to your comment via email and to add them to the proof's workflow.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
---
# Tag users to share a proof

When you are commenting on a proof in the proofing viewer, you can tag other users to bring their attention to your comment via email and to add them to the proof's workflow.

When tagging users in comments on a proof, the users you are able to tag might differ depending on various factors, such as individual user permissions and your membership in the organization:

* If you are the proof creator, owner, or have specific permissions enabled, you can tag users outside of the proof workflow and share the proof with them.
* If you were added to the proof as an outside user and you are a member of another environment with a different proof account, you can tag only those users from your original environment. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Access requirements {#access-requirements}

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Proof role</td> 
   <td>Author, Moderator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Supervisor or Administrator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Tag users to share a proof

Users with the Proof Permission Profile or Proof role outlined in the [Access requirements](#access-requirements) section above can tag users to share a proof by default. You can also tag users to share a proof regardless of Proof Permission Profile or Proof role if you are the proof owner or creator. You can enable users with lower Proof Permission Profile or Proof roles to tag users to share a proof when creating a proof. For more information, see the [Configure the workflow and add reviewers](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) section in the [Create an advanced proof with a Basic workflow](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) article.

>[!NOTE]
>
>You can tag an external collaborator using their email address only if either of the following is true:>
>* A user in your organization's Workfront account has added the collaborator's email address to a proof previously.
>* The collaborator has used the email address to subscribe to a proof in your organization's Workfront account previously.
>

To tag someone and share a proof in a comment:

1. As you comment on a proof, type an at sign (@) followed by the person's name or email address. When you start typing, available names appear in a drop-down list.
1. Select the person's name when you see it in the drop-down list.

   >[!TIP]
   >
   >If you want to close the drop-down list without selecting anyone, you can press the **Esc** key or click anywhere outside the list.

1. Repeat steps 1-2 for any other users you want to tag in the comment.
1. Finish the comment, then click **Post**.
1. (Conditional) If you tagged anyone who was not already added to the proof, specify a **Proof role** and **Email alerts** setting for each user listed in the box that appears, then click **Add people and post comment**.

   ![](assets/add-people-to-proof-350x220.png)

   For information about proof roles, see . For information about proof email alerts, see the section in the article [Configure email notification settings in Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   If the proof has an Automated Workflow, the users you tag are added to the stage you are in. For more information, see [Automated Workflow overview](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Anyone you tag receives a notification email about your proof comment, regardless of the proof email alert settings they are using:

   * If the user&nbsp;receives a daily summary or hourly summary email, Workfront sends the notification separately and includes information about your proof comment in the summary email.
   * If the user receives alerts for all activity, or for replies made to their comments, the notification replaces the notifications about these comments and replies.

For information about other ways to add users to a proof, see [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
