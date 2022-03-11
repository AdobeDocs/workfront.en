---
filename: configure-basic-proof-workflow
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Create an advanced proof with a Basic workflow
description: With a basic workflow, you can several reviewers to a proof, but they are not organized into stages. All of the reviewers you add can access the proof immediately after you create it.
---

# Create an advanced `proof` with a Basic workflow

With a basic workflow, you can several reviewers to a `proof`, but they are not organized into stages. All of the reviewers you add can access the `proof` immediately after you create it.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Higher</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Proof Permission Profile</span> </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or `Proof Permission Profile` you have, contact your `Workfront` or `Workfront Proof administrator`.

## Create an advanced `proof` with a Basic workflow

1. Go to the project, task, or issue where you want the `proof`, then click the `Documents` tab.
1. Click `Add new` > `Proof`, upload the content, then work through the sections listed below.

   or

   Hover over an existing document, then click the `Create Proof` > `Advanced `Proof`` and work through the sections listed below.

## Configure the workflow and add reviewers

<ol> 
 <li value="1">In the Workflow type section, choose <span class="bold">Basic</span>.</li> 
 <li value="2"> <p>Specify the users you want to add, then choose a Proof role.</p> <p> <img src="assets/new-proof---roles-350x213.png" style="width: 350;height: 213;"> </p> </li> 
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
     <th> <p><span class="bold">Delete comments made by others</span> </p> </th> 
     <th>Resolve comments</th> 
     <th>Apply Actions to Comments</th> 
     <th> <p><span class="bold">Edit the <span>proof</span></span> </p> </th> 
     <th>Share the <span>proof</span> with others</th> 
     <th>Create new version</th> 
     <th> <p><span class="bold">View approval requests in the Home area</span> </p> </th> 
     <th>Add new reviewers</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td> <p><span class="bold">Read Only</span> </p> </td> 
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
     <td> <p><span class="bold">Reviewer</span> </p> </td> 
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
     <td> <p><span class="bold">Approver</span> </p> </td> 
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
     <td> <p><span class="bold">Reviewer & Approver</span> </p> </td> 
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
     <td> <p><span class="bold">Author</span> </p> </td> 
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
     <td>&nbsp;</td> 
    </tr> 
    <tr> 
     <td> <p><span class="bold">Moderator</span> </p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p>✓</p> </td> 
     <td> <p><span class="bold">✓</span> </p> </td> 
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
  </table> </p> *Read-only and Reviewer roles are automatically granted View access on the document if they had none previously. <note type="note">
  Users on new Workfront plans can grant author or moderator roles to any users in the system. Users on legacy plans can grant author or moderator roles to any user with a proof license in the system.
 </note> 
 <li value="3"> <p>(Optional) With the drop-down menu still open, select any additional permissions available at the bottom of the menu:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Resolve comments and apply actions</span> </td> 
     <td> <p>Allows the <span>Workfront</span> user to do the following:</p> 
      <ul> 
       <li>Resolve a comment after it has been addressed, as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Resolve proof comments</a>.</li> 
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
 <li value="4">Repeat steps 1-3 for any other users you have added to the <span>proof</span>.</li> 
 <li value="5"> <p>For each user you are sharing with, in the <span class="bold">Email alerts</span>&nbsp;drop-down list, select the type of email alerts this user receives when people make comments and decisions on the proof:</p> 
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
 <li value="6">Continue with <a href="#configur2" class="MCXref xref">Configure email settings for the proof</a> below.</li> 
</ol>

## Configure email settings for the proof

<ol> 
 <li value="1"> <p>In the <span class="bold">Email notification</span> section, select whether to send email notifications and a custom message to&nbsp;the users you selected in <a href="#workflow" class="MCXref xref">Create an advanced proof with a Basic workflow</a> earlier in this article:</p> 
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
</ol>

1. Continue with [Configure proof settings](#configur3) below.

## Configure `proof` settings

<ol> 
 <li value="1"> <p>In the <span class="bold">Proof settings</span> section, select any of the following options:</p> 
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

