---
filename: disable-public-proofs
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
---



# Disable sharing proof via public URL or embed code {#disable-sharing-proof-via-public-url-or-embed-code}

You can turn off the ability to share a proof with a public URL or embed code on a proof by proof basis or for individual users.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Disable per *`Proof`* {#disable-per-proof}

You must be the *`proof`* owner or creator, or you must have the Author or Moderator proof role.



1.  In the project that contains the proof, click `Documents` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> in the left panel</MadCap:conditionalText>`.
1.  Hover over the proof and select`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  <span class="bold">Document Details</span></MadCap:conditionalText>` .
1.  In the left panel, click `Proofing Viewer Settings`, then disable the `Allow sharing proof via public URL or embed code` checkbox.


   ![](assets/proofing-viewer-settings-350x200.png)



1.  Click `Save`. 




## Disable per user {#disable-per-user}

You can disable the Public proof setting for individual users in your Workfront instance. You must have a *`Proof Permission Profile`* of administrator to make this change. 



1.   Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Proofing`.
1.  Click `Account Settings` near the top-right corner.
1.  Click the `Users` tab, then click on the name of a user.
1.  In the `Default proof settings` section, disable the `Public Sharing` checkbox. 


   ![](assets/default-proof-settings--public-sharing-350x210.png)





