---
filename: config-email-notification-settings-wp
product: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configure email notification settings in Workfront Proof
description: Important: This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see Proofing.
---

# Configure email notification settings in *Workfront Proof*

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product *Workfront Proof*. For information on proofing inside *Adobe Workfront*, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Email notifications inform collaborators about recent activity on *proofs*, such as comments, replies, decisions.

Email notifications for reviewers can be set on the New *proof* page, New version page, and managed in the Workflow section of the Proof details page. For more information, see [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) 

* [Manage Proof Details in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Every user can also set their own email alert settings that will be automatically applied when a *proof* is shared with them.&nbsp;If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a *proof* default on the users details pages.

>[!NOTE]
>
>These settings are suggested when users are creating the *proofs* and are adding these collaborators. However, these are suggestions only, so they can be adjusted at any time during the review process and the changes apply to all the activity made after the change.&nbsp;*Proof* default settings are overridden by the settings at *proof* level.

Users with Administrator or Billing Administrator profiles can also set the *proof* defaults for other users in their account from within Account settings.

For information about profiles, see [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Configure proof defaults in personal settings (Workfront Proof users only)](#configur2) 
* [Change email alerts for a recipient](#changing-email-alerts-recipient) 
* [Configure proof defaults for a user](#configur)

## Configure *proof* defaults in personal settings (*Workfront Proof* users only)

You can configure *proof* settings for *proof*s you create.&nbsp;

For information about proof settings the *Workfront administrator* or *Workfront Proof administrator* can configure, see [Configure proof settings for your organization](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

<ol> 
 <li value="1">Click <span class="bold">Settings</span> > <span class="bold">Personal settings</span>.</li> 
 <li value="2">Click the <span class="bold">Proofing defaults</span> tab.</li> 
 <li value="3">Click <span class="bold">Default email notification settings</span> to expand it.</li> 
 <li value="4"> <p>In the drop-down list to the right of the following two settings, select one of the options explained in the table below.</p> 
  <ul> 
   <li><span class="bold">Default email alert</span>: Affects every <em>proof</em> that is shared with you. This setting can be overridden at the <em>proof</em> level.</li> 
   <li> <p><span class="bold">Default email alert for new guest reviewers</span>: Affects reviewers that did not previously exist as contacts in your account. </p> </li> 
  </ul> <note type="note">
   If you do not choose one of the following options, 
   <em>Workfront Proof</em> sends you a daily summary about activity on your 
   <em>proofs</em>.
  </note> 
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
 <li value="5"> <p>Change any of the following: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Email confirmation when proofs are ready</td> 
     <td>Specify whether you want to receive a Proof made email when you create a <em>proof</em>. For more information, see <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a></td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Format of emails sent to me</span> </td> 
     <td> <p>Choose between HTML styled emails and Plain text emails. </p> <note type="note">
       &nbsp;Proofing default settings are overridden by the settings at 
       <em>proof</em> level. However, if 
       <em>proof</em> email notifications are disabled for the whole account in Account settings, no email alerts will be sent to the collaborators even if the Disabled email alert is not selected on 
       <em>proofs</em>.
       <br>
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Under <span class="bold">Message settings</span>,&nbsp;change any of the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Proof subject template</span> </td> 
     <td>Displays on the New proof page, New version page, Message page and Remind page. Can be edited before it's sent.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Proof message template</span> </td> 
     <td>Displays on the New proof page, New version page, Message page, and Remind page. Can be edited before it's sent.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

## Change email alerts for a recipient

You can change email alerts for a particular recipient in a batch action.

1. Click  `Contacts` in the left navigation panel.
1. Click the `More` (three dot) menu for the recipient, then click `View member details` in the dropdown menu.

1. Open the `Shared items` section.
1. Select the checkbox to the left of each item for which you want to change the email alert.
1. Click `More` above the list of shared items, then click  `Change email alert` in the dropdown menu.

1. Change the email alert, then click `Submit`.

## Configure *proof* defaults for a user

If you are a *Workfront Proof administrator*, you can set *proof* defaults for users in your account.

<ol> 
 <li value="1">Click <span class="bold">Settings</span> > <span class="bold">Account settings</span>.&nbsp;</li> 
 <li value="2">Open the <span class="bold">Users</span> tab.</li> 
 <li value="3">Open the <span class="bold">More</span> menu to the right of the user's name. <img src="assets/more-button-small.png" alt="More_button_small.png"></li> 
 <li value="4">Click <span class="bold">View users details</span> in the dropdown menu.</li> 
 <li value="5">Under <span class="bold">Settings</span>, click <span class="bold">Default email alert settings</span>&nbsp;to expand it.</li> 
 <li value="6">In the drop-down list to the right of the following two settings, select one of the options explained in the table below:
  <ul>
   <li><span class="bold">Default email alert</span>: Affects every <em>proof</em> that is shared with you. This setting can be overridden at the <em>proof</em> level.</li>
   <li><p><span class="bold">Default email alert for new guest reviewers</span>: Affects reviewers that did not previously exist as contacts in your account. </p></li>
  </ul><note type="note">
   If you do not choose one of the following options for a user, 
   <em>Workfront Proof</em> sends users a daily summary about activity on their 
   <em>proofs</em>.
  </note>
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
    </tr><draft-comment>
     <tr data-mc-conditions="">
      <td role="rowheader">No email</td>
      <td><em>Workfront</em> does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a <em>proof</em> only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your <em>proofs</em> have this setting.</p></td>
     </tr>
    </draft-comment>
    <tr data-mc-conditions="">
     <td role="rowheader">No email</td>
     <td><em>Workfront</em> does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a <em>proof</em> only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your <em>proofs</em> have this setting.</p></td>
    </tr><draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
      <td role="rowheader">Set a deadline</td>
      <td>Select the day and time when users must take action on the <em>proof</em>.<p>If you are adding users to a <em>proof</em> for a document&nbsp;that already exists in <em>Workfront</em>, you should have already set a deadline.</p></td>
     </tr>
    </draft-comment>
    <tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
     <td role="rowheader">Set a deadline</td>
     <td>Select the day and time when users must take action on the <em>proof</em>.<p>If you are adding users to a <em>proof</em> for a document&nbsp;that already exists in <em>Workfront</em>, you should have already set a deadline.</p></td>
    </tr><draft-comment>
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
  </table></li> 
 <li value="7"> <p> In the remaining <span class="bold">Default email alert settings</span>, change any of the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Email confirmation when <em>proofs</em> are ready</td> 
     <td>Specify whether you want to receive a Proof made email when you create a <em>proof</em>. For more information, see <a href="https://support.workfront.com/hc/en-us/article">The Proof Made Email.</a></td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Format of emails sent to me</span> </td> 
     <td> <p>Choose between HTML styled emails and Plain text emails. </p> <note type="note">
       &nbsp;Proofing default settings are overridden by the settings at 
       <em>proof</em> level. However, if 
       <em>proof</em> email notifications are disabled for the whole account in Account settings, no email alerts will be sent to the collaborators even if the Disabled email alert is not selected on 
       <em>proofs</em>.
       <br>
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

##  

