---
filename: generate-proof-for-a-document
product-area: documents
navigation-topic: create-proofs-within-workfront
---



# Create a *`proof`* for a document {#create-a-proof-for-a-document}

You can generate a *`proof`* for a document at the time you are uploading it to *`Workfront`*.


You can also generate a *`proof`* for a document already uploaded in *`Adobe Workfront`* or for a new version of a *`proof`* already in *`Workfront`*.


If a *`proof`* fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](troubleshooting-proof-creation-failures.md).


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


## Upload a document and create a *`proof`* {#upload-a-document-and-create-a-proof}




1. Go to the project, task, or issue where you want to create a new *`proof`*.
1. Click the `Documents`&nbsp;tab.
1. Click Documents ![](assets/document-icon.png) in the left panel.
1.  Click  `Add New`, then click `Proof` in the menu that appears.


   >[!TIP] {type="tip"}
   >
   >You can enable the `Automatically generate proofs when uploading documents` setting in your user profile to automate this process. For more information, see [Configure My Settings](configure-my-settings.md) .



1. In the `New proof` page that appears, continue with [Add files](configure-proof.md#add-files) in [Configure a proof](configure-proof.md).





## Upload a document and create a new version of a *`proof`* {#upload-a-document-and-create-a-new-version-of-a-proof}




1. Go to the project, task, or issue where you want to create a new version of an existing *`proof`*.
1.  Click the `Documents`&nbsp;tab.
1.   Select the document where you want to add a new version. 
1.  Click `Add New` > `Version` > `Proof`.
1.  In the `New Proof Version` page that appears, you can 

    
    
    *  [Create an advanced proof with a Basic workflow](configure-basic-proof-workflow.md) 
    *  [Create an advanced proof with an Automated workflow](create-automated-proof-workflow.md) 
    
    





## Use drag-and-drop to generate a simple *`proof`* for a new version {#use-drag-and-drop-to-generate-a-simple-proof-for-a-new-version}

You can drag-and-drop a document from your file system (such as your desktop) to create a new *`proof`* or a new version of an existing *`proof`*. The *`proof`* contains the following settings, depending on whether you are creating a new *`proof`* or a new version:



* `New *`proof`*:` Creates a simple *`proof`* that is shared only with you. You can modify share settings after the *`proof`* is created as described in [Edit proof settings](edit-proof-settings.md).

* `New version of existing *`proof`*:` Creates a new version with the same *`proof`* settings as the previous version.



To use drag-and-drop to generate a new *`proof`* or new *`proof`* version:



1. Ensure that proofs are configured to be automatically generated, as described in [Configure a user's proofing access](configure-a-users-proofing-access.md#configuring-proofs-to-automatically-generate) in [Configure a user's proofing access](configure-a-users-proofing-access.md).

1. Continue with&nbsp; [Add documents to Adobe Workfront from your file system](add-documents-from-file-system.md), which explains the drag-and-drop method of adding documents.&nbsp;




## Create a proof for an existing document  {#create-a-proof-for-an-existing-document}




1.  Go to the project, task, or issue where you want the *`proof`*, then click the `Documents` section.
1.  Hover over the document, then click the `Create Proof` link that appears below the document name. 


   >[!NOTE]
   >
   >If you have `Automatically generate proofs when uploading documents` enabled in your user profile, the system automatically creates a simple proof.



1. Choose one of the following:  
1.  

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 130px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Simple Proof</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This option creates a proof with no workflow attached and applies the default proof settings. You can update the default <span class="mc-variable WFVariables.proof-v variable varname">proof</span>settings or add a workflow after you've created the <span class="mc-variable WFVariables.proof-v variable varname">proof</span>. For more information on proof settings, see <a href="edit-proof-settings.md" class="MCXref xref">Edit proof settings</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Advanced Proof</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>This option allows you to configure a Basic or Advanced workflow and modify proof settings for the proof you create. For more information, see </p> 
    <ul> 
     <li> <p><a href="configure-basic-proof-workflow.md" class="MCXref xref">Create an advanced proof with a Basic workflow</a> </p> </li> 
     <li> <p><a href="create-automated-proof-workflow.md" class="MCXref xref">Create an advanced proof with an Automated workflow</a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



