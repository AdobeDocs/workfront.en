---
filename: generate-static-proof-website-other-web-content
product-area: documents
navigation-topic: create-proofs-within-workfront
---



# Create a static *`proof`* for a website or other web content {#create-a-static-proof-for-a-website-or-other-web-content}

You can generate a new static *`proof`* or a new version of an existing static *`proof`* for web content. Web content can include things like ads with streaming video, HTML animations, or interactive banners, but it will be cut into multiple screenshots to allow for static proofing. 


Consider the following when creating static *`proofs`* for a website or other web content:


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Create a static *`proof`* for a website or other web content {#create-a-static-proof-for-a-website-or-other-web-content-1}

To create a static proof, the website needs to be publicly accessible (not behind a firewall), or your organization's allowlist must include the *`Workfront`* domain. Workfront cannot capture a password-protected website as a static *`proof`*.


>[!TIP] {type="tip"}
>
>We recommend interactive *`proofing`* rather than static *`proofing`* for internal pages requiring authorization and password-protected pages. For more information, see [Interactive content proofs overview](interactive-content-proofs.md).





1. Go to the project, task, or issue where you want to create a new website *`proof`* or a new version of an existing one.
1. Click `Documents``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> &nbsp;in the left panel </MadCap:conditionalText>`.

1.  (Conditional) If you are creating a new *`proof`*, click  `Add New`, then click `Proof` in the menu that appears.
1. (Conditional) If you are creating a new version of an existing *`proof`*: 
    
    
    1. Mouse over the URL *`proof`*&nbsp;for which you want to create a new version, then select it by clicking in the light blue background surrounding it.
    
    
       ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)  

    
    1. Click `Add new` > `Version` > `Proof`.  

    
    

1.  Type the URL of the website you want to proof in the `Add Files` area, then press `Enter`.


   The URL appears below the box where you typed it.


   ![](assets/url-name-appears-below-350x142.png)



1.  Click the URL you have added.


   Options for configuring the website *`proof`* appear.


   ![](assets/interactive-proof-radio-btn-area-350x199.png)



1.  (Optional) If you want to change the name of the *`proof`* from the website URL to something else, type a  `Proof name.`
1.  Make sure  `Capture screenshot`&nbsp;is selected and use any of the following options:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Screenshot resolution</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Adjust the resolution of your content when reviewers view the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, allowing them to see how it appears on devices of varying sizes, such as phones, tablets, and monitors.</p> <p>If you select multiple resolutions, a separate <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is created for each resolution you select.</p> <p>Note: When a reviewer comments on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, the comment includes the resolution showing when the comment was made so that other reviewers know which resolution is associated with the comment.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Look for subpages</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Capture the website's subpages as well as its main pages. You can click&nbsp;Select all&nbsp;to include all the pages, or you can click only certain pages you want to be included. The plus and minus buttons let you expand and close the subpage areas in the website.</p> </td> 
  </tr> 
 </tbody> 
</table>



   >[!IMPORTANT] {type="important"}
   >
   >You cannot change the Capture screenshot setting for any subsequent versions of the *`proof`* that you create.



1.  Click `Done`.


   If you selected multiple screenshot resolutions in step 8, the list includes a set of screenshots for each resolution. You can generate these screenshots as separate *`proofs`* or combine them into a single *`proof`* (see  [Single proof](configure-proof.md#single-proof) in [Configure a proof](configure-proof.md).). We recommend that you combine them, especially if you are creating a static website *`proof`*.


   >[!NOTE]
   >
   >If you are adding a new version to an existing URL *`proof`*, any options that were configured on the original *`proof`* or previous version are maintained in this version.



1. Click `Create proof` to create a simple proof with no review process.  
   or  
   Continue by configuring an advanced *`proof`*: 
    
    
    * [Create an advanced proof with a Basic workflow](configure-basic-proof-workflow.md)
    * [Create an advanced proof with an Automated workflow](create-automated-proof-workflow.md)
    
    



