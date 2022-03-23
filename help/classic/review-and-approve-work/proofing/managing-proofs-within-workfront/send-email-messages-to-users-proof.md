---
filename: send-email-messages-to-users-proof
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Send email messages to reviewers on a proof
description: During the review and approval process, you can send a message to one or all of the reviewers on a proof. Messages are an easy way to remind reviewers to complete their review of a proof or to provide other information related to the proof.
---

# Send email messages to reviewers on a proof

During the review and approval process, you can send a message to one or all of the reviewers on a proof. Messages are an easy way to remind reviewers to complete their review of a proof or to provide other information related to the proof.

You can choose between sending a generic reminder email or sending a customized message to one or all of the users associated with a given stage.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof role</td> 
   <td>Author or Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Send email messages to users on a proof

1. Select the document for the proof that contains the users you want to message.
1. In the **Details**&nbsp;tab, locate&nbsp;the **Proofing**&nbsp;section.

1. 
1. Click **Details.**
1. The proofing viewer box appears.
1. (Conditional) To send a message to multiple&nbsp;users in a stage:
1. In the **Workflow** section, in the stage that contains the users that you want to message, do one of the following (depending on whether the proof for which you are messaging users has or does not have&nbsp;Advanced Workflow enabled):
1. ```<li> <p>If you are sending messages to users on a proof that has Advanced Workflow enabled:&nbsp;Click <strong>More,</strong>&nbsp;then click <strong>Message all</strong>.</p> <p> <img src="assets/proof-details-email-350x248.png" alt="" style="width: 350;height: 248;"> </p> </li>``` ```<li> <p>If you are sending messages to&nbsp;users on a proof without Advanced Workflow:&nbsp;Click the <strong>More Options</strong> icon, then click <strong>Message all</strong>.</p> <p> <img src="assets/proof-details-email-basic-350x247.png" alt="" style="width: 350;height: 247;"> </p> <p>The Message box appears.</p> <p> <img src="assets/proof-email-350x307.png" alt="" style="width: 350;height: 307;"> </p> </li>``` 

1. Workflow
1. ```<li><p>If you are sending messages to a user&nbsp;on a proof that has Advanced Workflow enabled:&nbsp;Click <strong>More,</strong>then click&nbsp;<strong>Message</strong>.</p><p><img src="assets/proof-details-email-user-350x247.png" alt="" style="width: 350;height: 247;"></p></li>``````<li><p>If you are sending messages to a user on a proof without Advanced Workflow:&nbsp;Click the <strong>More Options</strong> icon, then click <strong>Message.</strong></p><p><img src="assets/proof-details-email-user-basic-350x247.png" alt="" style="width: 350;height: 247;"></p><p>The <strong>Message</strong> box appears.</p><p><img src="assets/proof-email-350x307.png" alt="" style="width: 350;height: 307;"></p></li>```

1. Send to
1. In the **Message details** section, specify the following information:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Notify people by email</td> 
      <td>This option cannot be deselected. All users receive the message via email.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Discard custom message</td> 
      <td> <p>Click <strong>Discard custom message</strong> if you want to include only the default email content.</p> <p>The default reminder email includes the following information:</p> 
       <ul> 
        <li>Personal link to the proof<br>Thumbnail of the proof image<br></li> 
        <li>The following proof details: Proof name, version number, folder name (if applicable), and a list of the reviewers and their progress on the proof.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Subject</td> 
      <td>Type a message subject.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Message</td> 
      <td>Type your message content.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Send.**

