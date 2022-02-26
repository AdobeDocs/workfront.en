---
filename: configure-basic-proof-workflow
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Create an advanced proof with a Basic workflow
description: With a basic workflow, you can several reviewers to a proof, but they are not organized into stages. All of the reviewers you add can access the proof immediately after you create it.
---

# Create an advanced *proof* with a Basic workflow

With a basic workflow, you can several reviewers to a *proof*, but they are not organized into stages. All of the reviewers you add can access the *proof* immediately after you create it.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Higher</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Proof Permission Profile</em> </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *Proof Permission Profile* you have, contact your *Workfront* or *Workfront Proof administrator*.

## Create an advanced *proof* with a Basic workflow

1. Go to the project, task, or issue where you want the *proof*, then click the `Documents` tab.
1. Click `Add new` > *Proof*, upload the content, then work through the sections listed below.

   or

   Hover over an existing document, then click the `Create Proof` > `Advanced *Proof*` and work through the sections listed below.

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
     <th> <p><span class="bold">View a <em>proof</em></span> </p> </th> 
     <th> <p><span class="bold">Add markups</span> </p> </th> 
     <th> <p><span class="bold">Add comments</span> </p> </th> 
     <th> <p><span class="bold">Edit own comments if there are no replies</span> </p> </th> 
     <th> <p><span class="bold">Make a decision</span> </p> </th> 
     <th> <p><span class="bold">Delete comments made by others</span> </p> </th> 
     <th>Resolve comments</th> 
     <th>Apply Actions to Comments</th> 
     <th> <p><span class="bold">Edit the <em>proof</em></span> </p> </th> 
     <th>Share the <em>proof</em> with others</th> 
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
  </table> </p> <draft-comment>
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   *Read-only and Reviewer roles are automatically granted View access on the document if they had none previously.
  </MadCap:conditionalText>
 </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  *Read-only and Reviewer roles are automatically granted View access on the document if they had none previously.
 </MadCap:conditionalText> <note type="note">
  Users on new Workfront plans can grant author or moderator roles to any users in the system. Users on legacy plans can grant author or moderator roles to any user with a proof license in the system.
 </note> 
 <li value="3"> <p>(Optional) With the drop-down menu still open, select any additional permissions available at the bottom of the menu:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Resolve comments and apply actions</span> </td> 
     <td> <p>Allows the <em>Workfront</em> user to do the following:</p> 
      <ul> 
       <li>Resolve a comment after it has been addressed, as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Resolve proof comments</a>.</li> 
       <li>Apply actions to comments, as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Use actions on proof comments</a>. </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Share proof by tagging</span> </td> 
     <td> <p>Allows the reviewer to add any <em>Workfront</em> user to the <em>proof</em> as explained in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Tag users to share a proof</a>.</p> <note type="note"> 
       <p>If these two options are unavailable (dimmed), the user already has a permission profile that allows resolving comments, applying actions to comments, and tagging any user. </p> 
       <p>If the options do not display, the person you added is not a <em>Workfront</em> license holder.</p> 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">Repeat steps 1-3 for any other users you have added to the <em>proof</em>.</li> 
 <li value="5"> <p>For each user you are sharing with, in the <span class="bold">Email alerts</span>&nbsp;drop-down list, select the type of email alerts this user receives when people make comments and decisions on the proof:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">All activity</td> 
     <td><em>Workfront</em> sends an email to the reviewer every time there is any activity on the <em>proof</em>, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the <em>proofing</em> process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Replies to my comments</td> 
     <td>An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the <em>proof</em> makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the <em>proof</em> so that they are not&nbsp;notified of any other comments&nbsp;on the <em>proof</em>, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the <em>proof</em> in&nbsp;the <em>proofing viewer</em>.</p><p>For information about comments, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Decisions</td> 
     <td><em>Workfront</em> sends an email to the reviewer only when someone makes a&nbsp;decision.<p>This can be useful for the person who is managing the approval process&nbsp;(such as a project manager) and&nbsp;needs to monitor progress on the <em>proof</em> and see which users have&nbsp;made their&nbsp;decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Final decision</td> 
     <td><em>Workfront</em> sends an email when the last approver on the <em>proof</em> has made their&nbsp;decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.</p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Hourly Summary</td> 
     <td><em>Workfront</em> sends an email to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the hour.<p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the <em>proof</em>.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Daily Summary</td> 
     <td><em>Workfront</em> sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td> 
    </tr> <draft-comment>
     <tr data-mc-conditions=""> 
      <td role="rowheader">No email</td> 
      <td><em>Workfront</em> does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a <em>proof</em> only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your <em>proofs</em> have this setting.</p></td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions=""> 
     <td role="rowheader">No email</td> 
     <td><em>Workfront</em> does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a <em>proof</em> only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your <em>proofs</em> have this setting.</p></td> 
    </tr> <draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <td role="rowheader">Set a deadline</td> 
      <td>Select the day and time when users must take action on the <em>proof</em>.<p>If you are adding users to a <em>proof</em> for a document&nbsp;that already exists in <em>Workfront</em>, you should have already set a deadline.</p></td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
     <td role="rowheader">Set a deadline</td> 
     <td>Select the day and time when users must take action on the <em>proof</em>.<p>If you are adding users to a <em>proof</em> for a document&nbsp;that already exists in <em>Workfront</em>, you should have already set a deadline.</p></td> 
    </tr> <draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <td role="rowheader">Notify people by email</td> 
      <td>Select this option to send an email to the users, notifying them of the <em>proof</em>.<p>Click <span class="bold">Add a custom message</span>&nbsp;to specify a message to include in the email notification.</p></td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
     <td role="rowheader">Notify people by email</td> 
     <td>Select this option to send an email to the users, notifying them of the <em>proof</em>.<p>Click <span class="bold">Add a custom message</span>&nbsp;to specify a message to include in the email notification.</p></td> 
    </tr> 
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
     <td role="rowheader">Notify recipients about this <em>proof</em></td> 
     <td>Select this option to send an email notification to users. When <span class="bold">Basic sharing</span> is selected in the <span class="bold">Workflow</span> section, an email notification is sent when the <em>proof</em> is created. When <span class="bold">Automated workflow</span> is selected in the <span class="bold">Workflow</span> section, an email notification is sent when the <em>proof</em> enters the stage of the Automated Workflow that the user is associated with.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Add custom message</td> 
     <td>Select this option to include a custom message in the notification. You can specify a subject and message body. The message body can include rich text formatting, such as bold, bullets, and hyperlinks.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

1. Continue with [Configure proof settings](#configur3) below.

## Configure *proof* settings

<ol> 
 <li value="1"> <p>In the <span class="bold">Proof settings</span> section, select any of the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Require login - proof can only be shared with other users</td> 
     <td>When this option is disabled (default), anyone with the URL is able to view the <em>proof</em>. <br>When this option is selected:
      <ul>
       <li>Only <em>Workfront Proof</em>&nbsp;users are able to view the <em>proof</em>.</li>
       <li>Users cannot sign in to the <em>proof</em> unless they have been added to the <em>proof</em>.</li>
       <li>Subscriptions cannot be enabled.</li>
      </ul></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Only one decision required for this <em>proof</em></td> 
     <td>When this option is selected, the review is completed after one of the decision makers makes their decision.<br>This option is disabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Require decisions to be electronically signed</td> 
     <td>Users are required to specify their user name and password at the time that they make a decision on&nbsp;a <em>proof</em>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Lock <em>proof</em> when all required decisions are made</td> 
     <td>When this setting is enabled, the <em>proof</em> state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.<br>This option is disabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Download original file</td> 
     <td>When this option is selected, reviewers are able to download the original file from which the <em>proof</em> was created.<br>When this option is deselected, the Download icon is no longer visible.<br>This option is enabled by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Share <em>proof</em> via public URL or embed code</td> 
     <td>When this option is selected, the <em>proof</em> can be shared via a public URL or embed code.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Subscribe to <em>proof</em> via public URL or embed code</td> 
     <td>When this option is selected, people who have not been added explicitly to the <em>proof</em> can subscribe to the <em>proof</em>. The person subscribing to the <em>proof</em> is granted the role and email that you define in the following settings:
      <ul>
       <li><span class="bold">Subscriber role:</span>&nbsp;The default <em>proof</em> role that is&nbsp;assigned to all reviewers that subscribe to the <em>proof</em>.&nbsp;</li>
       <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <em>proof</em>.</li>
      </ul><p>
       <ul>
        <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <em>proof</em>. You can select <span class="bold">No email</span> (email link is not required to access the <em>proof</em>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <em>proof</em> via email without any verification), or <span class="bold">Validation and <em>proof</em> notification emails</span> (subscriber receives a link to the <em>proof</em> via email and must click the link to access a <em>proof</em>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
       </ul><note type="note">
        &nbsp;If the 
        <em>proofs</em> have Automated Workflow attached all subscriptions will generate confirmation emails to the 
        <em>proof</em> Owners, so they could decide which stage the person should be added to.
        <br>
       </note></p></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2"> <p>Click <span class="bold">Create Proof</span>.</p> <p><em>Workfront</em>&nbsp;begins generating a <em>proof</em> of the selected documents or websites.&nbsp;Depending on the file size and type, the lag time on a document upload can vary. Be patient as bigger files take longer to generate. You can navigate away from the page and <em>Workfront</em>&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.<br></p> </li> 
 <li value="3"> <p>After&nbsp;the <em>proof</em> is generated, click&nbsp;<span class="bold">Open proof</span>&nbsp;to launch the <em>proofing viewer</em>.</p> <p> <draft-comment>
    <img src="assets/open-proof-350x132.png" style="width: 350;height: 132;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/open-proof-350x132.png" style="width: 350;height: 132;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>Users who do not have <em>proofing</em> enabled on their account&nbsp;are still able to view the document and make comments to the proof<a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md">.</a><br></p> </li> 
</ol>

