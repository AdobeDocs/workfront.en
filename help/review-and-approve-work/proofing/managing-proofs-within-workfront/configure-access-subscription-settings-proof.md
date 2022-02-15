---
filename: configure-access-subscription-settings-proof
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
---



# Configure access and subscription settings for a *`proof`* {#configure-access-and-subscription-settings-for-a-proof}

You can configure certain access and subscription settings for individual *`proofs`*, such as whether to require users to log in and whether to allow users to subscribe to the *`proof`*. You can set up access and subscription settings for a *`proof`* while you are creating it, or you can set them up for a *`proof`* that already exists in *`Workfront`*.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Configure access and subscription settings while creating a *`proof`* {#configure-access-and-subscription-settings-while-creating-a-proof}

To set up access and subscription settings for a *`proof`* while you are creating it:



1. Begin the process for generating a *`proof`* on a document or website, as described in the [Generate a proof](generate-proof.md) articles.

1. Scroll to the `Proof settings` section in the lower-right corner of the `New proof` page.

1.  Configure the following settings:  


<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Allow sharing proof via public URL or embed code</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">When this option is selected, the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> can be shared via a public URL or embed code.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Allow subscribing to proof via public URL or embed code</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">When this option is selected, people who have not been added explicitly to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> can subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. The person subscribing to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is granted the role and email that you define in the following settings:
    <ul>
     <li><p><span class="bold">Subscriber role:</span>&nbsp;The default <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> role that is&nbsp;assigned to all reviewers that subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.&nbsp;</p><p>Important: If <span class="bold">Allow Sharing With</span> is set to anything other than <span class="bold">Everyone</span> in the Workfront Proof settings, the subscription works only for people within the organization. For more information, see <a href="configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.</p></li>
     <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</li>
    </ul><p>
     <ul>
      <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. You can select <span class="bold">No email</span> (email link is not required to access the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via email without any verification), or <span class="bold">Validation and <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> notification emails</span> (subscriber receives a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via email and must click the link to access a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
     </ul><p>Note: &nbsp;If the <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> have Automated Workflow attached all subscriptions will generate confirmation emails to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> Owners, so they could decide which stage the person should be added to.<br></p></p></td> 
  </tr> 
 </tbody> 
</table>


1. Continue creating your proof.




## Configure access and subscription settings for an existing proof {#configure-access-and-subscription-settings-for-an-existing-proof}

To set up access and subscription settings for a *`proof`* that already exists in *`Workfront`*:



1. Generate the *`proof`* (if you have not already done so) as described in the [Generate a proof](generate-proof.md) articles.

1. In the Documents area, select the document that contains the *`proof`* you want to configure settings for, then click `Document Details`.

1. In the left panel, click `Proofing Viewer Settings`.
1.  Configure the following settings:  


<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Allow sharing proof via public URL or embed code</span><span class="bold">e</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">When this option is selected, the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> can be shared via a public URL or embed code.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Allow subscribing to proof via public URL or embed code</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">When this option is selected, people who have not been added explicitly to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> can subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. The person subscribing to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is granted the role and email that you define in the following settings:
    <ul>
     <li><p><span class="bold">Subscriber role:</span>&nbsp;The default <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> role that is&nbsp;assigned to all reviewers that subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.&nbsp;</p><p>Important: If <span class="bold">Allow Sharing With</span> is set to anything other than <span class="bold">Everyone</span> in the Workfront Proof settings, the subscription works only for people within the organization. For more information, see <a href="configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.</p></li>
     <li><span class="bold">Email alert settings for subscribers:</span>&nbsp;The default email alert that is assigned to all reviewers that subscribe to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</li>
    </ul><p>
     <ul>
      <li><span class="bold">Proof access via email link required for:</span>&nbsp;Configure whether the subscriber receives an email with a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. You can select <span class="bold">No email</span> (email link is not required to access the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>), <span class="bold">Proof notification email only</span> (subscriber receives a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via email without any verification), or <span class="bold">Validation and <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> notification emails</span> (subscriber receives a link to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> via email and must click the link to access a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</li>
     </ul><p>Note: &nbsp;If the <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> have Automated Workflow attached all subscriptions will generate confirmation emails to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> Owners, so they could decide which stage the person should be added to.<br></p></p></td> 
  </tr> 
 </tbody> 
</table>


1. Click `Save`.


