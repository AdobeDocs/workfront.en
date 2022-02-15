---
filename: share-a-proof-in-workfront
product-area: documents
navigation-topic: manage-proofs-within-workfront
---



# Share a *`proof`* within *`Adobe Workfront`* {#share-a-proof-within-adobe-workfront}

You can share a proofed document within *`Adobe Workfront`* by sharing the document or by adding users to the *`proof`*. 


If you share the *`proof`*, as explained in this article, your recipient has the same access to the document and the *`proof`*. In addition, you can request approval for the *`proof`* from the recipient.


>[!TIP] {type="tip"}
>
>You can also share a *`proof`* from within the *`proofing viewer`*. For instructions, see [Share a proof from the proofing viewer](share-a-proof-in-proofing-viewer.md).




## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Current plan: <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span></p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.proofPermissionProfile variable varname">Proof Permission Profile</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Manager or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Proof Role</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Author or Moderator</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Share a *`proof`* link {#share-a-proof-link}

Sharing a proof link grants *`Workfront`* users viewing access. Users can comment on the *`proof`* and subscribe to email notifications for the *`proof`* using their *`Workfront`* login credentials. Non- *`proofing`* users can comment and subscribe using an email address and display name.


>[!IMPORTANT] {type="important"}
>
>The Allow sharing proof via public URL or embed code setting must be enabled.





1.  Select the document that contains the *`proof`* you want to share with users.


   You can select only one document. You cannot share the link for multiple documents at the same time.

1.  Click `Share` > `Proof Link`.
1. In the `Proof link` box that appears, do either of the following:
1.  `<li> <p>To copy the link to your clipboard, click <span class="bold">Copy link</span>.</p> <p>You can now distribute the link via a third-party tool, such as a chat or an email application.</p> </li>` `<li>To email the link directly from <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span>, do the following: <ol>  <li value="1"><p>In the <span class="bold">Or email link to</span> field, begin typing and select the name of your recipient. Or specify the email address of an external user who you want to share with.</p></li>  <li value="2"><p>Select from the following options:</p>   <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 178px;">    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">    <tbody>     <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">      <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Send public link</td>      <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Includes a button in the email notification that directs users to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> within the <span class="mc-variable WFVariables.PV variable varname">proofing viewer</span> they are using and grants View access.</p><p>If <span class="bold">Subscribe to proof via public URL or embed code</span> is turned off for the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, users can sign in with their <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> login credentials to add comments to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. If it is turned on, anyone providing their email address and name (no password required) can sign and add comments to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</p></td>     </tr>     <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">      <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Send download link</td>      <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Includes a button in the email notification that directs users to a download page, which provides file details, file name, and file size, with the file displayed inline. Users can click the Download link from the download page to download the file.</td>     </tr>     <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Add custom message</td>      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Allows you to specify a custom subject and body for the email notification.</td>     </tr>    </tbody>   </table></li>  <li value="3"><p>Click <span class="bold">Send</span>.</p><p>Your recipients receive an email notification containing information about the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> and the buttons you chose to include.</p><p><img src="assets/proof-share-email-350x87.png" style="width: 350;height: 87;"></p></li> </ol></li>` 





## Add users to a *`proof`* {#add-users-to-a-proof}

You can add any *`Workfront`* user to the *`proof`* if you have Edit rights on the *`proof`*. If the *`proof`* has multiple stages, you add the user to an individual stage


>[!NOTE]
>
>Keep the following in mind if you are using a legacy *`Workfront`* plan in which *`proofing`* can be enabled and disabled for a user:
>
>
>
>* Your recipients do not need to have *`proofing`* enabled in order to review the *`proof`*.
>
>* When Automated Workflow is enabled and you add a user to the *`proof`* who does not have *`proofing`* enabled in *`Workfront`*, a new stage is created within the Automated Workflow. The user who you are adding is automatically added to this new stage when they view the *`proof`* for the first time. (For more information, see [Automated Workflow overview](automated-workflow.md).)
>
>
>





### Add users to an existing *`proof`* from the Documents tab {#add-users-to-an-existing-proof-from-the-documents-tab}




1. Select the document that contains the *`proof`* that you want to add users to.
1.  &nbsp;
1.  If the *`proof`* does not have an automated workflow (stages), click the `More` icon in the upper-right corner of the Stage 1 section, then click `Share` in the drop-down menu.


   Or


   If the *`proof`* does have an Automated Workflow, click the `More` icon in the upper-right corner of the stage where you want to add the reviewer, then click `Share` in the drop-down menu.

1. In the `Share this version` box that appears, under `Share`, begin typing the name or email address of a user who you want to share the *`proof`* with, then click the name when it appears in the drop-down list.

1. (Optional) Repeat this step to add multiple users to the *`proof`*.
1. (Optional) Set a deadline for the reviewers.
1. (Optional) Make sure `Notify people by email` is selected if you want to let the reviewers know you have added them to the *`proof`*.

1. (Optional) `Add a custom message` to the email.
1. When you have added all the reviewers, click `Share`.




### Add users to an existing *`proof`* from the *`proofing viewer`* {#add-users-to-an-existing-proof-from-the-proofing-viewer}

You can add users to a *`proof`* while you review a *`proof`* in the *`Web Proofing Viewer`* and in the *`Desktop Proofing Viewer`*.


For more information, see [Share a proof by adding users to it](share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) in the article [Share a proof from the proofing viewer](share-a-proof-in-proofing-viewer.md)


## Report on *`proofing`* approvals {#report-on-proofing-approvals}

You can create a report that reports on the *`proofing`* approvals that have been shared within *`Workfront`*. This report provides the following *`proof`* approval information in your system:



* Document that was submitted for approval
* Name of the approver
* Proof version
* Proof ID
* Proof creation date


You access this approval when creating a report based on an object, as described in [Create a custom report](create-custom-report.md).


For more information about the Proof Approvals object report, see the [Report on objects](understand-objects.md#reporting-on-objects) section in [Understand objects in Adobe Workfront](understand-objects.md)


## Approve a shared *`proof`* {#approve-a-shared-proof}

When a user adds you to a *`proof`* and grants either the Approver role or the Reviewer & Approver role using Automated Workflow, the approval request displays on the Approvals tab in your Home or My Work area. You can then view the *`proof`* and make an approval decision on the *`proof`* directly from *`Workfront`*.


For information about how to make approval decisions from the My Work area, see [Approve work from the Home area](approving-work.md#approving-work-from-the-home-area) or [Approving work](approving-work.md#approving-work-from-the-my-work-area) in [Approving work](approving-work.md).
