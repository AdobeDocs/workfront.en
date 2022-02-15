---
filename: enhanced-connector-send-document
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
---



# Send a Document to Experience Manager Assets {#send-a-document-to-experience-manager-assets}

You can send documents from *`Workfront`* to *`Experience Manager Assets`*. Documents uploaded and sent from *`Workfront`* to Experience Manager Assets still count against your overall document storage. Assets linked from Experience Manager Assets don't count towards overall storage.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.ExperienceManagerAssets variable varname">Experience Manager Assets</span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>View access or higher on Documents</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you begin, you must



* Install the *`Workfront for Experience Manager enhanced connector`*. 




## Send a Document to Experience Manager Assets {#send-a-document-to-experience-manager-assets-1}

When a user sends a document from *`Workfront`* to *`Experience Manager Assets`*, mapped metadata transfers along the document. If configured, the metadata syncs continuously each time a change is made. 


To send a document:



1.  Go to the `Documents` area in *`Workfront`*, and select the document you want to send.
1.  Click `Send to`, then choose the Experience Manager Assets integration your administrator set up.


   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention *`Experience Manager Assets`*.


   ![](assets/copy-of-send-to-in-toolbar-350x149.png)



1.  Choose where you want the asset to go, then click `Select Folder`.
1.  When you find your desired destination, click `Save`. 




## Send a new version to *`Experience Manager Assets`* {#send-a-new-version-to-experience-manager-assets}

You can add a new version to a document you have previously uploaded to *`Workfront`*. For more information, see [Upload a new version of a document](upload-new-document-version.md). After the latest version is uploaded, you can send it to *`Experience Manager Assets`*. If a mapped field in *`Workfront`* has changed, the new version updates the metadata in *`Experience Manager Assets`* when it sends.


To send the most recent version:



1. Go to the `Documents` area in *`Workfront`*, and locate the document.

1.  Click `Send to`, then choose the Experience Manager Assets integration your administrator set up.


   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention *`Experience Manager Assets`*.


   ![](assets/copy-of-send-to-in-toolbar-350x149.png)



1.  Click `Save`. The new version saves in the same location as the previous version. 


