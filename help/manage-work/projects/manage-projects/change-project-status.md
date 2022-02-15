---
filename: change-project-status
product-area: projects
navigation-topic: manage-projects
---



# Change the status of a project  {#change-the-status-of-a-project}

You can manually change the status of a project.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Considerations about updating to specific statuses {#considerations-about-updating-to-specific-statuses}




* `When updating a project to Complete:`Ensure that all tasks and issues are completed on the project. You cannot select the Complete status for a project, or any other status that equates Complete when there are tasks or issues that have not been completed on the project. This includes approving any task or issue that is in a Complete-Pending Approval status.
* `When updating a project from Complete to Current:`If all the tasks and issues on the project are completed, ensure that the project's Completion Mode is set to Manual. If the project's Completion&nbsp;Mode is Automatic, the status of the project remains Complete. 




## Change project status {#change-project-status}




1. Go to the project whose status you want to update.
1.  In the project header, click the name of the status in the `Status` field, then select a new status.


   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)




   Or  



   Click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the  <span class="bold">More</span> menu  <img src="assets/qs-more-menu.png"> next to the name of the project and click  <span class="bold">Edit</span></MadCap:conditionalText>` and select a new status in the `Status` field, then click `Save`.


   The project status updates to the status you selected.   




