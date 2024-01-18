---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Create an advanced proof with a Basic workflow
description: With a basic workflow, you can several reviewers to a proof, but they are not organized into stages. All of the reviewers you add can access the proof immediately after you create it.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
---
# Create an advanced proof with a Basic workflow

With a basic workflow, you can several reviewers to a proof, but they are not organized into stages. All of the reviewers you add can access the proof immediately after you create it.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>
   <p>New: Any</p>
    <p>Current plan: Pro or Higher</p>
   <p>Legacy plan: Select or Higher</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
    <p>Current: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Documents</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Create an advanced proof with a Basic workflow

1. Go to the project, task, or issue where you want the proof, then click the **Documents** tab.
1. Click **Add new** > Proof, upload the content, then work through the sections listed below.

   or

   Hover over an existing document, then click the **Create Proof** > **Advanced Proof** and work through the sections listed below.

## Configure the workflow and add reviewers

1. In the Workflow type section, choose **Basic**.
1. Specify the users you want to add, then choose a Proof role.

   ![](assets/new-proof---roles-350x213.png)

1. The following table lists each role and the rights associated with it. 

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>&nbsp;</p> </th> 
      <th> <p><strong>View a proof</strong> </p> </th> 
      <th> <p><strong>Add markups</strong> </p> </th> 
      <th> <p><strong>Add comments</strong> </p> </th> 
      <th> <p><strong>Edit own comments if there are no replies</strong> </p> </th> 
      <th> <p><strong>Make a decision</strong> </p> </th> 
      <th> <p><strong>Delete comments made by others</strong> </p> </th> 
      <th>Resolve comments</th> 
      <th>Apply Actions to Comments</th> 
      <th> <p><strong>Edit the proof</strong> </p> </th> 
      <th>Share the proof with others</th> 
      <th>Create new version</th> 
      <th> <p><strong>View approval requests in the Home area</strong> </p> </th> 
      <th>Add new reviewers</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Read Only</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td>&nbsp;</td> 
      <td>✓</td> 
      <td> <p>&nbsp;</p> </td> 
      <td>✓</td> 
      <td>&nbsp;</td> 
      <td>&nbsp;</td> 
      <td>&nbsp;</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Reviewer</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td>&nbsp;</td> 
      <td>✓</td> 
      <td> <p>&nbsp;</p> </td> 
      <td>✓</td> 
      <td>&nbsp;</td> 
      <td>&nbsp;</td> 
      <td>&nbsp;</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Approver</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td>&nbsp;</td> 
      <td>✓</td> 
      <td> <p>&nbsp;</p> </td> 
      <td>✓</td> 
      <td>&nbsp;</td> 
      <td> <p>✓</p> </td> 
      <td>&nbsp;</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Reviewer &amp; Approver</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td>&nbsp;</td> 
      <td>✓</td> 
      <td> <p>&nbsp;</p> </td> 
      <td>✓</td> 
      <td>&nbsp;</td> 
      <td> <p>✓</p> </td> 
      <td>&nbsp;</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Author</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>&nbsp;</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>&nbsp;</td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Moderator</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p>&nbsp;</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. Users on new Workfront plans can grant author or moderator roles to any users in the system. Users on legacy plans can grant author or moderator roles to any user with a proof license in the system.
1. (Optional) With the drop-down menu still open, select any additional permissions available at the bottom of the menu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Resolve comments and apply actions </td> 
      <td> <p>Allows the Workfront user to do the following:</p> 
       <ul> 
        <li>Resolve a comment after it has been addressed, as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Resolve proof comments</a>.</li> 
        <li>Apply actions to comments, as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Use actions on proof comments</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Share proof by tagging</td> 
      <td> <p>Allows the reviewer to add any Workfront user to the proof as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Tag users to share a proof</a>.</p> <p>Note:  <p>If these two options are unavailable (dimmed), the user already has a permission profile that allows resolving comments, applying actions to comments, and tagging any user. </p> <p>If the options do not display, the person you added is not a Workfront license holder.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Repeat steps 1-3 for any other users you have added to the proof.
1. For each user you are sharing with, in the **Email alerts**&nbsp;drop-down list, select the type of email alerts this user receives when people make comments and decisions on the proof:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">All activity</td> 
      <td>Workfront sends an email to the reviewer every time there is any activity on the proof, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the proofing process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Replies to my comments</td> 
      <td>An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the proof makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the proof so that they are not&nbsp;notified of any other comments&nbsp;on the proof, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the proof in&nbsp;the proofing viewer.</p><p>For information about comments, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisions</td> 
      <td>Workfront sends an email to the reviewer only when someone makes a&nbsp;decision.<p>This can be useful for the person who is managing the approval process&nbsp;(such as a project manager) and&nbsp;needs to monitor progress on the proof and see which users have&nbsp;made their&nbsp;decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Final decision</td> 
      <td>Workfront sends an email when the last approver on the proof has made their&nbsp;decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.</p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hourly Summary</td> 
      <td>Workfront sends an email to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the hour.<p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the proof.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Daily Summary</td> 
      <td>Workfront sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">No email</td> 
      <td>Workfront does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a proof only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your proofs have this setting.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue with [Configure email settings for the proof](#configure-email-settings-for-the-proof) below.

## Configure email settings for the proof {#configure-email-settings-for-the-proof}

1. In the **Email notification** section, select whether to send email notifications and a custom message to&nbsp;the users you selected in [Create an advanced proof with a Basic workflow](#workflow) earlier in this article:

   <table>
   <tbody>
   <tr>
   <td>Notify recipients about this proof</td>
   <td>Select this option to send an email notification to users. When <strong>Basic sharing</strong> is selected in the <strong>Workflow</strong> section, an email notification is sent when the proof is created. When <strong>Automated workflow</strong> is selected in the <strong>Workflow</strong> section, an email notification is sent when the proof enters the stage of the Automated Workflow that the user is associated with.</td>
   </tr>
   <tr>
   <td>Add custom message</td>
   <td>Select this option to include a custom message in the notification. You can specify a subject and message body. The message body can include rich text formatting, such as bold, bullets, and hyperlinks.</td>
   </tr>
   </tbody>
   </table>


1. Continue with [Configure proof settings](#configure-proof-settings) below.

## Configure proof settings {#configure-proof-settings}

1. In the **Proof settings** section, select any of the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Require login - proof can only be shared with other users</td> 
      <td>When this option is disabled (default), anyone with the URL is able to view the proof. <br>When this option is selected:
       <ul>
        <li>Only Workfront Proof&nbsp;users are able to view the proof.</li>
        <li>Users cannot sign in to the proof unless they have been added to the proof.</li>
        <li>Subscriptions cannot be enabled.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Only one decision required for this proof</td> 
      <td>When this option is selected, the review is completed after one of the decision makers makes their decision.<br>This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Require decisions to be electronically signed</td> 
      <td>Users are required to specify their user name and password at the time that they make a decision on&nbsp;a proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock proof when all required decisions are made</td> 
      <td>When this setting is enabled, the proof state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.<br>This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Download original file</td> 
      <td>When this option is selected, reviewers are able to download the original file from which the proof was created.<br>When this option is deselected, the Download icon is no longer visible.<br>This option is enabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Share proof via public URL or embed code</td> 
      <td>When this option is selected, the proof can be shared via a public URL or embed code.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Subscribe to proof via public URL or embed code</td> 
      <td>When this option is selected, people who have not been added explicitly to the proof can subscribe to the proof. The person subscribing to the proof is granted the role and email that you define in the following settings:
       <ul>
        <li><strong>Subscriber role:</strong>&nbsp;The default proof role that is&nbsp;assigned to all reviewers that subscribe to the proof.&nbsp;</li>
        <li><strong>Email alert settings for subscribers:</strong>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the proof.</li>
       </ul><p>
        <ul>
         <li><strong>Proof access via email link required for:</strong>&nbsp;Configure whether the subscriber receives an email with a link to the proof. You can select <strong>No email</strong> (email link is not required to access the proof), <strong>Proof notification email only</strong> (subscriber receives a link to the proof via email without any verification), or <strong>Validation and proof notification emails</strong> (subscriber receives a link to the proof via email and must click the link to access a proof, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
        </ul><p>Note: &nbsp;If the proofs have Automated Workflow attached all subscriptions will generate confirmation emails to the proof Owners, so they could decide which stage the person should be added to.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Create Proof**.

   Workfront&nbsp;begins generating a proof of the selected documents or websites.&nbsp;Depending on the file size and type, the lag time on a document upload can vary. Be patient as bigger files take longer to generate. You can navigate away from the page and Workfront&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.

1. After&nbsp;the proof is generated, click&nbsp;**Open proof**&nbsp;to launch the proofing viewer.

   ![](assets/open-proof-350x132.png)

   Users who do not have proofing enabled on their account&nbsp;are still able to view the document and make comments to the proof.