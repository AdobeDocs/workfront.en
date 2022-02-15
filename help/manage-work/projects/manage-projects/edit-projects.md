---
filename: edit-projects
product-area: projects
navigation-topic: manage-projects
---



# Edit projects {#edit-projects}

You can edit a project in *`Adobe Workfront`* as often as needed. We recommend that you edit projects minimally after they become Current, to avoid confusion by sending out notifications about the changes to the entire project team. You should ideally edit a project when the project is in Planning status. For information about the Project Team, see [Project Team overview](project-team-overview.md). 



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information about access to projects, see <a href="grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit it in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit it in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Limitations for editing projects {#limitations-for-editing-projects}

There are some limitations that might prevent you from editing projects. 


Consider the following when editing projects: 



* You cannot edit projects that are in an Approval Process, except for logging time. 
* You can attach documents or templates to a project that has a status of Complete, Dead, or is in Pending Approval only if your *`Workfront administrator`* or a *`group administrator`* enabled this functionality in the Project Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](set-project-preferences.md). 

* You can only edit the following information on a project in a Dead or Complete status:
    
    
    * Modify existing expenses.
    * Add, remove, or edit custom forms.
    
    





## Edit a project  {#edit-a-project}

Editing a project allows you to modify information and settings for the project, as well as tasks and issues on the project. 


Some settings mentioned in this article might be modified from their default status for the template from which the project was created. For information about editing templates, see [Edit project templates](edit-templates.md). 



1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Projects`. 
1.  (Optional) Click `Projects I'm On` or `Projects I Ow`n to display projects where you are the owner or projects where you are part of the project team. 


   ![](assets/projects-i'm-on-i-own-buttons-350x302.png)



1.  Click the project you want to edit to access it. 


   >[!NOTE]
   >
   >If you are a *`group administrator`*, you can see and edit your group’s projects in the Groups area as well as in the Projects area. For more information, see [Create and modify a group’s projects](create-and-modify-a-groups-projects.md).   




1.  
   (Optional) To edit limited information about a project, click `Project Details` in the left panel. 


   ![](assets/nwe-project-details-expanded-350x298.png)




   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* or *`Group administrator`* modified your Layout Template, the fields in the Project&nbsp;Details area might be rearranged or not display. For information, see [Customize the Details view using a layout template](customize-details-view-layout-template.md). 


   To edit information in the Details section, do the following: 

    
    
    1.  (Optional) Click the `Collapse All` icon in the upper-right corner to collapse all areas. 
    1.  (Optional and conditional) When an area is collapsed, click the `right-pointing arrow` ![](assets/right-pointing-arrow.png) next to each area to expand the area you want to edit. 
    1.  `<MadCap:snippetBlock src="assets/edit-fields-in-details-section-all-objects-step.flsnp" />` For more information about editing information in the Project Details tab, see the following articles:
    
        
        
        *  [Manage information in the project Overview area](understand-project-overview-area.md) 
        *  [Manage information in the project Finance area](manage-project-finance-area.md) 
        
        
    
    1.  (Optional) To attach a custom form, start typing the name of a form in the `Add custom form` field, then select it when it displays in the list, then click `Save Changes`.
    1.  (Optional) Click the `Export` icon ![](assets/export.png) to export the Overview and custom forms information to a PDF file, then click `Export`. Select from the following:
    
        
        
        *  Select all (displays only when there is at least one custom form attached)
        *  Overview
        *  The name of one or multiple custom forms
        
        
       The PDF file downloads to your computer. 
    
    
       ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)    
    

    
    
       For more information, see [Export custom forms and object details in Adobe Workfront](export-custom-forms-details.md).
    
    
    
   For information about the fields visible in the Project Details section, continue with editing the project in the Edit Project box as described below.
1.   To edit all information about the project, click the `More` menu ![](assets/qs-more-menu.png) next to the name of the project, then click `Edit`. 


   Or


   From a list of projects, select a project, then click the `Edit` icon ![](assets/edit-icon.png) at the top of the list. 


   The `Edit Project` box opens. 


   >[!IMPORTANT] {type="important"}
   >
   >You must have Manage permissions to the project in order to see the Edit option.


   All project fields are available in the Edit Project box and are grouped by the areas listed in the left panel. 


   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* or *`Group administrator`* modified your Layout Template, the areas in the left panel of the Edit Project box or any fields listed in these areas might be rearranged or not display. For information, see [Customize the Details view using a layout template](customize-details-view-layout-template.md).



1.   (Conditional) If you clicked the `More` menu and then `Edit`, consider specifying information in any of the following areas listed in the left panel:

    
    
    * [Project Name](#project) 
    * [Overview](#overview) 
    * [Custom Forms](#custom) 
    * [Finance](#finance) 
    * [Project Settings](#project2) 
    * [Task Settings](#task) 
    * [Issue Settings](#issue) 
    *  [Access](#access2)
    
    


   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* sets up our Layout Template, the fields in the Edit Project box might be different in your environment. For information, see [Customize the Details view using a layout template](customize-details-view-layout-template.md).







### Project Name {#project-name}




1. Begin editing your project as described above.
1.  Click `Project Name` in the left panel. 


   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)



1. Update the name of the project. 




### Overview {#overview}




1. Begin editing your project as described above.
1.  Click `Overview` in the left panel. 


   ![](assets/nwe-overview-in-edit-project-box-350x172.png)



1. Update the following information about the project: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Description</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Add additional information about the project.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" colspan="2" role="rowheader">Basic information section</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Status</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Select the status of the project. You cannot mark a project Complete before all tasks and issues complete. For information about project statuses, see <a href="project-statuses.md" class="MCXref xref">Access the list of system project statuses</a></p><p>Tip: You can update the Status in the project header. </p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Priority</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p><p>This is just a visual flag for you which allows you to prioritize your projects.</p><p>Depending on the Project Preferences selected by your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>, the names of priorities might be different for you. For more information about editing priorities, see <a href="create-customize-priorities .md" class="MCXref xref">Create and customize priorities</a></p></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">URL</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Specify a web link that relates to information about this project.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" colspan="2" role="rowheader">Project condition section</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Condition Type</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Select between the following Condition Types:
     <ul>
      <li><span class="bold">Manual: </span>The project owner sets the condition on the project manually.</li>
      <li><span class="bold">Progress Status: </span><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> automatically sets the condition based on the Progress Status of tasks on the Critical Path. For more information about understanding Progress Status, see <a href="task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</li>
     </ul><p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span><span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span></span> selects the default for how the projects' condition is calculated for your system <span>or your group</span>. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Condition</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p><p>(Appears only after you select <span class="bold">Manual</span> for the <span class="bold">Condition Type</span>): Select a Condition to indicate how the project is going. </p><p>Tip: If the Condition Type is set to Manual, you can also update the Condition in the project header.</p><p>For information how project Conditions can be set automatically or manually, see <a href="project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a></p></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" colspan="2" role="rowheader">Project dates section</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Schedule Mode</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>Specify whether the project is scheduled from the Start Date, or from the Completion Date. This selection determines the planned dates of the tasks on the project.
     <ul>
      <li><span class="bold">Start Date</span>: The first task of the project has the same Planned Start Date as the project by default. For information about the task Planned Start Date, see <a href="task-planned-start-date.md" class="MCXref xref">Overview of the task Planned Start Date</a>. The project timeline calculates from the Start Date and the Completion Date of the project is calculated by the system, based on the duration of all the tasks. </li>
      <li><span class="bold">Completion Date</span>: The last task of the project has the same Planned Completion Date as the project. The project timeline calculates from the Completion Date and the Start Date of the project is calculated by the system, by subtracting the duration of all the tasks from the Completion Date of the project. </li>
     </ul><p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span><span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span></span> selects the default Schedule Mode setting for your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Planned Start Date and time</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p><p>Specify the date when you select <span class="bold">Schedule From Start Date</span>. <br></p><p>This is a read-only field when you select <span class="bold">Schedule from Completion Date</span>.<br></p></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Planned Completion Date and time</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>Specify the date when you select <span class="bold">Schedule from Completion Date</span>. </p><p>This is a read-only field when you select <span class="bold">Schedule from Start Date</span>.<br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" colspan="2" role="rowheader">Project association section</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Portfolio</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Indicate a Portfolio that the project belongs to. You must create a Portfolio first, before it appears in the drop-down list. Only active portfolios can be associated with a project. For more information about creating portfolios, see <a href="create-portfolios.md" class="MCXref xref">Create a portfolio</a>.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Program</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>If you selected a Portfolio for the project, specify a Program for the project. Some Portfolios might not have Programs. You must create a Program first, before it appears in this drop-down list. Only active programs can be associated with a project. </p><p>For more information about creating programs, see <a href="create-program.md" class="MCXref xref">Create a program</a>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p><p>Specify the name of the group associated with the project. </p>This is a required field. You cannot have a project which is not associated with a group. </p><p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
       Depending on the details configured for the group, you might also see its Business Leader and description.
     </MadCap:conditionalText></p><p><img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"></p><p>Note: <p>By default, one of the following groups is automatically associated <span data-mc-edit-date="2020-12-02T17:06:08.1586452-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted, only in QS" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2020-12-02T17:06:00.8315301-05:00">with</span> a project when it is created, unless you specify a different group:</p>
     <ul>
      <li><p><span>When the project is created from the Projects area, the Home Group of the project creator is associated with the project.</span></p><p>This is also true when the project is created from the Projects <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
         section
        </MadCap:conditionalText> in a portfolio or program.</p></li>
      <li><p>When the project is created from a group’s main page in the Setup area, that group is associated with the project.</p></li>
     </ul></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Company</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Specify a company associated with the project. You must create a company before you can associate it with a project. Only active companies can be associated with a project. For information about creating companies, see <a href="create-and-edit-companies.md" class="MCXref xref">Create and edit companies</a>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" colspan="2" role="rowheader">Project stakeholders section</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Project Owner</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>The user specified in this field is added to the project team and is automatically given manage permissions to the project. The user who is designated as the Project Owner must be a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> active user.</p><p>Tip: You can update the Project Owner in the project header. <br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Project Sponsor</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>The specified user is added to the project team and is automatically given view permissions to the project. The user who is designated as the Project Sponsor must be a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> active user.<br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Resource Manager</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><p>The specified user is automatically given Manage permissions to the project and can assign resources to the tasks and issues on the project. The user maintains Manage permissions on the project even when they are removed from the Resource Manager field. You can specify more than one Resource Manager.<br></p></td>
  </tr>
 </tbody>
</table>

1.  (Optional) Continue editing the following sections, depending on the information you want to modify.


   Or


   Click `Save`.






### Custom Forms {#custom-forms}




1. Begin editing your project as described above.
1.  Click `Custom Forms` in the left panel. 


   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)



1.  Click the `Add custom form` box and select a form from the list to attach it to the project.


   You must build the custom forms before they are available to select in this field. Only active custom forms appear in the list. For more information about building custom forms, see [Create or edit a custom form](create-or-edit-a-custom-form.md). You can add up to ten custom forms to a project. 

1.  (Conditional) If you attached a custom form to the project, edit any fields on the form. You must specify all required fields before you can save the project. 


   >[!NOTE]
   >
   >Depending on how your *`Workfront`* administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the project itself. For information about setting permissions on sections of a custom form, see [Create or edit a custom form](create-or-edit-a-custom-form.md). For information about setting permissions on projects, see [Share a project in Adobe Workfront](share-a-project.md).  




1.  (Optional) Click the `X icon` to the right of the name of a custom form to remove it, then click `Remove`. 
1.  (Optional) Continue editing the following sections, depending on the information you want to modify


   Or


   Click `Save`.





### Finance {#finance}




1. Begin editing your project as described above.
1.  Click `Finance` in the left panel. 


   ![](assets/nwe-finance-in-edit-project-box-350x183.png)



1.  Update the following financial information for the project:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" colspan="2" role="rowheader">Budget section</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Project Currency</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>Specify the currency for the project, if it is different than the default currency of your system. You cannot change the currency of a project if there is already financial information on the project. This field is not visible if you have only the default currency in the system. </p> <p>For more information about currency, see <a href="set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.<br></p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Budget</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify a Budget for the project.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" colspan="2" role="rowheader">Performance metrics section</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Performance Index Method</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify whether the Earned Value metrics of the project are calculated using hours or costs. </p> <p>For more information about the Performance Index Method, see <a href="set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p> <p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span><span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span></span> selects the default Performance Index Method setting for your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Estimate at Completion</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>Specify how Estimate at Completion (EAC) calculates. </p> <p>For more information about how the Estimate at Completion calculates, see <a href="calculate-eac.md" class="MCXref xref">Calculate Estimate At Completion (EAC)</a>.</p> <p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span><span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span></span> selects the default Estimate at Completion setting for your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" colspan="2" role="rowheader">Benefit section</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Planned Benefit</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Estimate what the Planned Benefit of the project is. This is used in the Business Case of the project and the Portfolio Optimizer. For more information about the Planned Benefit of a project, see <a href="project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>. The Planned Benefit of a project is taken into account when the Net Value of a project is calculated. </p> <p>For more information, see <a href="_manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Manage projects in the Portfolio Optimizer</a> .<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Actual Benefit</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Estimate the Actual Benefit of the project. This is a currency amount that represents the benefit that your company or department would gain after this project is complete. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" colspan="2" role="rowheader">Revenue section</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Fixed Revenue</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify the Fixed Revenue for the project.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" colspan="2" role="rowheader">Cost section</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Fixed Cost</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Specify the Fixed Cost for the project. This is different than the Labor Cost which comes from the hours on the project and the Expense Cost which comes from the amount of expenses on the project. The Fixed Cost of a project is taken into account when calculating the Net Value of a project and it is part of the Budgeted Cost.<br></p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Optional) Continue editing the following sections, depending on the information you want to modify.


   Or


   Click `Save`.





### Project Settings {#project-settings}




1. Begin editing your project as described above.
1.  Click `Settings` in the left panel. 


   ![](assets/nwe-project-settings-in-edit-project-box-350x320.png)



1.  Update the following information:



<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Milestone Path</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select a Milestone Path for the project. Only active milestone paths display in the list.</p> <p>For more information about Milestone Paths, see <a href="create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Completion Mode</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Controls how the project is marked as Complete. Select from the following options:
     <ul>
      <li><p><span class="bold">Automatic</span>: The project is marked Complete when all the tasks and issues are completed.</p><p>Note: The project Status is automatically changed to Complete only when the project status is Current when the tasks are completed. </p></li>
      <li><span class="bold">Manual</span>: You have to manually select the Complete status for the project, when all the tasks and issues are completed.</li>
     </ul></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Summary Completion Mode </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Controls how the parent tasks are marked as Complete. Select from the following options:
     <ul>
      <li><span class="bold">Automatic</span>: The parent tasks are marked Complete and they update their percent complete automatically, as the children tasks are completed and the percent complete of the children is updated. </li>
      <li><span class="bold">Manual</span>: You have to manually update the percent complete and the status of the parent tasks, independently of what changes are made to the children tasks.</li>
     </ul></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Update Type </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Controls when the changes you make to the project timeline are saved on the project or the parent tasks. For example, the following changes to the project trigger an update to the timeline of the project:
     <ul>
      <li>Update the dates of tasks</li>
      <li>Change predecessor relationships of tasks</li>
      <li><p>Change parent-child relationships, adding or removing assignments in addition to changing the task constraint or duration type.</p><p>When the tasks update, their parent objects (parent tasks or the project) update at the time indicated by the Update Type. </p><p>Note: If the parent objects do not update immediately after the change when selecting "Automatic and On Change" or "Change Only" Update Type, refresh the page</p><p>Select from the following options: </p><p>- <span class="bold">Automatic and On Change</span> (Default setting): The project timeline is updated each time a change occurs in the project or in another project that the project is dependent on (On Change). The project timeline is also updated each night (Automatic).</p><p>This is the recommended setting for this field because it ensures that the project is always up to date.</p><p>When you perform an action on a task or project that triggers a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer recalculations display briefly as a question mark (between 1 and 5 seconds, or up to a minute for large projects). This indicates that the recalculation is not yet finished, and the dates are subject to change.</p><p>- <span class="bold">Change Only</span>: The project timeline is updated each time a change occurs in the project or in another project that the project is dependent on. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.</p><p>- <span class="bold">Automatic Only</span>: The project timeline is updated each night; the timeline is not updated immediately after changes are made.</p><p>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. However, be aware that you chose this setting, as the project will not update at the same time that the changes are made.</p><p>- <span class="bold">Manual Only</span>: The project timeline is updated only when you select the option to Recalculate Timeline. For more information about manually recalculating the project timeline, see <a href="recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>. </p><p>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</p></li>
     </ul></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Schedule </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select a schedule for your project. This should be the same schedule assigned to most people that are working on the project. You must create a schedule before you can assign it to a project or a user. If you have not created custom schedules in your system, the Default Schedule is selected.</p> <p>For more information about creating schedules, see <a href="create-schedules.md" class="MCXref xref">Create a schedule</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">User Time Off </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Determines whether the time off of the Primary Assignee of a task adjusts the task planned dates on the project. </p><p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span><span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span></span> selects the default for this setting for your system <span>or your group</span>. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p><p>Select from the following options:<br>- <span class="bold">Consider user time off in task durations</span>: When selecting this option, the planned dates of the tasks adjust according to the time off of the Primary Assignee of the task, if the time off occurs during the duration of the task. </p><p>For example, if a task with a constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, when this selection is enabled the task planned dates are June 1 to June 4. Depending on the Task&nbsp;Constraint, the following scenarios exist: </p>
    <ul>
     <li>For task constraints that relate to planning from a start date (As Soon As Possible, Earliest Available Time, Start No Earlier Than, Start No Later Than, Must Start On) the Planned Start Date does not change but the Planned Completion Date changes.</li>
     <li>For task constraints that relate to planning from a completion date (As Late As Possible, Latest Available Time,&nbsp;Finish No Earlier Than, Finish No Later Than, Must&nbsp;Finish On), the Planned Completion Date does not change, but the Planned Start&nbsp;Date changes.</li>
     <li>For tasks with a constraint of Fixed&nbsp;Dates, neither the Planned Start nor Completion Date changes. </li>
    </ul><p>Important: The Duration of the task does not change when you select this setting. Only the planned dates change, depending on the Task Constraint. For information about task constraint, see <a href="task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>. </p><p>- <span class="bold">Ignore user time off in task durations</span>: When selecting this option, the planned dates of the tasks on the project remain as originally planned, even if the Primary Assignee of the task has time off during the duration of the task. </p><p>Consider the following when selecting options for this setting:</p>
    <ul>
     <li><p>The default option for this setting for a new project is the same as the system-level project preference. </p><p>For information about the project preferences at the System level, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p></li>
     <li>When you attach a template to an existing project, the setting on the project is updated to match the one of the template. </li>
     <li><p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> decides which planned task dates to adjust according to the Task Constraint value of the task. Depending on what that is, either the Planned Start or the Planned Completion Date, or both could be affected, or might even remain the same. For example, if a task has a Constraint of Fixed Dates, the dates do not adjust when the Primary Assignee has time off, even when <span class="bold">Consider user time off in task durations</span> is selected. </p></li>
    </ul></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Resource Leveling Mode </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> <p>Select from the following options:</p> <p>- <span class="bold">Manual</span>: you must manually level your resources (this is the default setting)</p> <p>- <span class="bold">Automatic</span>: <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> levels your resources.</p> <p>For more information about Resource Leveling, see <a href="level-resources-in-gantt.md" class="MCXref xref">Level Resources in the Gantt Chart </a>.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Risk </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>Define the level of risk of your project. The risk is just an indicator of how risky a project can be. You can prioritize the execution of your projects based on the level of risk.</p> <p> <p>Consider selecting from the following levels of risk:</p> <p>- Very Low</p> <p>- Low</p> <p>- Medium</p> <p>- High</p> <p>- Very High</p> <p>The levels of risks you indicate here cannot be customized.</p> <p>Note: These are not related to the potential Risks that could occur during the life of a project and which you should record in the Risks tab of the project, or in the Business Case. For information about potential project Risks, see <a href="edit-create-risk-types.md" class="MCXref xref">Edit and create risk types </a>. </p> </p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Resource Pools </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> <p>Specify the Resource Pools associated with the project. Resource Pools are collections of users that are needed at the same time for the completion of a project and allow for project budgeting in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span>. For more information about Resource Pools, see <a href="work-with-resource-pools.md" class="MCXref xref">Work with Resource Pools </a>. </p> <p>Note: When you edit projects in bulk, only the Resource Pools that are common to all the projects selected appear in this field. If the projects selected have no shared Resource Pools, this field will be empty. The Resource Pools you specify here will overwrite the projects' individual Resource Pools.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> Allow company-level billing rates to override project-level billing rates</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select this option to allow company-level billing rates to override historical job role rates unless those rates are marked as billed. Enabling this option overrides historical job role rates unless they are marked as billed. <br>For more information, see <a href="override-project-level-with-company-level-billing-rates.md" class="MCXref xref">Override Project-Level Billing Rates with Company-Level Billing Rates</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Require time to be approved for this project</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> Select this option to require the Project Owner to approve time logged on the project. If you are using Billing Records and you select this option, only the approved hours on the project appear as available billable hours for the Billing Records. Approving time on the project is independent of approving timesheets. </p> <p>For more information about requiring time to be approved on a project, see <a href="require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Filter Hour Types</span><span style="font-weight: normal;"> and</span> Hour Types</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>Consider the following:</p> 
     <ul> 
      <li> <p>Select <span class="bold">No</span> to make all project-specific hour types available on the project. (This is the default selection)</p> <p>Or</p> </li> 
      <li>Select <span class="bold">Yes</span> to make only a subset of the project-specific hour types available on the project, then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)</li> 
     </ul> <p>If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). You must select at least one hour type; if you select this option and you do not select any hour types, all hour types are made available on the project.</p> <p>The same hour type selections must be made at the individual user level in order for the user to see these hour type options on the project. For more information about defining hour types at the user level, see <a href="log-time.md" class="MCXref xref">Log time</a>. </p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Reminder Notification</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> <p>Select the Reminder Notification that should be associated with the project. You must configure Reminder Notifications for projects for this field to appear during editing a project. For more information about configuring Reminder Notifications, see <a href="set-up-reminder-notifications.md"><a href="set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a> .</a></p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Approval Process</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the approval process you want to associate with the project. Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> must define system-level Approval Processes before you can associate them with projects. <span>A user with administrative access to Approval processes can also create group-specific approval processes.</span> For more information about creating approval processes, see <a href="create-approval-processes.md" class="MCXref xref">Create an approval process</a>.</p> <p>Consider the following when adding approval processes: </p> 
    <ul> 
     <li>Only active approval processes display in the list. </li> 
     <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.</p> <p>Important: If the group associated with the project changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
     <li> <p>When bulk-editing projects, the following scenarios exist:</p> 
      <ul> 
       <li> <p>When you select projects from the same group, both system-level and group-level approval processes display in this field.</p> </li> 
       <li> <p>When you select projects from different groups, only system-level approval processes display in this field.</p> </li> 
       <li> <p>When any of the projects have a single-use approval process attached, it is replaced by the system-level or group-level approval process you select. </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
  </tr> 
 </tbody> 
</table>



1.  (Optional) Continue editing the following sections, depending on the information you want to modify.  



   Or


   Click `Save`.






### Task Settings {#task-settings}

You can define the defaults that will be associated with all the new tasks when you add them to the project.


For information about how these settings affect creating new tasks, see the section [Task defaults when adding tasks to a project](create-tasks-overview.md#understa) in the article [Create tasks overview](create-tasks-overview.md). 



1. Begin editing your project as described above.
1.  Click `Task Settings` in the left panel. 


   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)



1.  In the `Task Default Approval Process` box, select the task Approval Process you want to associate with all new tasks when you add them to the project. 


   Your *`Workfront administrator`* (or a user with administrative access to Approval processes) must create a system-level approval process for a task before you can associate it with a project. Only active approval processes display in the list. For information about creating Approval Processes, see [Create an approval process](create-approval-processes.md). For information about how changes to the group of the project or changes in the approval process affect approval settings, see [How group and approval process changes affect assigned approval processes](how-changes-affect-group-approvals.md).


   When bulk-editing projects, the following scenarios exist:

    
    
    *  When you select multiple projects from the same group, both system-level and group-specific task approval processes display in this field.
    *  When you select multiple projects from different groups, only system-level task approval processes display in this field.
    
    

1.  In the `Task Default Custom Forms` box, select the custom form or forms that you want to associate with all new tasks when you add them to the project. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Create or edit a custom form](create-or-edit-a-custom-form.md). You can associate up to ten custom forms with a task.
1.  (Optional) Select `Use` *`Work Effort`* `to automatically calculate task Planned Hours` if you want to enable managing task effort by using *`Work Effort`* instead of Planned Hours.


   ![](assets/nwe-work-effort-on-projects-350x182.png)



1.  (Conditional and optional) If you selected Use *`Work Effort`* to automatically calculate task Planned Hours, click the drop-down menu for each level of effort and select a percentage for each level. The following percentage values are defaults:



   >[!TIP] {type="tip"}
   >
   >`When the project Update Type is set to Automatic and you select this setting, the Planned Hours of the tasks update according to the task Duration and the *`Work Effort`* percentage, if they are set to zero. For more information about using *`Work Effort`* to plan effort for a task, see` [Work Effort overview](work-effort.md).



1.  (Optional) Continue editing the following sections, depending on the information you want to modify.


   Or


   Click `Save`.





###  




### Issue Settings {#issue-settings}




1.  Begin editing your project as described above.
1.  Click `Issue Settings` in the left panel.


   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)



1.  (Optional) Deselect the `Allow users to add issues inline` option. It is selected by default. 


   When deselecting this option users cannot add issues inline to the project or the tasks in the Issues section.


   >[!TIP] {type="tip"}
   >
   >Deselect this option if you want to enforce users to complete the New Issue Fields or the custom forms associated with new issues. Enabling users to enter issues inline allows them to bypass the New Issue fields and custom forms when creating issues. For information about setting fields and custom forms for new issues, see [Create a Request Queue](create-request-queue.md). 


   When deselecting this option, users with permissions to add issues to the project or the tasks can do so in the following ways: 

    
    
    *  Click New Issue at the top of the list of issues in the Issues section of the project or of the tasks. 
    *  When the project is configured as a request queue, they can enter a new request in the Requests area. 
    
    


   >[!NOTE]
   >
   >When editing projects in bulk this setting is enabled if at least one project has it enabled and it is disabled if all selected projects have it disabled.



1.  (Optional) Continue editing the following sections, depending on the information you want to modify.


   Or


   Click `Save`.





### Access {#access}




1. Begin editing your project as described above.
1.  Click `Access` in the left panel. 


   ![](assets/nwe-access-in-edit-project-box-350x262.png)



1. Specify the following `Access` information for the project:  

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">When someone is assigned to a task</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Select from <span class="bold">View</span>, <span class="bold">Contribute,</span> or <span class="bold">Manage</span> access to a task. The user assigned to a task is automatically granted this access to the task.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Also grant access to the project</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>Select from <span class="bold">View</span>, <span class="bold">Contribute</span>, or <span class="bold">Manage</span> access to the project. The user assigned to a task is automatically granted this access to the project, as well.<br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">When someone is assigned to an issue</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Select from <span class="bold">View</span>, <span class="bold">Contribute,</span> or <span class="bold">Manage</span> access to an issue. The user assigned to an issue is automatically granted this access to the issue. For more information, see <a href="share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a>.<br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Also grant access to the project</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>Select from <span class="bold">View</span>, <span class="bold">Contribute</span>, or <span class="bold">Manage</span> access to the project. The user assigned to an issue is automatically granted this access to the project, as well.<br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">When someone submits a request: Give them access</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Select from <span class="bold">View</span>, <span class="bold">Contribute</span>, or <span class="bold">Manage</span> access to the request. When the project is also a request queue and a user submits a request to the project, they are granted this access to the request they submitted. For information about setting up a project as a request queue, see <a href="create-request-queue.md" class="MCXref xref">Create a Request Queue</a>.<br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">People from the same company will inherit the same permissions for all requests</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>Select this field if you want people from the same company to have the same access to all the requests on the project, whether they submitted them or not.<br></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">When someone is given access to this project: Give them access to ...</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><p>Select the access options that you want users to have on the project, if the project is shared with them. Select the specific options for their access if they are designated as <span class="bold">Viewers</span>, <span class="bold">Contributors</span>, or <span class="bold">Managers</span> when sharing the project with them. </p><p>Note:  The <span class="bold">Delete</span> access in the <span class="bold">Manage</span> permission level determines whether users can&nbsp;delete the project itself. Users with <span class="bold">Manage</span> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have <span class="bold">Manage</span> permissions to the tasks and issues.&nbsp;</p></td>
  </tr>
 </tbody>
</table>


1.  Click `Save`.





## Edit a project in the project header (limited) {#edit-a-project-in-the-project-header-limited}

You can edit a limited amount of information in the project header. 


![](assets/project-header-350x18.png)




You can edit the following fields in the project header:



* Project name
* Project&nbsp;Owner
*  Planned Completion Date `and time` 


  >[!NOTE]
  >
  >You can edit this field only when the project is scheduled from Completion Date. When the project is scheduled from Start Date, *`Workfront`* calculates the Planned Completion&nbsp;Date and time based on the duration oft he tasks.   




*  Condition


  >[!NOTE]
  >
  >You can edit this field only when the Condition Type of the project is Manual. When the Condition Type is set to Progress Status, *`Workfront`* calculates the condition based on the progress of the tasks. For information, see [Overview of Project Condition and Condition Type](project-condition-and-condition-type.md).   




* Status
* Make approval decisions if you are set as the approver in a current approval process




##  



## Edit projects in bulk {#edit-projects-in-bulk}

You can edit projects in bulk and update all their information at the same time. 


To edit projects in bulk:



1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Projects</span>.</MadCap:conditionalText>` 
1. Select several projects in the list.
1.  Click `Edit`.  



   The `Edit Projects` dialog box opens.


   ![](assets/edit-projects-in-bulk-nwe-350x303.png)



1.   Specify the information on all selected projects in the following sections: 

    
    
    *  Overview
    
    
      For information, see the [Overview](#overview) section in this article.
    
    *  Finance 
    
    
      For information, see the [Finance](#finance) section in this article.
    
    *  Portfolio
    
    
      For information, see the "Project association" section in the [Overview](#overview) section in this article.
    
    *  Settings
    
    
      For information, see the [Project Settings](#project2) section in this article.
    
    *  Access
    
    
      For information, see the [Access](#access2) section in this article.
    
    *  Custom Forms
    
    
      For information, continue with step 7 below. 
    
    *  Tasks
    
    
      For information, see the [Task Settings](#task) section in this article.
    
    *  `Issues` 
    
    
      `For information, see the` ` [Issue Settings](#issue)` `section in this article.` 
    
    *  Comment
    
    
      For information, continue with step 9 below. 
    
    
    


   >[!NOTE]
   >
   >The information you are changing on all the projects selected will override the existing information on individual projects, except for the `Resource Manager` field. Adding a new resource manager in bulk edit will add that manager to all the selected projects. If other resource managers are associated with the selected projects, they will remain on the projects in addition to the one added through bulk edit. 



1.  (Optional) In the Settings area, select any of the following options:  


    
    
    * `Recalculate Costs and Revenues`: Select this option to recalculate Costs and Revenues on all projects selected.
    * `Recalculate Timelines`: Select this option to recalculate the Timelines of all projects selected.
    * `Recalculate Scorecards`: Select this option to recalculate the Scorecard values for all projects selected. 
    
    
   ![recalculate_costs__scorecards__etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)



1.  Click `Custom Forms` to edit the custom forms attached to all the projects selected.  



   If the projects selected do not have any common custom forms, no forms are listed in this section.  



   You can edit only the fields on the forms that are attached to all projects selected and which you have permissions to edit. 

1.  (Optional) In the Custom Forms section, select the `Recalculate Custom Expressions` option to ensure that all Calculated Custom Fields that are on the Custom Forms attached to the projects selected are up to date. 


   >[!IMPORTANT] {type="important"}
   >
   >We recommend not to select more than 500 projects at a time when you recalculate custom expressions. 



1.  (Optional) Click `Comment`, then select the Post an update to each project box and specify a comment that you want to display in the updates stream of the project in the available field and do one of the following:

    
    
    *  Click the `People` icon ![](assets/people-icon-updates-classic.png) to tag a user who will be notified about your comment.
    *  Click the `Lock` icon ![](assets/lock-icon-open-updates-classic.png) to restrict your comment only to people within your company. 
    
    
   This comment is visible for everyone with View access to the project and with access to view Notes.

1.  Click `Save Changes`.  



   All changes you made are now visible on all the selected projects. 



