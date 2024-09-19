---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Manage notifications for proof comments and decisions
description: When you work on a proof, whether you are a Adobe Workfront user or an external collaborator, you can specify which email notifications you want to receive about comments and decisions made on the proof. For more information, see Notifications for proof comments and decisions overview.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
---
# Manage notifications for proof comments and decisions

When you work on a proof, whether you are a Adobe Workfront user or an external collaborator, you can specify which email notifications you want to receive about comments and decisions made on the proof. For more information, see [Notifications for proof comments and decisions overview](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>These notifications are different from the email alerts you can receive about the flow of a proof among reviewers. They are also different from the email alert settings you can configure in Workfront.&nbsp;

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
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
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Manage notifications for proof comments and decisions

1. Open the proof for which you want to configure notifications you will receive.
1. If the left toolbar is not showing, click the&nbsp;**Menu**&nbsp;icon, located in the upper-left corner of the Web Proofing Viewer.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. In the left toolbar, click the&nbsp;**Settings**&nbsp;icon. ![Settings_icon.png](assets/settings-icon.png)  

1. Under **Send me email notifications about**, click the setting you want for the proof.

   The setting you select remains in effect only for the proof you have open.

   The system default is **Daily summary**. If you or your reviewers do not make any other changes, all your proofs have this setting.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">All activity</td> 
      <td>An email is sent to the reviewer every time there is any activity on the proof, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision.<br><p>This is a great option for the person who is managing the proofing process because&nbsp;it allows them to see the activity as it happens. Users do not receive an email alert about their own activity (for example, comments, replies, and decisions made.)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Replies to my comments</td> 
      <td>An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the proof makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the proof so that they are not&nbsp;notified of any other comments&nbsp;on the proof, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the proof in&nbsp;the proofing viewer.<br></p><p>For information see, <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisions</td> 
      <td>An email is sent to the reviewer only when someone makes a&nbsp;decision.<br><p>This email alert can be useful for the person who is managing the approval process&nbsp;(such as a project manager) because&nbsp;it allows the person managing the approval process&nbsp;to monitor progress on the proof and to see which users have&nbsp;made their&nbsp;decision.<br></p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Final decision</td> 
      <td>An email is sent when the final&nbsp;decision&nbsp;is&nbsp;made on the proof (when the last approver on the proof has made their&nbsp;decision).<br><p>This alert is often used by the designer because the designer does not&nbsp;need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.<br></p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hourly summary</td> 
      <td>An email is sent to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the last hour.<br><p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. If there is&nbsp;no activity from other users,&nbsp;no email is&nbsp;sent.<br></p><p>This alert is a good way of seeing an overview of the project.<br></p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the proof.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Daily summary</td> 
      <td>(Default setting): An email is sent every day with all&nbsp;comments, replies, and decisions listed. An email is sent only on days when there is activity besides your own.<br><p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.<br></p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">No email</td> 
      <td>No email alerts are sent.<br><p>This setting is useful&nbsp;for a person who is added to a proof only for reference purposes and does not need to be notified of any changes.</p><p>Note: <p>This option turns off only email alerts you can receive about proof comments and decisions. It does not turn off the email alerts you can receive about the flow of a proof, such as the New Proof or Late Proof email. For more information about email alerts concerning the flow of a proof, see the following articles: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">The New Version email</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">Late proof email</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
