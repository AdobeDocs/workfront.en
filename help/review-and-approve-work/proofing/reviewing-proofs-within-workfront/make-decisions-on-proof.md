---
filename: make-decisions-on-proof
product-area: documents
navigation-topic: review-proofs-within-workfront
---



# Make decisions on a *`proof`* {#make-decisions-on-a-proof}

The method you use to make a decision on a *`proof`* depends on whether the *`proof`* is configured with an Automated Workflow or with an approval. If you need more information about these two approval processes, see&nbsp;the following:



* [Create an advanced proof with an Automated workflow](create-automated-proof-workflow.md) 
* [Approving work](approving-work.md) 




>[!NOTE]
>
>A single *`proof`* should not include both decision types (Automated Workflow and approval).&nbsp;





You can make both *`proof`* approval decisions and *`Adobe Workfront`* approval decisions.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.



## Make a decision on a *`proof`* with an Automated Workflow {#make-a-decision-on-a-proof-with-an-automated-workflow}

You can make decisions on a *`proof`* in the *`proofing viewer`* if you are assigned one of the following roles in an Automated Workflow stage:



* Approver
* Reviewer & Approver
* Author
* Moderator


This section explains how to make a decision and change a decision on a *`proof`* with an Automated Workflow.



* [Make a decision on a proof](#making-a-decision-on-a-proof) 
* [Change a decision on a proof](#changing-your-decision) 




### Make a decision on a *`proof`* {#make-a-decision-on-a-proof}




1. Open the *`proof`* where you want to make a decision.
1.  Click `Make Decision` at the top-center of the *`proofing`* viewer.


  


1.  In the `Proof decision` box that appears, click one of the following decisions:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Approved</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is ready to move to the next stage of the Automated Workflow.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Approved with changes</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> requires some changes, but you do not need to see the revision before it moves to the next stage of the Automated Workflow.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Changes required</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> requires changes and you need to see another revision before it moves to the next stage of the Automated Workflow.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Not relevant</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is not relevant to you and you do not need to make a decision.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Custom decision</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>On Select and Premium plans, the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> or <span class="mc-variable WFVariables.AdminWFP variable varname">Workfront Proof administrator</span> can rename, reorder, and hide decisions.&nbsp;For more information,&nbsp;see&nbsp;<a href="configure-approval-decision-in-wp.md" class="MCXref xref">Configure approval decision options in Workfront Proof</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Conditional) If the *`Adobe Workfront administrator`* or *`Workfront Proof administrator`* has added a Reasons section, select any applicable reasons for your decision.


   For more information about how administrators can configure decision reasons, see&nbsp; [Configure approval decision options in Workfront Proof](configure-approval-decision-in-wp.md).

1. (Optional) Select `Send me an email confirmation`&nbsp;to receive an email confirmation of your decision.
1. Click `Make Decision`.




### Change a decision on a *`proof`* {#change-a-decision-on-a-proof}

As long as the *`proof`* is active (not locked or archived), you can change your decision at any time.&nbsp;



1. Open the *`proof`* where you want to change your decision.
1.  Click the decision you made at the top-center of the *`proofing viewer`*.
1. In the `Proof decision` box that appears, click `Remove decision` beneath the decision you made previously.





## Make a decision when the *`proof`* is configured with an approval process {#make-a-decision-when-the-proof-is-configured-with-an-approval-process}

You can make decisions on a *`proof`* when it is configured with an approval process (within *`Workfront`*) and&nbsp;a user has sent you a document approval request, as described in [Request document approvals](request-document-approvals.md).



* [Make a Workfront approval decision in a proof](#making-a-workfront-approval-decision-in-a-proof) 
* [Change your Workfront approval decision in a proof](#changing-your-workfront-approval-decision-in-a-proof) 




### Make a *`Workfront`* approval decision in a *`proof`* {#make-a-workfront-approval-decision-in-a-proof}




1.  Open the *`proof`* of the document that you want to make a decision on.
1. In the *`proofing viewer`*, select whether you want to `Approve`, require `Changes`, or `Reject` the approval request.





### Change your *`Workfront`* approval decision in a *`proof`* {#change-your-workfront-approval-decision-in-a-proof}




1. Open the *`proof`* of the document where you want to change your *`Workfront`* approval decision.

1.  At the top-center of the *`proofing viewer`*, click the decision you made previously.
1. In the `Proof decision` box that appears, select whether you want to `Approve`, require `Changes`, or `Reject` the approval request.



