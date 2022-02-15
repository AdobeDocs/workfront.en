---
filename: create-project-from-template
product-area: projects;templates
navigation-topic: create-projects
---



# Create a project using a template {#create-a-project-using-a-template}

You can use templates as a framework to create new projects. If you have projects that repeat often, using templates for the general timeline of the new project saves you from having to build the same projects repeatedly. 


Templates provide you with a way to capture all of the repeatable processes, information, and settings associated with your projects. All of the information associated with a template is transferred to the project. This includes tasks, assignments, durations, documents, financial details, risks, custom forms. 


>[!TIP] {type="tip"}
>
>The status of a new project created from a template corresponds with the status defined by your *`Workfront administrator`* in the main Project Preferences area `or by a` *`group administrator`* `(or *`Workfront administrator`*) in the Project Preferences area for a group.` For information about configuring project preferences, see [Configure system-wide project preferences](set-project-preferences.md) or [Configure project preferences for a group](configure-project-preferences-group.md).


You have the following options for creating a project from a template:



* Create a project from a template in the Projects area
* Create a project from a template at the template level
*  Attach a template to an existing project


  For information, see [Attach a template to a project](attach-template-to-project.md). 

* Create a project from a template in the Groups area




## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> licenses overview*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects and to Templates</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information about access to projects, see <a href="grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create a project from a template in the Projects area {#create-a-project-from-a-template-in-the-projects-area}

You can create a project from the Projects area in the`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>`, or from the Projects area of a portfolio or a program. 




1.  Do one of the following:

    
    
    *   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span>  <img src="assets/main-menu-icon.png">, click  <span class="bold">Projects</span>, then expand  <span class="bold">New Project</span>. </MadCap:conditionalText>`
    *   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a portfolio, then expand  <span class="bold">New Project</span>.</MadCap:conditionalText>`
    
    
      >[!TIP] {type="tip"}
      >
      >When you create a project using a template from a portfolio, the Portfolio field of the new project updates to display the portfolio you chose to create the project from. This overwrites the Portfolio field on the template, if it is specified. 
    
    
    
    *   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a program, then expand  <span class="bold">New Project</span>.</MadCap:conditionalText>`
    
    
      >[!TIP] {type="tip"}
      >
      >When you create a project using a template from a program, the Program field of the new projects updates to display the Program you chose to create the project from. The Portfolio field of the template updates to display the portfolio of the program you chose to create the project from. This overwrites the Program and Portfolio fields on the template, if they are specified. 
    
    
    
    *  If you are a *`group administrator`*, you can also create a project in the Projects section of a group you manage. For more information, see [View and create projects from the Groups area in the new Adobe Workfront experience](view-manage-projects-groups-area.md).
    
    
      >[!TIP] {type="tip"}
      >
      >When you create a project using a template from a group, the group you create the project from displays in the Group field of the new project only when the Group field of the template is not specified. If the template Group field is specified, the Group field of the new project is that of the template. 
    
    
    
    
    


   >[!NOTE]
   >
   >If you have the Milestone View applied to the list of projects, follow the steps in the following section: [Create a project from a template](https://one.workfront.com/s/document-item?bundleId=workfront-classic&topicId=Content%2FManage_work%2FProjects%2FCreate_projects%2Fcreate-project-from-template.html#Create).


   ![](assets/new-project-dropdown-nwe-350x358.png)



1.  Click the name of a template in the `Favorite templates` list


   Or 


   Do the following:

    
    
    1.  Select `New Project from Template`.
    1.  In the `Search Templates` field, start typing the name of a template and click it when it displays in the list. 
    1.  Review template details on the right. 
    
       The template details include the following:
    
        
        
        *  Template duration
        *  Template owner
        *  The number of top-level tasks which includes the names of the top three tasks
        *  The number of all tasks in the template
        *  The names of the template custom forms
        
        
    
    1.      
       (Optional) Hover over the name of a template name and click the `Favorites` `icon` ![](assets/favorites-icon-small.png) to mark it as a favorite for future use. 
    
    
       Or
    
    
       Expand the `Favorite templates` list and select a template from the drop-down list. 
    
    
       >[!TIP] {type="tip"}
       >
       >You can have up to 40 *`Workfront`* items marked as favorites. This includes templates and other items.
    
    
    1.  Click `Use template` when you have selected a template.
    
    
   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)



1.  The `New Project` box opens.&nbsp;


   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x285.png)



1.  If a field is already populated in the template, the field is pre-populated in the `New Project`box. You can edit the pre-populated values to better match your project. For more information, see [Edit projects](edit-projects.md).
1.  Click `Create Project`.


   All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step. 





## Create a project from a template in the Templates area {#create-a-project-from-a-template-in-the-templates-area}

Instead of starting in the Projects area, you can create a project from a template by starting with the template. 


&nbsp;




1. From the `Main Menu`, click `Templates`.

1. Click the name of a template you want to use.
1.  Click the `More` menu ![](assets/more-icon.png), then click `Create Project.`


   ![](assets/create-project-from-template-template-level-nwe-350x179.png)




   The `New Project` box opens.&nbsp;

1.  Specify a name for the project, then review each section and make any necessary changes. 


   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x285.png)




   If a field is already populated in the template, the field is pre-populated in the `New Project`box. You can edit the pre-populated values to better match your project. For more information, see [Edit projects](edit-projects.md).

1.  Click `Create Project.`


   All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step. 



&nbsp;
