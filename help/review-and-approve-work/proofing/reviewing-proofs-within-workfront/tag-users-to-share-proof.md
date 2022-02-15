---
filename: tag-users-to-share-proof
product-area: documents;user-management;resource-management
navigation-topic: review-proofs-within-workfront
---



# Tag users to share a *`proof`* {#tag-users-to-share-a-proof}

When you are commenting on a *`proof`* in the *`proofing viewer`*, you can tag other users to bring their attention to your comment via email and to add them to the *`proof`*'s workflow.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Tag users to share a *`proof`* {#tag-users-to-share-a-proof-1}

If you are using an integrated *`proofing`* account ( *`Adobe Workfront`* integrated with *`Workfront Proof`*), you can tag anyone, including external collaborators, if at least one of the following is true:



* You are the *`proof`* creator or owner.
*  You have the Author or Moderator *`proof`* role on the *`proof`*. For information about the Author and Moderator roles, see [Proof Roles overview](proof-roles.md).
*  You have the *`Proof Permission Profile`* of Administrator or Supervisor.


  >[!NOTE]
  >
  >Your *`Workfront administrator`* assigns your *`Proof Permission Profile`*. For more information about *`Proof Permission Profiles`*, see [Proof Permission Profile overview](permission-profiles.md).



* When adding you to the *`proof`*, the *`proof`* creator gave you permission to share the proof by tagging users. For more information, see [Create an advanced proof with a Basic workflow](configure-basic-proof-workflow.md).



If none of the above are true, you can tag only the proof owner and any users who have been added previously to the proof's workflow.


>[!NOTE]
>
>You can tag an external collaborator using their email address only if either of the following is true:
>
>
>
>* A user in your organization's *`Workfront`* account has added the collaborator's email address to a *`proof`* previously.
>
>* The collaborator has used the email address to subscribe to a *`proof`* in your organization's *`Workfront`* account previously.
>
>
>



To tag someone in a comment:



1.  As you comment on a proof, type an at sign (@) followed by the person's name or email address. (For information about commenting on a *`proof`*, see [Create and manage proof comments](create-manage-proof-comments.md).)


   When you start typing, available names appear in a drop-down list.

1.   Select the person's name when you see it in the drop-down list. 


   If you want to close the drop-down list without selecting anyone, you can press the `Esc` key or click anywhere outside the list.

1. Repeat steps 1-2 for any other users you want to tag in the comment.
1. Finish the comment, then click `Post`.
1.  (Conditional) If you tagged anyone who was not already added to the *`proof`*, specify a `Proof role` and `Email alerts` setting for each user listed in the box that appears, then click `Add people and post comment`.


   ![](assets/add-people-to-proof-350x220.png)




   For information about *`proof`* roles, see [Configure default proofing roles](configure-default-proofing-roles.md). For information about proof email alerts, see the section in the article [Configure email notification settings in Workfront Proof](config-email-notification-settings-wp.md).


   If the *`proof`* has an Automated Workflow, the users you tag are added to the stage you are in. For more information, see [Automated Workflow overview](automated-workflow.md).


   Anyone you tag receives a notification email about your proof comment, regardless of the *`proof`* email alert settings they are using:

    
    
    * If the user receives a daily summary or hourly summary email, *`Workfront`* sends the notification separately and includes information about your proof comment in the summary email.
    *  If the user receives alerts for all activity, or for replies made to their comments, the notification replaces the notifications about these comments and replies.
    
    



For information about other ways to add users to a *`proof`*, see [Share a proof within Adobe Workfront](share-a-proof-in-workfront.md).
