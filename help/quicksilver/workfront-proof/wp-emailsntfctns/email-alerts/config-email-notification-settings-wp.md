---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configure email notification settings in [!DNL Workfront Proof]
description: Email notifications generated from Workfront Proof inform collaborators about recent activity on proofs, such as comments, replies, or decisions.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
---
# Configure email notification settings in [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Email notifications inform collaborators about recent activity on proofs, such as comments, replies, or decisions.

You can set email notifications for reviewers in the following areas: 

* The New proof page
* The [!UICONTROL New version] page
* The [!UICONTROL Workflow] section of the [!UICONTROL Proof details] page. 

For more information, see [Generate Proofs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Generate Proofs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Generate Proofs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Manage Proof Details in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Every user can also set their own email alert settings that will be automatically applied when a proof is shared with them. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>These settings are suggested when users are creating the proofs and are adding these collaborators. However, these are suggestions only, so they can be adjusted at any time during the review process and the changes apply to all the activity made after the change. Proof default settings are overridden by the settings at proof level.

Users with [!UICONTROL Administrator] or [!UICONTROL Billing Administrator] profiles can also set the proof defaults for other users in their account from within Account settings.

For information about profiles, see [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Configure proof defaults in personal settings ([!DNL Workfront Proof] users only)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [Change email alerts for a recipient](#change-email-alerts-for-a-recipient)
* [Configure proof defaults for a user](#configure-proof-defaults-for-a-user)

## Configure proof defaults in personal settings ([!DNL Workfront Proof] users only) 

You can configure proof settings for proofs you create. 

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Click **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]**.

1. Click the **[!UICONTROL Proofing defaults]** tab.
1. Click **[!UICONTROL Default email notification settings]** to expand it.
1. In the drop-down list to the right of the following two settings, select one of the options explained in the table below.

   * **[!UICONTROL Default email alert]**: Affects every proof that is shared with you. This setting can be overridden at the proof level.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Affects reviewers that did not previously exist as contacts in your account.

   >[!NOTE]
   >
   >If you do not choose one of the following options, [!DNL Workfront Proof] sends you a daily summary about activity on your proofs.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>[!UICONTROL Workfront] sends an email to the reviewer every time there is any activity on the proof, such as a new comment, reply, or decision. <p>This is a great option for the person who is managing the proofing process because it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Replies to my comments]</td> 
      <td>An email is sent to the reviewer only if someone replies explicitly to their comment (this excludes their own replies on their own comments). This means that if somebody on the proof makes a new comment, the reviewer is not notified.<p>This setting is recommended for your clients on the proof so that they are not notified of any other comments on the proof, and are notified only of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new comments, they can still view all comments on the proof in the proofing viewer.</p><p>For information about comments, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] sends an email to the reviewer only when someone makes a decision.<p>This can be useful for the person who is managing the approval process (such as a project manager) and needs to monitor progress on the proof and see which users have made their decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Final decision]</td> 
      <td>[!DNL Workfront] sends an email when the last approver on the proof has made their decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is notified and can then take action on any necessary changes.</p><p>This alert can also be useful for a department leader who needs to be notified only when the review process is finished.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hourly Summary]</td> 
      <td>[!DNL Workfront] sends an email to the reviewer every hour with a summary of all the comments, replies, and decisions that have occurred in the hour.<p>The email is sent only when activity besides your own occurs within the past hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a senior reviewer who needs an overview of the project but does not need to be notified immediately of all activity on the proof.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Daily Summary]</td> 
      <td>[!DNL Workfront] sends one email with all comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project without being overwhelmed with multiple updates throughout the day.</p><p>An example use case for this summary is a department leader who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] does not send any email alerts.<br>This is useful for a person who is added to a proof only for reference purposes and does not need to be notified of any changes.<p>The system default is [!UICONTROL Daily summary] (also seen as [!UICONTROL Not Set]). If you or your reviewers do not make any other changes, all your proofs have this setting.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Change any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Specify whether you want to receive a [!UICONTROL Proof made] email when you create a proof. For more information, see <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The [!UICONTROL Proof Made] email</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>Choose between HTML styled emails and Plain text emails. </p> <p><b>NOTE</b></p>
      <p>Proofing default settings are overridden by the settings at proof level. However, if proof email notifications are disabled for the whole account in [!UICONTROL Account] settings, no email alerts will be sent to the collaborators even if the [!UICONTROL Disabled email alert] is not selected on proofs.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Under **[!UICONTROL Message settings]**, change any of the following:

   |Proof template |Description|
   |---|---|
   |**[!UICONTROL Proof subject template]** | Displays on the New proof page, New version page, Message page and Remind page. Can be edited before it's sent. |
      | **[!UICONTROL Proof message template]** | Displays on the New proof page, New version page, Message page, and Remind page. Can be edited before it's sent. |

## Change email alerts for a recipient

You can change email alerts for a particular recipient in a batch action.

1. Click **[!UICONTROL Contacts]** in the left navigation panel.
1. Click the **[!UICONTROL More]** menu ![](assets/more-button-small.png) for the recipient, then click **[!UICONTROL View member details]** in the dropdown menu.

1. Open the **[!UICONTROL Shared items]** section.
1. Select the checkbox to the left of each item for which you want to change the email alert.
1. Click **[!UICONTROL More]** above the list of shared items, then click **[!UICONTROL Change email alert]** in the dropdown menu.

1. Change the email alert, then click **[!UICONTROL Submit]**.

## Configure proof defaults for a user

If you are a [!DNL Workfront Proof] administrator, you can set proof defaults for users in your account.

1. Click **[!UICONTROL Settings]** > **[!UICONTROL Account settings]**. 

1. Open the **[!UICONTROL Users]** tab.
1. Open the **[!UICONTROL  More]** menu ![More_button_small.png](assets/more-button-small.png) to the right of the user's name. 

1. Click **[!UICONTROL View users details]** in the dropdown menu.
1. Under **[!UICONTROL Settings]**, click **[!UICONTROL Default email alert settings]** to expand it.

1. In the dropdown list to the right of the following two settings, select one of the options explained in the table below:

   * **[!UICONTROL Default email alert]**: Affects every proof that is shared with you. This setting can be overridden at the proof level.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Affects reviewers that did not previously exist as contacts in your account.

   >[!NOTE]
   >
   >If you do not choose one of the following options for a user, [!DNL Workfront Proof] sends users a daily summary about activity on their proofs.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] sends an email to the reviewer every time there is any activity on the proof, such as a new comment, reply, or decision. <p>This is a great option for the person who is managing the proofing process because it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Replies to my comments]</td>
      <td>An email is sent to the reviewer only if someone replies explicitly to their comment (this excludes their own replies on their own comments). This means that if somebody on the proof makes a new comment, the reviewer is not notified.<p>This setting is recommended for your clients on the proof so that they are not notified of any other comments on the proof, and are notified only of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new comments, they can still view all comments on the proof in the proofing viewer.</p><p>For information about comments, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] sends an email to the reviewer only when someone makes a decision.<p>This can be useful for the person who is managing the approval process (such as a project manager) and needs to monitor progress on the proof and see which users have made their decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Final decision]</td>
      <td>[!DNL Workfront] sends an email when the last approver on the proof has made their decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is notified and can then take action on any necessary changes.</p><p>This alert can also be useful for a department leader who needs to be notified only when the review process is finished.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Hourly Summary]</td>
      <td>[!DNL Workfront] sends an email to the reviewer every hour with a summary of all the comments, replies, and decisions that have occurred in the hour.<p>The email is sent only when activity besides your own occurs within the past hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a senior reviewer who needs an overview of the project but does not need to be notified immediately of all activity on the proof.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Daily Summary]</td>
      <td>[!DNL Workfront] sends one email with all comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project without being overwhelmed with multiple updates throughout the day.</p><p>An example use case for this summary is a department leader who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] does not send any email alerts.<br>This is useful for a person who is added to a proof only for reference purposes and does not need to be notified of any changes.<p>The system default is [!UICONTROL Daily summary] (also seen as [!UICONTROL Not Set]). If you or your reviewers do not make any other changes, all your proofs have this setting.</p></td>
     </tr>
    </tbody>
   </table>

1. In the remaining **[!UICONTROL Default email alert settings]**, change any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Specify whether you want to receive a [!UICONTROL Proof made] email when you create a proof. For more information, see <a href="https://support.workfront.com/hc/en-us/article">The [!UICONTROL Proof Made] Email.</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>Choose between HTML styled emails and Plain text emails. </p> <p><b>NOTE</b></p> <p>Proofing default settings are overridden by the settings at proof level. However, if proof email notifications are disabled for the whole account in [!UICONTROL Account] settings, no email alerts will be sent to the collaborators even if the [!UICONTROL Disabled email alert] is not selected on proofs.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
