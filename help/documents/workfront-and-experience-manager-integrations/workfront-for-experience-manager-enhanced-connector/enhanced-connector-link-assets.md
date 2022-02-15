


# Link assets and folders from *`Experience Manager Assets`* {#link-assets-and-folders-from-experience-manager-assets}

You can link an asset or folder from *`Experience Manager Assets`* to any Workfront object that supports documents. Assets sent from *`Experience Manager Assets`* don't count towards your overall document storage in *`Workfront`*. Documents uploaded and sent from *`Workfront`* to *`Experience Manager Assets`* do count towards overall storage.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>View access or higher on a Document</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you begin, you must



* Install the *`Workfront for Experience Manager enhanced connector`*




## Link an asset from *`Experience Manager Assets`* {#link-an-asset-from-experience-manager-assets}

You can link an asset from *`Experience Manager Assets`* to *`Workfront`*. Once the asset is linked you can



*  [Proof a linked asset for Experience Manager Assets](enhanced-connector-proof-asset.md) 
*  [Upload a new version of a document](upload-new-document-version.md) 


To link an asset to *`Experience Manager Assets`*:



1. Go to the `Documents` area in *`Workfront`* where you want to add the document.

1.  Click `Add new`, then choose the Experience Manager Assets integration your administrator set up.
1.  

   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention *`Experience Manager Assets`*.


1.  Select the assets you want.


   ![](assets/select-an-asset.png)



1.  Click `Link`.




## Link a folder from *`Experience Manager Assets`* {#link-a-folder-from-experience-manager-assets}

Permissions to view individual assets inside of a folder rely on *`Experience Manager Assets`* permissions. 


To link a folder to *`Experience Manager Assets`*:



1. Go to the `Documents` area in *`Workfront`* where you want to add the document.

1.  Click `Add new`, then choose the Experience Manager Assets integration your administrator set up.
1.  

   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention *`Experience Manager Assets`*.


1.  Select the folders you want.


   ![](assets/select-a-folder.png)



1.  Click `Link`.




## Link a new version from *`Experience Manager Assets`* {#link-a-new-version-from-experience-manager-assets}

You can pull a new asset over from *`Experience Manager Assets`* and add it to an existing asset as a new version in *`Workfront`*. If the document is already linked and a new version is added in *`Experience Manager Assets`*, the new version appears automatically in *`Workfront`*.


>[!TIP] {type="tip"}
>
>You can view all versions of an asset if you go to `Document Details` > `Versions`. 


To link a new version from *`Experience Manager Assets`*:



1. Go to the `Documents` area in *`Workfront`* where you want to add the document.

1.  Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder. 
1.  Click `Add new`, then choose the Experience Manager Assets integration your administrator set up.


   >[!NOTE]
   >
   >Any name may be chosen for this integration, so it may not specifically mention *`Experience Manager Assets`*.



1.  Select the asset you want.


   ![](assets/select-an-asset.png)



1.  Click `Link`. 


