---
filename: wf-adobe-xd-proofs
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
---



# Upload XD art boards as proofs to *`Workfront`* {#upload-xd-art-boards-as-proofs-to-workfront}

You can upload your art boards as proofs directly to *`Adobe Workfront`* for a thorough review and approval.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium</p> <p>For more information about proofing access with the different plans, see <a href="access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Current plan: <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or <span class="mc-variable WFVariables.Proof-UC-n variable varname">Proof</span></p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">You must have an Adobe Creative Cloud license in addition to a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.proofPermissionProfile variable varname">Proof Permission Profile</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Manager or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Prerequisites {#prerequisites}




*  You must install the *`Workfront`* for Adobe XD plugin before you can upload *`proofs`* in Adobe XD.


  For instructions, see [Install Workfront for Adobe XD](wf-adobe-xd-install.md).





## Upload a static *`Proof`* {#upload-a-static-proof}




1.  Click the `Menu` icon in the top-right corner, then select `Work List`. You can also use the menu to navigate to parent objects.  



   ![](assets/menu-350x627.png)   


1. Go to the work item where you want to upload a static proof.
1. Click the `Document` icon ![](assets/documents.png) in the navigation bar. 

1. Click `New File` near the bottom of the plugin.
1.  Select the art boards you wish to upload.


   >[!TIP] {type="tip"}
   >
   >To select more than one art board, click and drag the mouse over the art boards you want.



1. Choose the `Asset Type` from the drop-down menu.  

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 136px;">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td colspan="2" class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" role="rowheader">Export Format</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" style="font-weight: normal;" role="rowheader">.png</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The art board upoads as a .png to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>Work. </td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" style="font-weight: normal;" role="rowheader">.jpg</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The art board uploads as a .jpg to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. <br></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" style="font-weight: normal;" role="rowheader">.svg</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The art board uploads as a .svg to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. </td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" style="font-weight: normal;" role="rowheader">.pdf</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">The art board uploads as a .pdf to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</td>
  </tr>
 </tbody>
</table>


1. In the **Proof Approvals** section, click `Add Approvers`, then type the names of the users you want to tag for approval from the `Approvers` drop-down menu that appears.  
   Or  
   Click `Select Proof workflow`, then select the workflow from the `Workflow Template` drop-down menu that appears.

1.  (Optional) Type a comment in the `Updates` area.


   ![](assets/proof-approvals-xd-350x847.png)



1.  Click `Upload`.  
   The document appears in the Documents area in the plugin and the desktop app.




## Upload an interactive proof {#upload-an-interactive-proof}

You can create an interactive proof for your art boards with the *`Workfront`* for Adobe plugin. It is a 2-step process. First you need to create an interactive link, then you need to upload the proof to a work item.


### Create an interactive link for your art board  {#create-an-interactive-link-for-your-art-board}




1. Open your art board, then click `Share` in the top-left area of the screen.
1.  Specify the link settings:

    
    
    1.  Name the link.
    1.  Choose a view setting.
    1.  In the `Link Access` section, ensure `Anyone with this link` is selected.
    
    
       You must enable this type of access in order to generate an interactive proof. 
    
    1.  Click `Create Link`.
    
    

1.  Click back to `Design` in the top-left area of the screen. Continue to the [Upload an interactive proof](#upload) section below. 


   >[!NOTE]
   >
   >You may need to reopen the plugin panel in the bottom-left corner of the screen.







### Upload an interactive proof {#upload-an-interactive-proof-1}




1.  Click the `Menu` icon in the top-right corner, then select `Work List`. You can also use the menu to navigate to parent objects.  



   ![](assets/menu-350x627.png)   


1. Go to the work item where you want to upload an interactive proof.
1. Click the `Document` icon ![](assets/documents.png) in the navigation bar. 

1. Click `New File` near the bottom of the plugin.
1.  In the `Asset Type`drop-down menu, choose the link you just created under the `Shared links`.  
   ![](assets/shared-links-xd-350x870.png)


1. In the `Proof Approvals` section, click `Add Approvers`, then select the users you want to tag for approval from the `Approvers` drop-down menu that appears.  
   Or  
   Click `Select Proof workflow`, then select the workflow from the `Workflow Template` drop-down menu that appears.

1. (Optional) Type a comment in the `Updates` area.
1.  Click `Upload`.


   The document appears in the Documents area in the plugin and the desktop app.


   >[!IMPORTANT] {type="important"}
   >
   >Users must have access to the *`Desktop Proofing Viewer`* to review and approve interactive proofs. For more information, see [Install the Desktop Proofing Viewer](installing-desktop-proofing-viewer.md).







## Upload a new proof version {#upload-a-new-proof-version}

You can upload a new version of a proof. The plugin remembers the proofing workflow set on the previous version, but you can change this if you wish. 



1.  Click the `Menu` icon in the top-right corner, then select `Work List`. You can also use the menu to navigate to parent objects.  



   ![](assets/menu-350x627.png)   


1. Go to the work item you need to upload a document to.
1. Click the `Document` icon ![](assets/documents.png)in the navigation bar. 

1. Click `New Version` near the bottom of the plugin.
1.  Select the art boards you wish to upload.


   >[!NOTE]
   >
   >If you want to upload a new version of an .svg, .png, or .jpg, you can upload only one art board.



1. Choose the `Asset Type` from the drop-down menu.  


1. In the `Proof Approvals` section, click `Add Approvers`, then select the users you want to tag for approval from the `Approvers` drop-down menu that appears.  
   Or  
   Click `Select Proof workflow`, then select the workflow from the `Workflow Template` drop-down menu that appears.

1.  (Optional) Type a comment in the `Updates` area.


   ![](assets/proof-approvals-xd-350x847.png)



1. Click `Upload`.  
   The document appears in the Documents area in the plugin and the desktop app.



