---
filename: set-pim
product-area: projects
navigation-topic: financials
---



# Set the Performance Index Method (PIM) {#set-the-performance-index-method-pim}



##  

The Performance Index Method (PIM) for the project controls the method *`Adobe Workfront`* uses to calculate project performance metrics such as Cost `Performance Index` (CPI), Cost Schedule Performance Index (CSI), Schedule Performance Index (SPI), and Estimate At Completion (EAC). 


*`Workfront`* calculates these values using the following:



* Hours
* Cost





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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Considerations about PIM in *`Workfront`*  {#considerations-about-pim-in-workfront}




* Your *`Workfront administrator`* `or a *`group administrator`*`sets up the default for whether the Performance Index Method (PIM) should be hour-based or cost-based. The calculations for the performance metrics change according to how this default is set. For more information about how to change the default for how to calculate the PIM, see [Configure system-wide project preferences](set-project-preferences.md). 

* Project managers can also change the setting for the PIM, at the project level, for individual projects in the Finance subtab of the project. You must have Manage permissions to the project to edit the Finance subtab of the project.




## Set the Performance Index Method (PIM) for a project {#set-the-performance-index-method-pim-for-a-project}




1.  Go to a project which you are the owner of.


   >[!IMPORTANT] {type="important"}
   >
   >You need Manage permissions to the project to perform the following steps. We also recommend that only the Project Owner should make changes to the Finance `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area </MadCap:conditionalText>`of the project. 



1.  Click `Project Details` in the left panel, then go to the `Finance` area.
1.  Double-click the value in the `Performance Index Method` field to edit it.
1.  Select from the following options in the `Performance Index Method` field:


1. Click `Save``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">Changes</span></MadCap:conditionalText>`.



