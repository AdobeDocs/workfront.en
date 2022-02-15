---
filename: wf-adobe-xd-docs
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
---



# Upload XD art boards as documents to *`Workfront`* {#upload-xd-art-boards-as-documents-to-workfront}

You can upload your art boards as documents for a quick review and approval or simply to store in *`Adobe Workfront`*.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">You must have an Adobe Creative Cloud license in addition to a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>View access or higher to the object where you want to upload a document.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}




*  You must install the *`Workfront`* for Adobe XD plugin before you can upload XD art boards as documents to *`Workfront`*.


  For instructions, see [Install Workfront for Adobe XD](wf-adobe-xd-install.md).





## Add a new document {#add-a-new-document}




1.  Click the `Menu` icon in the top-right corner, then select `Work List`. You can also use the menu to navigate to parent objects.  



   ![](assets/menu-350x627.png)   


1. Go to the work item where you want to upload a document. 
1. Click the `Document` icon ![](assets/documents.png) in the navigation bar. 

1. Click `New File` near the bottom of the plugin.
1.  Select the art board you wish to upload.


   >[!TIP] {type="tip"}
   >
   >To select more than one art board, click and drag the mouse over the art boards you want.



1. Choose the `Asset Type` from the drop-down menu:  

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" style="font-weight: bold;" colspan="2" role="rowheader">Export Format</td>
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



   >[!NOTE]
   >
   >If you add an approver, the art board uploads to *`Workfront`* as a *`Proof`*.



1. (Optional) Type a comment in the `Updates` area. 
1. Click `Upload`.  
   The document appears in the Documents area in the plugin and the desktop app.





## Add a new version {#add-a-new-version}




1.  Click the `Menu` icon in the top-right corner, then select `Work List`. You can also use the menu to navigate to parent objects.  



   ![](assets/menu-350x627.png)   


1. Go to the work item where you want to upload a document. 
1. Click the `Document` icon ![](assets/documents.png)in the navigation bar. 

1. Click on the document you want to add a new version to.
1. Click `New version` near the bottom of the plugin.
1.  Select the art board you wish to upload.


   >[!NOTE]
   >
   >If you want to upload a new version of an svg, png, or jpg, you can upload only one art board.



1. Choose the `Asset Type` from the drop-down menu:  

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" style="font-weight: bold;" colspan="2" role="rowheader">Export Format</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" style="font-weight: normal;" role="rowheader">png</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The art board upoads as a png to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>Work. </td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" style="font-weight: normal;" role="rowheader">jpg</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The art board uploads as a jpg to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. <br></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" style="font-weight: normal;" role="rowheader">svg</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The art board uploads as a svg to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. </td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" style="font-weight: normal;" role="rowheader">pdf</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">The art board uploads as a pdf to the work item's Documents tab in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</td>
  </tr>
 </tbody>
</table>



   >[!NOTE]
   >
   >If you add an approver, the art board uploads to *`Workfront`* as a *`Proof`*.



1. (Optional) Type a comment in the `Updates` area. 
1. Click `Upload`.  
   The document appears in the Documents area in the plugin and the desktop app.



