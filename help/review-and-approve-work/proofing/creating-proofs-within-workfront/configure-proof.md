---
filename: configure-proof
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Configure a proof
description: After you generate a proof, as described in the Generate a proof articles, the New Proof page displays. The following sections of the New proof page let you configure the proof so that it's ready for review.
---

# Configure a `proof`

After you generate a `proof`, as described in the [Generate a proof](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md) articles, the New Proof page displays. The following sections of the New proof page let you configure the `proof` so that it's ready for review.

## Add files

<ol> 
 <li value="1"> <p>Begin creating the <span>proof</span>, as described in the <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md" class="MCXref xref">Generate a proof</a> articles.</p> <p>The <span class="bold">New Proof</span> page appears.<br></p> </li> 
 <li value="2">To <span>proof</span> one or more documents, add documents to be proofed in either of the following ways (repeat this process to add multiple documents to be proofed): 
  <ul>
   <li>Drag a document from your file system into the drag-and-drop area in the <span class="bold">Add Files</span> area.</li>
   <li><p>Click <span class="bold">browse</span>, then find and select the document you want to upload from the file system on your workstation.</p><p><img src="assets/proof-document-upload-350x64.png" alt="proof_document_upload.png" style="width: 350;height: 64;"></p><p>The filename appears below the box where you added it. By default, the filename is also the name of the <span>proof</span>. You can upload up to 100 files at a given time.<br></p></li>
  </ul></li> 
 <li value="3">(Optional) If you want to change the name of the <span>proof</span>, type a new <span class="bold">Proof name</span>, then click <span class="bold">Done</span>.</li> 
 <li value="4">Continue with <a href="#single-proof" class="MCXref xref">Single proof</a> below.</li> 
</ol>

## Single proof

When the `Single proof` is enabled, all static files and websites are available in a single `proof`, and you can upload up to 500 files at a given time.

>[!NOTE]
>
>Interactive files, including videos and interactive websites, cannot be combined into a single `proof`.

1. Ensure that you have first added documents or the URL for a website or other web content to the `proof`, as described above in [Add files](#add-files).

1. (Optional) Enable  `Combine all compatible files into single proof`, then type a `Proof name` for the resulting `proof`.

1. (Optional) In the `Add Files` area on the left, drag the files or websites you have specified to change the order in which they appear as pages in the combined `proof`.&nbsp;

1. Continue with [Workflow](#workflow) below.

## Workflow

The workflow is where you add users and specify how you want them to review the `proof`. You can create either a basic workflow or an Automated Workflow for a `proof`.

With a basic workflow, you can add as many reviewers as you want to a `proof`, but they are not organized into stages. All of the reviewers you add can access the `proof` immediately after you create it.

An Automated Workflow makes it easier to manage the review process if your process is complex, or if you send content for review to the same people regularly. The `proof` moves from stage to stage and `Adobe Workfront` notifies each user when it is their turn to review it.

![](assets/proof-workflow-diagram-350x63.png)

For more information, see [Automated Workflow overview](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

>[!NOTE]
>
>* You can add an Automated Workflow to a `proof` only if your `Adobe Workfront` environment is integrated with a `Workfront Proof` Premium account. If you cannot use `proofing` as discussed in this section, contact your `Workfront administrator`.
>
>* You can add an Automated Workflow to a `proof` when you are uploading the document or after the document is uploaded.
>

* [Create a basic workflow for the proof](#create) 
* [Create an Automated Workflow for the proof](#create2) 
* [Configure settings for users added to the proof](#configuring-share-settings)

### Create a basic workflow for the `proof`

1. In the `Workflow` section, click `Basic`.

1. Continue with [Configure settings for users added to the proof](#configuring-share-settings) below.

>[!TIP]
>
>If you decide later than you would rather use an Automated Workflow for the `proof`, can do so. For more information, see [Convert a basic workflow to an Automated Workflow on a proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/convert-basic-automatic-workflow.md)

### Create an Automated Workflow for the `proof`

<ol> 
 <li value="1"> <p>In the <span class="bold">Workflow</span> section, click <span class="bold">Automated</span>. </p> </li> 
 <li value="2"> <p>(Optional) If you want to use an Automated Workflow template that your <span>Workfront administrator</span> created and shared with you, click <span class="bold">Add template</span>, select the template in the box that appears, then click <span class="bold">Add template</span>.</p> <p>Consider the following when you use an Automated Workflow template:</p> 
  <ol> 
   <ul> 
    <li style="font-style: normal;">An Automated Workflow template's settings determine&nbsp;what you can do with the Automated Workflow for a <span>proof</span>. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the <span>proof</span>. </li> 
    <li style="font-style: normal;">When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the <span>proof</span>, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. </li> 
    <li style="font-style: normal;">Your ability to modify an Automated Workflow template depends on the template settings configured by the <span>Workfront administrator</span>, as described in <a href="../../../administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md" class="MCXref xref">Create and manage Automated Workflow templates</a>. If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.</li> 
   </ul> 
  </ol> </li> 
 <li value="3">Configure the first stage of the Automated Workflow:
  <ol>
   <li value="1">(Optional) If you want to create a name for the first stage, click <span class="bold">Stage 1</span>, then type the name.</li>
   <li value="2"><p>In the <span class="bold">Recipients</span> section for the stage, add reviewers to the stage.</p><p>Consider the following when&nbsp;adding reviewers to a stage:</p>
    <ul>
     <li>After you add a user to a stage, you can configure settings for that user on the <span>proof</span>, such as the proof role and any additional permissions they should have and the type of email alerts they will receive when people make comments and decisions on the proof.. For more information, see <a href="#configuring-share-settings" class="MCXref xref">Configure settings for users added to the proof</a> in the article <a href="#" class="MCXref xref selected">Configure a proof</a>.</li>
     <li><p>You can drag one or more users from one stage to another. You can drag users directly to another stage, or you can drag users to a stage on the <span class="bold">Stages</span> diagram. To select multiple users, press Shift+Ctrl (on Windows) or Shift+Command (on Mac).</p><p><img src="assets/drag-name-stage-350x238.png" style="width: 350;height: 238;"></p></li>
     <li>You&nbsp;can add a reviewer to a <span>proof</span> only once, which means that you cannot add the same person to more than one stage on the <span>proof</span>.</li>
     <li>Reviewers who are not added to a private stage cannot see that stage on the <span>proof</span> or comments made in that stage.</li>
     <li>You can use an email address to add external users as reviewers.</li>
     <li><p>By default, adding a user&nbsp;to a stage grants&nbsp;that user access to view the <span>proof</span> from the moment the <span>proof</span> is created.<br></p><p>Your <span>Workfront administrator</span> can restrict users from accessing the <span>proof</span> until the workflow enters the stage where the user was added. For more information, see&nbsp;<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md" class="MCXref xref">Configure sharing settings for your users</a>&nbsp;in&nbsp;<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md" class="MCXref xref">Configure sharing settings for your users</a>.</p></li>
    </ul></li>
   <li value="3">Click <span class="bold">Stage settings</span>.</li>
   <li value="4"><p>Click an <span class="bold">Activate stage</span> option to indicate how you want the stage to activate.</p><p>For the first stage, you can select only <span class="bold">On proof creation</span>, <span class="bold">On a specific date and time</span>, or <span class="bold">Manually</span>. </p></li>
   <li value="5">(Conditional) If you selected <span class="bold">On a specific date and time</span> in the previous step, select the date and time when you want to activate the stage in the <span class="bold">Activate on</span> box that appears.</li>
   <li value="6"><p>Use any of the options below to further configure the stage.</p>
    <table cellspacing="0">
     <col>
     <col>
     <tbody>
      <tr>
       <td role="rowheader">Set stage deadline</td>
       <td><p>To set a deadline for the stage, click an option in the <span class="bold">Deadline options</span> drop-down list. Then, under <span class="bold">Deadline</span>, do one of the following:</p>
        <ul>
         <li>If you chose <span class="bold">Set specific date</span>: Select the deadline date and time you want.</li>
         <li>If you chose <span class="bold">Calculate from stage activation date</span>: Select the number of business days you want to add to the stage activation date to determine the deadline.</li>
        </ul></td>
      </tr>
      <tr>
       <td role="rowheader">Lock stage</td>
       <td>Specify when the stage can be locked. </td>
      </tr>
      <tr>
       <td role="rowheader">Transfer primary decision rights to</td>
       <td><p>Select the Primary decision maker on the stage (available only after you add&nbsp;at least one person to the stage who has a Proof role of Approver or higher). If you select a Primary decision maker, the <span class="bold">Only one decision required</span> option is disabled on this stage.</p></td>
      </tr>
      <tr>
       <td role="rowheader">Require only one decision for this stage</td>
       <td>Ends the entire review process when one of the decision makers makes a decision.<p>This option is not available if you designated a user in the&nbsp;<span class="bold">Primary decision maker&nbsp;</span>drop-down menu.</p></td>
      </tr>
      <tr>
       <td role="rowheader">Make this stage private</td>
       <td>Allows only the following people to view comments and decisions made during this stage: Supervisors, <span>Workfront administrators</span>, and <span>Workfront Proof administrators</span></td>
      </tr>
     </tbody>
    </table></li>
  </ol></li> 
 <li value="4">To add and configure another stage:
  <ol style="list-style-type: lower-alpha;">
   <li value="1">Click <span class="bold">New stage</span>.</li>
   <li value="2">(Optional) If you want to create a name for the first stage, click <span class="bold">Stage 2</span> (or <span class="bold">Stage 3</span>, <span class="bold">Stage 4</span>, and so on), then type the name.</li>
   <li value="3"><p>Click the <span class="bold">Activate stage</span>, then select an option to specify whether the stage is activated automatically or manually.</p><p>In addition to the options <span class="bold">On proof creation</span>, <span class="bold">On a specific date and time</span>, or <span class="bold">Manually</span>, you can select an option that is dependent on what occurred in the previous step: </p><p><img src="assets/activate-stage-options-for-stage-2-plus-350x177.png" style="width: 350;height: 177;"></p></li>
   <li value="4"><p>If you selected an Activate stage option that is dependent on what occurred in the previous step, use the options that appear to configure the activation setting. </p><p>For example, if you selected <span class="bold">When previous stage status changes</span>, select the <span class="bold">Previous stage</span>, then select the status in the <span class="bold">Status changed to</span> box.</p></li>
  </ol></li> 
 <li value="5"> <p>Repeat the previous step as needed to add more stages.</p> <p>As you add stages to the Automated Workflow, a diagram forms on the screen to represent them:</p> <p> <img src="assets/stages-diagram-350x213.png" style="width: 350;height: 213;"> </p> </li> 
 <li value="6">Continue the process of generating a new proof, as described in the <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof.md" class="MCXref xref">Generate a proof</a> articles.</li> 
 <li value="7">Continue with <a href="#configuring-share-settings" class="MCXref xref">Configure settings for users added to the proof</a> below. </li> 
</ol>

### Configure settings for users added to the `proof`

<ol> 
 <li value="1"> <p>In the <span class="bold">Workflow</span> section, in the row of a user you have added, click the drop-down menu in the <span class="bold">Proof role</span> column, then click the role you want to assign to the user. </p> <p> <img src="assets/new-proof---roles-350x213.png" style="width: 350;height: 213;"> </p> </li> 
 <p> <p>The following table lists each role and the rights associated with it. </p> 
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
   <thead> 
    <tr> 
     <th> <p>&nbsp;</p> </th> 
     <th> <p><span class="bold">View a <span>proof</span></span> </p> </th> 
     <th> <p><span class="bold">Add markups</span> </p> </th> 
     <th> <p><span class="bold">Add comments</span> </p> </th> 
     <th> <p><span class="bold">Edit own comments if there are no replies</span> </p> </th> 
     <th> <p><span class="bold">Make a decision</span> </p> </th> 
     <th> <p><span class="bold">Edit or delete comments made by others</span> </p> </th> 
     <th> <p><span class="bold">Edit the <span>proof</span></span> </p> </th> 
     <th> <p><span class="bold">View approval requests in the Home area</span> </p> </th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td> <p><span class="bold">Read Only</span>*</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td>&nbsp;</td> 
    </tr> 
    <tr> 
     <td> <p><span class="bold">Reviewer</span>*</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td>&nbsp;</td> 
    </tr> 
    <tr> 
     <td> <p><span class="bold">Approver</span> </p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>✓</p> </td> 
    </tr> 
    <tr> 
     <td> <p><span class="bold">Reviewer & Approver</span> </p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>✓</p> </td> 
    </tr> 
    <tr> 
     <td> <p><span class="bold">Author</span> </p> <p>(Not available when sharing with non-<span>proofing</span> users)</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>✓</p> </td> 
     <td>&nbsp;</td> 
    </tr> 
    <tr> 
     <td> <p><span class="bold">Moderator</span> </p> <p>(Not available when sharing with non-<span>proofing</span> users)</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p><span class="bold">✓</span> </p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>&nbsp;</p> <p>✓</p> <p>&nbsp;</p> </td> 
     <td> <p>&nbsp;</p> </td> 
     <td>&nbsp;</td> 
    </tr> 
   </tbody> 
  </table> </p> *Read-only and Reviewer roles are automatically granted View access on the document if they had none previously. <note type="note"> 
  <p> In addition to what is shown in this table, a Moderator can also submit new versions, add new reviewers, apply actions on comments, resolve comments, and delete comments and replies. (Deleting the first comment in a comment thread deletes the entire thread. Deleting a reply in the comment thread deletes only that reply.)</p> 
 </note> 
 <li value="2"> <p>(Optional) With the drop-down menu still open, select any additional permissions available at the bottom of the menu:</p> <p> <img src="assets/new-proof---addtnl-perms-350x213.png" style="width: 350;height: 213;"> </p> <note type="note">
   These additional permissions are available only if you are using an integrated 
   <span>proofing</span> account (
   <span>Workfront</span> integrated with 
   <span>Workfront Proof</span>).
  </note> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Resolve comments and apply actions</span> </td> 
     <td> <p>Allows the <span>Workfront</span> user to do the following:</p> 
      <ul> 
       <li>Resolve a comment after it has been addressed, as explained in the section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/create-manage-proof-comments.md#resolving-a-comment" class="MCXref xref">Resolve a comment</a> in the article <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/create-manage-proof-comments.md" class="MCXref xref">Create and manage proof comments</a>.</li> 
       <li>Apply actions to comments, as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Use actions on proof comments</a>. </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Share proof by tagging</span> </td> 
     <td> <p>Allows the reviewer to add any <span>Workfront</span> user to the <span>proof</span> as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Tag users to share a proof</a>.</p> <note type="note"> 
       <p>If these two options are unavailable (dimmed), the user already has a permission profile that allows resolving comments, applying actions to comments, and tagging any user. </p> 
       <p>If the options do not display, the person you added is not a <span>Workfront</span> license holder.</p> 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3">Repeat steps 1-3 for any other users you have added to the <span>proof</span>.</li> 
 <li value="4"> <p>For each user you are sharing with, in the <span class="bold">Email alerts</span>&nbsp;drop-down list, select the type of email alerts this user will receive when people make comments and decisions on the proof.</p> <p>For more information about these options, see <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">Notifications for proof comments and decisions overview</a>.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">All activity</td> 
     <td><span>Workfront</span> sends an email to the reviewer every time there is any activity on the <span>proof</span>, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the <span>proofing</span> process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Replies to my comments</td> 
     <td>An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the <span>proof</span> makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the <span>proof</span> so that they are not&nbsp;notified of any other comments&nbsp;on the <span>proof</span>, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the <span>proof</span> in&nbsp;the <span>proofing viewer</span>.</p><p>For information about comments, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Decisions</td> 
     <td><span>Workfront</span> sends an email to the reviewer only when someone makes a&nbsp;decision.<p>This can be useful for the person who is managing the approval process&nbsp;(such as a project manager) and&nbsp;needs to monitor progress on the <span>proof</span> and see which users have&nbsp;made their&nbsp;decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Final decision</td> 
     <td><span>Workfront</span> sends an email when the last approver on the <span>proof</span> has made their&nbsp;decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.</p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Hourly Summary</td> 
     <td><span>Workfront</span> sends an email to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the hour.<p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the <span>proof</span>.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Daily Summary</td> 
     <td><span>Workfront</span> sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td> 
    </tr> No email Workfront does not send any email alerts. This is useful for a person who is added to a proof only for reference purposes and does not need to be notified of any changes. The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your proofs have this setting. <!--
     Set a deadline Select the day and time when users must take action on the proof. If you are adding users to a proof for a document that already exists in Workfront, you should have already set a deadline.
    --> <!--
     Notify people by email Select this option to send an email to the users, notifying them of the proof. Click Add a custom message to specify a message to include in the email notification.
    --> 
   </tbody> 
  </table> </li> 
 <li value="5">Continue with <a href="#email-notification" class="MCXref xref">Email notification</a> in this article.</li> 
</ol>

## Email notification

<ol> 
 <li value="1"> <p>In the <span class="bold">Email notification</span> section, select whether to send email notifications and a custom message to&nbsp;the users you selected in <a href="#workflow" class="MCXref xref">Workflow</a> earlier in this article:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Notify recipients about this <span>proof</span></td> 
     <td>Select this option to send an email notification to users. When <span class="bold">Basic sharing</span> is selected in the <span class="bold">Workflow</span> section, an email notification is sent when the <span>proof</span> is created. When <span class="bold">Automated workflow</span> is selected in the <span class="bold">Workflow</span> section, an email notification is sent when the <span>proof</span> enters the stage of the Automated Workflow that the user is associated with.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Add custom message</td> 
     <td>Select this option to include a custom message in the notification. You can specify a subject and message body. The message body can include rich text formatting, such as bold, bullets, and hyperlinks.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2">Continue with <a href="#proof-settings" class="MCXref xref">Proof settings</a> below.</li> 
</ol>

## Proof settings

<ol> 
 <li value="1"> <p>In the <span class="bold">Proof settings</span> section, select any of the following options: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Require login - proof can only be shared with other users</td> 
     <td>When this option is disabled (default), anyone with the URL is able to view the <span>proof</span>. <br>When this option is selected:
      <ul>
       <li>Only <span>Workfront Proof</span>&nbsp;users are able to view the <span>proof</span>.</li>
       <li>Users cannot sign in to the <span>proof</span> unless they have been added to the <span>proof</span>.</li>
       <li>Subscriptions cannot be enabled.</li>
      </ul></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Only one decision required for this <span>proof</span></td> 
     <td>When this option is selected, the review is completed after one of the decision makers makes their decision.<br>This option is disabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Require decisions to be electronically signed</td> 
     <td>Users are required to specify their user name and password at the time that they make a decision on&nbsp;a <span>proof</span>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Lock <span>proof</span> when all required decisions are made</td> 
     <td>When this setting is enabled, the <span>proof</span> state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.<br>This option is disabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Download original file</td> 
     <td>When this option is selected, reviewers are able to download the original file from which the <span>proof</span> was created.<br>When this option is deselected, the Download icon is no longer visible.<br>This option is enabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Share <span>proof</span> via public URL or embed code</td> 
     <td>When this option is selected, the <span>proof</span> can be shared via a public URL or embed code.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Subscribe to <span>proof</span> via public URL or embed code</td> 
     <td>When this option is selected, people who have not been added explicitly to the <span>proof</span> can subscribe to the <span>proof</span>. The person subscribing to the <span>proof</span> is granted the role and email that you define in the following settings:
      <ul>
       <li><span class="bold">Subscriber role:</span>&nbsp;The default <span>proof</span> role that is&nbsp;assigned to all reviewers that subscribe to the <span>proof</span>.&nbsp;</li>
       <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <span>proof</span>.</li>
      </ul><p>
       <ul>
        <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <span>proof</span>. You can select <span class="bold">No email</span> (email link is not required to access the <span>proof</span>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <span>proof</span> via email without any verification), or <span class="bold">Validation and <span>proof</span> notification emails</span> (subscriber receives a link to the <span>proof</span> via email and must click the link to access a <span>proof</span>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
       </ul><note type="note">
        &nbsp;If the 
        <span>proofs</span> have Automated Workflow attached all subscriptions will generate confirmation emails to the 
        <span>proof</span> Owners, so they could decide which stage the person should be added to.
        <br>
       </note></p></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2"> <p>Click <span class="bold">Create Proof</span>.</p> <p><span>Workfront</span>&nbsp;begins generating a <span>proof</span> of the selected documents or websites.&nbsp;Depending on the file size and type, the lag time on a document upload can vary. Be patient as bigger files take longer to generate. You can navigate away from the page and <span>Workfront</span>&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.<br></p> </li> 
 <li value="3"> <p>After&nbsp;the <span>proof</span> is generated, click&nbsp;<span class="bold">Open proof</span>&nbsp;to launch the <span>proofing viewer</span>.</p> <p>  </p> <p>Users who do not have <span>proofing</span> enabled on their account&nbsp;are still able to view the document and make comments to the proof<a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md">.</a><br></p> </li> 
</ol>

