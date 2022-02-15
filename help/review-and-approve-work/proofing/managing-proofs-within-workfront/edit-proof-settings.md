---
filename: edit-proof-settings
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
---



# Edit proof settings {#edit-proof-settings}

You can edit *`proof`* settings any time after you create a proof. 


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Edit proof settings {#edit-proof-settings-1}

Some settings may be locked if your *`Workfront administrator`* disabled them at the account level.



1.  Go to the project, task, or issue where you want the *`proof`*, then click the `Documents` tab.
1.  Mouse over the *`proof`*, then click `Document Details`.
1.  In the left panel, click `Proofing Viewer Settings`. 
1.  Adjust the following settings:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Require login. This proof cannot be shared with guest users</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>If you require higher levels of security for your review and approval process, you can use require login to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. This means that only <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>&nbsp;users can be added to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. They must enter their email and password before they can access it.</p> <p>Note: <em style="font-style: normal;">If Login required is enabled, Subscriptions cannot be enabled.</em> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Require decisions to be electronically signed</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>You can require an electronic signature of any reviewer who makes a decision on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. When&nbsp;a reviewer makes a decision, a prompt appears asking them to input their email and password and to confirm their decision. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Lock proof when all required decisions are made</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You can set a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> state to lock when the final Approver makes their decision. This is useful if you want to make sure that your reviewers won't be able to go back to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> and add additional comments or change their decisions.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Allow downloading the original file</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>You can allow reviewers on a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> to download the original file from which a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> was created. This is enabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Allow sharing proof via public URL or embed code</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">You can allow users to share the <span class="mc-variable WFVariables.proof-v variable varname">proof</span> with a public URL or embed code. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Allow subscribing to proof via public URL or embed code</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Enabling subscription on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> allows people who have not been added explicitly to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> to subscribe themselves to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> (i.e. add themselves to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>). They will then be assigned the role and email alert that you select for them in the Subscription settings.</p> <p>If Subscription has been enabled on a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, the fields below will become active:</p> 
    <ul> 
     <li><span class="bold">Subscriber validation required</span> - Subscriber must click a link in an email to access a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span><br>Selecting this option means that the person subscribing will not get immediate access to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, but will get a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> in an email. The purpose of subscriber validation is to ensure that the person has entered a correct email address to which they have access.</li> 
     <li><span class="bold">Default role for new subscribers -</span> This is the default <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> role that will be assigned to all reviewers that subscribe themselves to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</li> 
     <li><span class="bold">Default email alert for new subscribers</span>&nbsp;- This the default email alert that will be assigned to all reviewers that subscribe themselves to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


1. Click `Save`.


&nbsp;
