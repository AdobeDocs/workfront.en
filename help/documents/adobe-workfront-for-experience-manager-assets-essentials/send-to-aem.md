---
filename: send-to-aem
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
---



# Send a Document to *`Experience Manager Assets Essentials`* {#send-a-document-to-experience-manager-assets-essentials}

You can send documents from *`Workfront`* to *`Experience Manager Assets Essentials`*. Documents uploaded and sent from *`Workfront`* to *`Assets Essentials`* still count against your overall document storage. Assets linked from *`Assets Essentials`* don't count towards overall storage.


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><a href="wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">You must have <span class="mc-variable WFVariables.AEMAssetEssentials variable varname">Experience Manager Assets Essentials</span>.</td> 
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


## Send a Document from *`Workfront`* {#send-a-document-from-workfront}

When a user sends a document from *`Workfront`* to *`Assets Essentials`*, mapped metadata transfers along the document. After the document is sent, changes made to the document's metadata in *`Workfront`* are not reflected in *`Assets Essentials`*. If a mapped field in *`Workfront`* is changed, you must send a new version of the document with the updated metadata to *`Assets Essentials`*. To set up or edit metadata, see [Configure the Experience Manager Assets Essentials integration](setup-asset-essentials.md).


To send a document:



1.  Go to the `Documents` area in *`Workfront`*, and select the document you want to send.
1.  Click `Send to`, then choose the *`Assets Essentials`* integration your administrator set up.


   >[!NOTE]
   >
   >The *`Workfront administrator`* can choose any name for this integration, so it may not specifically mention *`Assets Essentials`*.


   ![](assets/copy-of-send-to-in-toolbar-350x149.png)



1.  Choose where you want the asset to go, then click `Select Folder`.
1.  When you find your desired destination, click `Save`. 




## Send a new version {#send-a-new-version}

You can add a new version to a document you have previously uploaded to *`Workfront`*. For more information, see [Upload a new version of a document](upload-new-document-version.md). After the latest version is uploaded, you can send it to *`Assets Essentials`*. If a mapped field in *`Workfront`* has changed, the new version updates the metadata in *`Assets Essentials`* when it sends.


>[!IMPORTANT] {type="important"}
>
>Before you upload a new version to Workfront, we recommend renaming the file. If you upload a new version with the exact same file name as a previous version, only the most recent version can be downloaded from Workfront. All versions can be downloaded from AEM Assets Essentials regardless of the file name.


To send the most recent version:



1. Go to the `Documents` area in *`Workfront`*, and locate the document.

1.  Select `Send to`, then choose the *`Assets Essentials`* integration your administrator set up.


   >[!NOTE]
   >
   >The *`Workfront administrator`* can choose any name for this integration, so it might not specifically mention *`Assets Essentials`*.


   ![](assets/copy-of-send-to-in-toolbar-350x149.png)



1.  Click `Save`. The new version saves in the same location as the previous version. 


