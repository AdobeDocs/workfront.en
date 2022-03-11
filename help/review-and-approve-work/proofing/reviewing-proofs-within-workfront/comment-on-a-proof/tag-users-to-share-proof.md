---
filename: tag-users-to-share-proof
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Tag users to share a proof
description: When you are commenting on a proof in the proofing viewer, you can tag other users to bring their attention to your comment via email and to add them to the proof's workflow.
---

# Tag users to share a `proof`

When you are commenting on a `proof` in the `proofing viewer`, you can tag other users to bring their attention to your comment via email and to add them to the `proof`'s workflow.

When tagging users in comments on a proof, the users you are able to tag might differ depending on various factors, such as individual user permissions and your membership in the organization:

* If you are the proof creator, owner, or have specific permissions enabled, you can tag users outside of the proof workflow and share the proof with them.
* If you were added to the proof as an outside user and you are a member of another environment with a different proof account, you can tag only those users from your original environment. For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> Proof role Author, Moderator Proof Permission Profile Supervisor or Administrator Access level configurations* Edit access to Documents For information on requesting additional access, see Request access to objects in Adobe Workfront. 
 </tbody> 
</table>

&#42;To find out what plan, role, or `Proof Permission Profile` you have, contact your `Workfront` or `Workfront Proof administrator`.

## Tag users to share a `proof`

Users with the `Proof Permission Profile` or Proof role outlined in the [Access requirements](#access) section above can tag users to share a `proof` by default. You can also tag users to share a `proof` regardless of `Proof Permission Profile` or Proof role if you are the proof owner or creator. You can enable users with lower `Proof Permission Profile` or Proof roles to tag users to share a proof when creating a proof. For more information, see the [Configure the workflow and add reviewers](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) section in the [Create an advanced proof with a Basic workflow](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) article.

>[!NOTE]
>
>You can tag an external collaborator using their email address only if either of the following is true:>
>* A user in your organization's `Workfront` account has added the collaborator's email address to a `proof` previously.
>
>* The collaborator has used the email address to subscribe to a `proof` in your organization's `Workfront` account previously.
>

To tag someone and share a `proof` in a comment:

<ol> 
 <li value="1"> <p>As you comment on a proof, type an at sign (@) followed by the person's name or email address. When you start typing, available names appear in a drop-down list.</p> </li> 
 <li value="2"> <p> Select the person's name when you see it in the drop-down list. </p> <note type="tip">
   If you want to close the drop-down list without selecting anyone, you can press the 
   <span class="bold">Esc</span> key or click anywhere outside the list.
  </note> </li> 
 <li value="3">Repeat steps 1-2 for any other users you want to tag in the comment.</li> 
 <li value="4">Finish the comment, then click <span class="bold">Post</span>.</li> 
 <li value="5"> <p>(Conditional) If you tagged anyone who was not already added to the <span>proof</span>, specify a <span class="bold">Proof role</span> and <span class="bold">Email alerts</span> setting for each user listed in the box that appears, then click <span class="bold">Add people and post comment</span>.</p> <p> <img src="assets/add-people-to-proof-350x220.png" style="width: 350;height: 220;"> </p> <p>For information about <span>proof</span> roles, see <a href="../../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configure default proofing roles</a>. For information about proof email alerts, see the section in the article <a href="../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.</p> <p>If the <span>proof</span> has an Automated Workflow, the users you tag are added to the stage you are in. For more information, see <a href="../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Automated Workflow overview</a>.</p> <p>Anyone you tag receives a notification email about your proof comment, regardless of the <span>proof</span> email alert settings they are using:</p> 
  <ul> 
   <li>If the user&nbsp;receives a daily summary or hourly summary email, <span>Workfront</span> sends the notification separately and includes information about your proof comment in the summary email.</li> 
   <li> <p>If the user receives alerts for all activity, or for replies made to their comments, the notification replaces the notifications about these comments and replies.</p> </li> 
  </ul> </li> 
</ol>

For information about other ways to add users to a `proof`, see [Share a proof within Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
