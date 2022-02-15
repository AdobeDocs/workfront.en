---
filename: setup-asset-essentials
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
---



# Configure the *`Experience Manager Assets Essentials`* integration {#configure-the-experience-manager-assets-essentials-integration}

Connect your work with your content in *`Experience Manager Assets Essentials`*​:



*  Push assets and metadata from *`Adobe Workfront`* to *`Experience Manager Assets Essentials`*​
*  Link assets from *`Experience Manager Assets Essentials`* to your projects and tasks in *`Workfront`*​
*  Facilitate versioning workflows for assets pushed to *`Experience Manager Assets Essentials`*




## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> licenses*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">You must have <span class="mc-variable WFVariables.AEMAssetEssentials variable varname">Experience Manager Assets Essentials</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For information on <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Set up the integration {#set-up-the-integration}




1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup`.
1.  Select ![](assets/document-icon.png) `Documents`in the left panel, then select `Experience Manager Integration`.
1.  Select `Add Experience Manager Integration`.
1.  Specify the following:

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Enter the name you want users to see in the Add new button in the Documents area.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Navigation&nbsp;URL</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The system automatically populates the Navigation URL. This URL is used to link to your organization's <span class="mc-variable WFVariables.AssetsEssentials variable varname">Assets Essentials</span> instance from the Main Menu for quick access.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">IMS&nbsp;Org</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>The system automatically populates your IMS Org. You can modify this field if desired.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Optional) Set up metadata mapping:


   `Documents with the specified native or custom fields automatically map to the specified fields the first time an asset is sent to` *`Experience Manager Assets Essentials`*:

    
    
    1.  In the `Workfront Source Field` column, choose a built-in or custom *`Workfront`* field.
    1.  In the `Experience Manager Target Field`, choose an *`Experience Manager Assets Essentials`* field. 
    1.  Repeat steps a and b as needed.
    
    
       >[!NOTE]
       >
       >You can map metadata only in one direction: from *`Workfront`* to *`Assets Essentials`*. Metadata for documents linked to *`Workfront`* from *`Assets Essentials`* cannot be transferred to *`Workfront`*.
    
    
    
    
    

1.  Select `Save`.


