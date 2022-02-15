---
filename: config-email-notification-settings-wp
product: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
---



# Configure email notification settings in *`Workfront Proof`* {#configure-email-notification-settings-in-workfront-proof}



>[!IMPORTANT] {type="important"}
>
>This article refers to functionality in the standalone product *`Workfront Proof`*. For information on proofing inside *`Adobe Workfront`*, see [Proofing](_proofing.md).


Email notifications inform collaborators about recent activity on *`proofs`*, such as comments, replies, decisions.


Email notifications for reviewers can be set on the New *`proof`* page, New version page, and managed in the Workflow section of the Proof details page. For more information, see [Generate Proofs in Workfront Proof](generate-proofs.md)



* [Generate Proofs in Workfront Proof](generate-proofs.md) [Generate Proofs in Workfront Proof](generate-proofs.md) 

* [Manage Proof Details in Workfront Proof](manage-proof-details.md).


Every user can also set their own email alert settings that will be automatically applied when a *`proof`* is shared with them. If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a *`proof`* default on the users details pages.


>[!NOTE]
>
>These settings are suggested when users are creating the *`proofs`* and are adding these collaborators. However, these are suggestions only, so they can be adjusted at any time during the review process and the changes apply to all the activity made after the change.  *`Proof`* default settings are overridden by the settings at *`proof`* level.


Users with Administrator or Billing Administrator profiles can also set the *`proof`* defaults for other users in their account from within Account settings.


For information about profiles, see [Proof Permissions Profiles in Workfront Proof](proof-perm-profiles-in-wp.md).



* [Configure proof defaults in personal settings (Workfront Proof users only)](#configur2) 
* [Change email alerts for a recipient](#changing-email-alerts-recipient) 
* [Configure proof defaults for a user](#configur) 




## Configure *`proof`* defaults in personal settings ( *`Workfront Proof`* users only) {#configure-proof-defaults-in-personal-settings-workfront-proof-users-only}

You can configure *`proof`* settings for *`proof`*s you create.&nbsp;


For information about proof settings the *`Workfront administrator`* or *`Workfront Proof administrator`* can configure, see [Configure proof settings for your organization](configure-proofing-organization.md).



1. Click `Settings` > `Personal settings`.

1. Click the `Proofing defaults` tab.
1. Click `Default email notification settings` to expand it.
1.  In the drop-down list to the right of the following two settings, select one of the options explained in the table below.

    
    
    * `Default email alert`: Affects every *`proof`* that is shared with you. This setting can be overridden at the *`proof`* level.
    
    *  `Default email alert for new guest reviewers`: Affects reviewers that did not previously exist as contacts in your account. 
    
    


   >[!NOTE]
   >
   >If you do not choose one of the following options, *`Workfront Proof`* sends you a daily summary about activity on your *`proofs`*.



<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 175px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">All activity</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email to the reviewer every time there is any activity on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the <span class="mc-variable WFVariables.proof-gerund variable varname">proofing</span> process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Replies to my comments</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> so that they are not&nbsp;notified of any other comments&nbsp;on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> in&nbsp;the <span class="mc-variable WFVariables.PV variable varname">proofing viewer</span>.</p><p>For information about comments, see <a href="create-manage-proof-comments.md" class="MCXref xref">Create and manage proof comments</a>.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Decisions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email to the reviewer only when someone makes a&nbsp;decision.<p>This can be useful for the person who is managing the approval process&nbsp;(such as a project manager) and&nbsp;needs to monitor progress on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> and see which users have&nbsp;made their&nbsp;decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Final decision</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email when the last approver on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> has made their&nbsp;decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.</p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Hourly Summary</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the hour.<p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Daily Summary</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="create-manage-proof-comments.md" class="MCXref xref">Create and manage proof comments</a> and <a href="make-decisions-on-proof.md" class="MCXref xref">Make decisions on a proof</a>.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">No email</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> have this setting.</p></td> 
  </tr> 
 </tbody> 
</table>


1.  Change any of the following: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Email confirmation when proofs are ready</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify whether you want to receive a Proof made email when you create a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. For more information, see <a href="proof-made-email.md" class="MCXref xref">The Proof Made email</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Format of emails sent to me</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Choose between HTML styled emails and Plain text emails. </p> <p>Note: &nbsp;Proofing default settings are overridden by the settings at <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> level. However, if <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> email notifications are disabled for the whole account in Account settings, no email alerts will be sent to the collaborators even if the Disabled email alert is not selected on <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Under `Message settings`,&nbsp;change any of the following:






## Change email alerts for a recipient  {#change-email-alerts-for-a-recipient}

You can change email alerts for a particular recipient in a batch action.



1. Click  `Contacts` in the left navigation panel.
1. Click the `More` (three dot) menu for the recipient, then click `View member details` in the dropdown menu.

1. Open the `Shared items` section.
1. Select the checkbox to the left of each item for which you want to change the email alert.
1. Click `More` above the list of shared items, then click  `Change email alert` in the dropdown menu.

1. Change the email alert, then click `Submit`.




## Configure *`proof`* defaults for a user {#configure-proof-defaults-for-a-user}

If you are a *`Workfront Proof administrator`*, you can set *`proof`* defaults for users in your account.



1. Click `Settings` > `Account settings`.&nbsp;

1. Open the `Users` tab.
1. Open the `More` menu to the right of the user's name. ![More_button_small.png](assets/more-button-small.png)


1. Click `View users details` in the dropdown menu.
1. Under `Settings`, click `Default email alert settings`&nbsp;to expand it.

1. In the drop-down list to the right of the following two settings, select one of the options explained in the table below:
    
    
    * `Default email alert`: Affects every *`proof`* that is shared with you. This setting can be overridden at the *`proof`* level.
    
    * `Default email alert for new guest reviewers`: Affects reviewers that did not previously exist as contacts in your account. 
    
    


   >[!NOTE]
   >
   >If you do not choose one of the following options for a user, *`Workfront Proof`* sends users a daily summary about activity on their *`proofs`*.



<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 175px;">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">All activity</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email to the reviewer every time there is any activity on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the <span class="mc-variable WFVariables.proof-gerund variable varname">proofing</span> process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Replies to my comments</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> so that they are not&nbsp;notified of any other comments&nbsp;on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> in&nbsp;the <span class="mc-variable WFVariables.PV variable varname">proofing viewer</span>.</p><p>For information about comments, see <a href="create-manage-proof-comments.md" class="MCXref xref">Create and manage proof comments</a>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Decisions</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email to the reviewer only when someone makes a&nbsp;decision.<p>This can be useful for the person who is managing the approval process&nbsp;(such as a project manager) and&nbsp;needs to monitor progress on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> and see which users have&nbsp;made their&nbsp;decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Final decision</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email when the last approver on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> has made their&nbsp;decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.</p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Hourly Summary</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an email to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the hour.<p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Daily Summary</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="create-manage-proof-comments.md" class="MCXref xref">Create and manage proof comments</a> and <a href="make-decisions-on-proof.md" class="MCXref xref">Make decisions on a proof</a>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">No email</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> have this setting.</p></td>
  </tr>
 </tbody>
</table>


1.   In the remaining `Default email alert settings`, change any of the following:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Email confirmation when <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> are ready</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify whether you want to receive a Proof made email when you create a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. For more information, see <a href="https://support.workfront.com/hc/en-us/article">The Proof Made Email.</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Format of emails sent to me</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Choose between HTML styled emails and Plain text emails. </p> <p>Note: &nbsp;Proofing default settings are overridden by the settings at <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> level. However, if <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> email notifications are disabled for the whole account in Account settings, no email alerts will be sent to the collaborators even if the Disabled email alert is not selected on <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>






##  

