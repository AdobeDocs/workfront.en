---
filename: share-a-proof-in-proofing-viewer
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Share a proof from the proofing viewer
description: You can share a proof from the proofing viewer if sharing is enabled by the proof owner or creator.
---

# Share a proof from the proofing viewer

You can share a proof from the proofing viewer if sharing is enabled by the proof owner or creator.

>[!IMPORTANT]
>
>The Allow sharing proof via public URL or embed code setting must be enabled.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
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
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Share the URL

You can share a proof via a URL if the owner has configured the proof for sharing. Proof owners can update sharing settings any time. For more information, see [Edit proof settings](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

<ol> 
 <li value="1"> <p>If the left icon menu is not displayed, click the <span class="bold">Menu</span> icon on the upper-left corner of the proofing viewer.</p> <p> <img src="assets/menu-icon-in-proofing-viewer-350x188.png" style="width: 350;height: 188;"> </p> </li> 
 <li value="2"> <p>In the left icon menu of the proofing viewer, click the <span class="bold">Share</span>&nbsp;icon.</p> <p> <img src="assets/share-btn-in-viewer.png" alt="Share_btn_in_viewer.png"> </p> </li> 
 <li value="3">In the <span class="bold">Share proof</span> options that appear, make sure <span class="bold">Get shareable link</span> is selected.</li> 
 <li value="4"> <p>&nbsp;Do either of the following:</p> 
  <ul> 
   <li> <p>To copy the link to your clipboard, click <span class="bold">Copy link</span>.</p> <p>You can now distribute the link via a third-party tool, such as a chat or an email application.</p> </li> 
   <li>To email the link directly from Adobe Workfront, do the following:
    <ol>
     <li value="1"><p>In the <span class="bold">Or email link to</span> field, begin typing and select the name of your recipient. Or specify the email address of an external user who you want to share with.</p></li>
     <li value="2"><p>Select from the following options:</p>
      <table cellspacing="0">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Send public link</td>
         <td><p>Includes a button in the email notification that directs users to the proof within the proofing viewer they are using and grants View access.</p><p>If <span class="bold">Subscribe to proof via public URL or embed code</span> is turned off for the proof, users can sign in with their Workfront login credentials to add comments to the proof. If it is turned on, anyone providing their email address and name (no password required) can sign and add comments to the proof.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Send download link</td>
         <td>Includes a button in the email notification that directs users to a download page, which provides file details, file name, and file size, with the file displayed inline. Users can click the Download link from the download page to download the file.</td>
        </tr>
        <tr>
         <td role="rowheader">Add custom message</td>
         <td>Allows you to specify a custom subject and body for the email notification.</td>
        </tr>
       </tbody>
      </table></li>
     <li value="3"><p>Click <span class="bold">Send</span>.</p><p>Your recipients receive an email notification containing information about the proof and the buttons you chose to include.</p><p><img src="assets/proof-share-email-350x87.png" style="width: 350;height: 87;"></p></li>
    </ol></li> 
  </ul> </li> 
</ol>

## Share the embed code

You can share a proof via embed code if the proof owner has configured it for this.

For information about configuring a prof with an embedded code, see [Configure a proof](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-proof.md) in [Configure a proof](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-proof.md).

To share a proof via the embed code:

<ol> 
 <li value="1"> <p>In the toolbar on the left of the proofing viewer, click the <span class="bold">Share</span>&nbsp;icon.<br></p> <p> <img src="assets/share-btn-in-viewer--1-.png" alt="Share_btn_in_viewer__1_.png"> </p> </li> 
 <li value="2">In the <span class="bold">Share proof</span> options that appear, click <span class="bold">Get embed code</span>, then click <span class="bold">Copy</span>.</li> 
</ol>

## Share a proof by adding users to it

You can add users to a proof while reviewing a proof if you have any of the following permissions:<![CDATA[    ]]>

* Supervisor or Administrator permissions
* Manager permissions and you are the proof creator or owner
* Manager permissions with the Author or Moderator proof role

If the proof has an Automated Workflow, you can add the user to an individual stage. For more information, see [Automated Workflow overview](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

By default, users you add to the proof:

* Receive an email notification with a link to the proof.
* Can make approval decisions on the proof from the Home or My Work area, as described in [Approving work in Adobe Workfront](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Do not need to have proofing enabled in order to review the proof.

When Automated Workflow is enabled and you add a user to the proof who does not have proofing enabled in Workfront, a new stage is created within the Automated Workflow. The user who you are adding is automatically added to this new stage when they view the proof for the first time. For more information, see [Automated Workflow overview](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

To share a proof with individual users:

<ol> 
 <li value="1"> <p>In the toolbar on the left of the proofing viewer, click the <span class="bold">Share</span>&nbsp;icon.<br></p> <p> <img src="assets/share-btn-in-viewer--2-.png" alt="Share_btn_in_viewer__2_.png"> </p> </li> 
 <li value="2">Click <span class="bold">Add recipients</span> in the list on the left.</li> 
 <li value="3">Under&nbsp;<span class="bold">New proof recipients</span>, begin typing the name of a user who you want to share the proof with, then click the name when it appears in the drop-down list.</li> 
 <li value="4"> <p>(Optional) Change any reviewer options to the right of the person's name:</p> 
  <ul> 
   <li><span class="bold">Proof role</span>: For more information, see <a href="../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</li> 
   <li><span class="bold">Stage</span>: (Available only if the proof has an Automated Workflow). For more information, see&nbsp;<a href="../../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li> 
   <li> <p><span class="bold">Email alerts</span>:&nbsp;Select one of the following options to specify how the person will be notified about activity on the proof.</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">All activity</td> 
       <td>Workfront sends an email to the reviewer every time there is any activity on the proof, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the proofing process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
      </tr> 
      <tr> 
       <td role="rowheader">Replies to my comments</td> 
       <td>An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the proof makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the proof so that they are not&nbsp;notified of any other comments&nbsp;on the proof, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the proof in&nbsp;the proofing viewer.</p><p>For information about comments, see <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
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
       <td>Workfront sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td> 
      </tr> No email Workfront does not send any email alerts. This is useful for a person who is added to a proof only for reference purposes and does not need to be notified of any changes. The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your proofs have this setting. <!--
       Set a deadline Select the day and time when users must take action on the proof. If you are adding users to a proof for a document that already exists in Workfront, you should have already set a deadline.
      --> <!--
       Notify people by email Select this option to send an email to the users, notifying them of the proof. Click Add a custom message to specify a message to include in the email notification.
      --> 
     </tbody> 
    </table> </li> 
  </ul> </li> 
 <li value="5">(Optional) Repeat the two previous steps to add multiple users to the proof.&nbsp;</li> 
 <li value="6"> <p>(Optional) Set a <span class="bold">Deadline</span> for the reviewers (available only if the proof does not have automated workflow). </p> </li> 
 <li value="7">(Optional) Select <span class="bold">Send email notification to new recipients</span> to let them know you have added them to the proof.</li> 
 <li value="8">When you are finished adding users to the proof, click <span class="bold">Done.</span></li> 
</ol>

