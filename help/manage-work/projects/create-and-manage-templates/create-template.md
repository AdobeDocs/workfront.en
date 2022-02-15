---
filename: create-template
product-area: templates
navigation-topic: templates-navigation-topic
---



# Create a project template {#create-a-project-template}

You can create and delete templates from the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Templates </MadCap:conditionalText>`area. When building a new template, you can enter the information for all of the tasks and all information for your future project settings. This information will then transfer to the project, when you create it from the template. 


You can create a new template in the following ways:



* From scratch, as described in this article.
*  From existing projects, by saving a project as a template.


  For more information about creating templates from existing projects, see [Save a project as a template](save-project-as-template.md).

*  By copying it from another template.


  For more information about copying an existing template, see [Copy a project template](copy-template.md).

*  If you are a *`Workfront administrator`*, you can create templates by importing Blueprints. For information, see [Configure a blueprint](configure-template-package.md). 




## Access requirements {#access-requirements}

You must have the following:

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">System administrator for importing templates from Blueprints</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>You have Manage permissions to the templates you create, by default</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create a template {#create-a-template}




1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> From the  <span class="bold">Main Menu</span>  <img src="assets/main-menu-icon.png"> click  <span class="bold">Templates</span>. </MadCap:conditionalText>`
1.  Click `New Template`.


   The template is untitled.


   ![](assets/create-template-nwe-350x178.png)



1.  Specify a name for the new template in the template header, then press `Enter.`
1.  Click the `Template Tasks` section in the left panel. 
1.  Click `Start Adding Template Tasks`.


   Or


   Click `New Template Task`to start adding tasks to your template.


   Adding template tasks to a template is identical to adding tasks to a project.


   For more information about adding tasks to a project, see [Create tasks in a project](create-tasks-in-project.md).


   >[!NOTE]
   >
   >You cannot add recurring tasks to a template. 



1.  (Optional) Click the `Gantt chart` icon in the upper-right corner of the Task List to see a visual representation of the template's task list. 


   >[!TIP] {type="tip"}
   >
   >You cannot edit tasks directly from this Gantt chart.



1.  To add information to your new template, click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the  <span class="bold">More</span> menu  <img src="assets/more-icon.png">, then click  <span class="bold">Edit</span></MadCap:conditionalText>`.


   For information about editing a template, see [Edit project templates](edit-templates.md).

1. Click `Save Changes`.
1. (Optional) If you want to add additional items to the template, see the section [Add additional items to a template](edit-templates.md#adding-items-to-template) in the article [Edit project templates](edit-templates.md). 





## Template settings determined by group association {#template-settings-determined-by-group-association}

A project template's association with a group (or lack thereof) affects how project, task, and issue preferences determine certain settings in the template. For more information, see the section [Create and modify a group’s project templates](create-and-modify-a-groups-templates.md#template2) in the article [Create and modify a group’s project templates](create-and-modify-a-groups-templates.md).
