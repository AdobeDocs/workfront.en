---
filename: remove-template-from-project
product-area: templates
navigation-topic: templates-navigation-topic
---



# Remove template information from a project {#remove-template-information-from-a-project}

You cannot remove a template from a project. You can only manually remove information that was added to the project after a template was attached to the project. For information about attaching templates, see [Attach a template to a project](attach-template-to-project.md). 


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Options to remove template information from a project {#options-to-remove-template-information-from-a-project}

To remove template information that was added to the project, you can do one of the following: 



*  Manually remove information from the project after the template was attached.


  For information, see [Edit projects](edit-projects.md). 






*  Delete the tasks in the project which were added with the template.


  For information, see the [Delete tasks created from a template](#delete) section in this article.

*   Delete the template from  *`Workfront`*. Deleting the template from *`Workfront`* does not delete the tasks added from the template from projects. 


  For information, see [Delete project templates](delete-templates.md). 





## Delete tasks created from a template {#delete-tasks-created-from-a-template}




1.  Go to the `Tasks` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section </MadCap:conditionalText>`of the project.
1.  Do one of the following:

    
    
    *  Create a filter for the task list to display only tasks that were created from a template using the following statement: 
    
    
    
    
      ```    
      Task >> Template Task ID >>Is Not Blank
      ```    
    

    
    
      For information about creating a filter, see [Create or edit filters in Adobe Workfront](create-filters.md). 
    
    
      When you apply the filter, only tasks associated with a Template Task ID display in the list. 
    
    *  Create a view for the task list to display the `Template Task ID` or `Template Task Name` fields in a column. 
    
    
      When you apply the view, the tasks that contain information in the Template Task ID or Template Task name column were created using a template. 
    
    
      For information about creating a view, see [Views overview in Adobe Workfront](views-overview.md). 
    
    
    

1.  Select all the tasks identified in Step 2 as created from a template, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">the Delete icon <img src="assets/delete.png"></span></MadCap:conditionalText>` `> Yes, Delete it`. For more information, see [Delete tasks](delete-tasks.md). 


