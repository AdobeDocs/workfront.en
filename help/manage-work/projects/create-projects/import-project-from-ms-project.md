---
filename: import-project-from-ms-project
product-area: projects
navigation-topic: create-projects
---



# Import a project from Microsoft Project {#import-a-project-from-microsoft-project}

You can import projects from Microsoft Project into *`Adobe Workfront`* and manage all your projects in one application. Every time you import a project from Microsoft Project, a new project is created in *`Workfront`*. 


>[!IMPORTANT] {type="important"}
>
>Not all Microsoft Project fields are transferred to *`Workfront`*. 
>
>
>For more information about the compatibility of fields between *`Workfront`* and Microsoft Project, see [Map Microsoft Project fields to Adobe Workfront](map-ms-project-fields-to-workfront.md).





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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information about access to projects, see <a href="grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create a project from a MS&nbsp;Project {#create-a-project-from-a-ms-project}

You can create a project from the Projects area in the`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>`, or from the Projects area of a portfolio or a program. 



1. Go to Microsoft Project and open a project that you want to import from in *`Workfront`*. 
1. Click `File`, then `Save As` to save the project as an .xml file. 

1. Log in to *`Workfront`*. 
1.  Do one of the following:

    
    
    *   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> <img src="assets/main-menu-icon.png">, click  <span class="bold">Projects</span>, then expand  <span class="bold">New Project</span>. </MadCap:conditionalText>` 
    *   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a portfolio, then expand  <span class="bold">New Project</span>.</MadCap:conditionalText>` 
    *   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a program, then expand  <span class="bold">New Project</span>.</MadCap:conditionalText>` 
    *  If you are a *`group administrator`*, you can also create a project in the Projects section of a group you manage. For more information, see [View and create projects from the Groups area in the new Adobe Workfront experience](view-manage-projects-groups-area.md).
    
    

1.  Choose the `Import MS Project` option. 


   ![](assets/new-project-dropdown-nwe-350x358.png)



1. Click `Select File`, then browse for the .xml file on your computer which you exported from Microsoft Project. 
1.  Import the selected file.


   *`Workfront`* begins the import process and creates a new project based on the file exported from Microsoft Project.  



   After the import process is complete, you are directed to the new project page that displays a confirmation that the import has completed successfully.


   >[!NOTE]
   >
   >*`Workfront`* has a 15-minute time limitation on file uploads. If the file upload takes longer than that, we recommend that you break out your project into smaller projects and import them separately. Once they have been imported into *`Workfront`*, move the tasks from one project to the other project to combine them into one project. For information on moving tasks, see [Move tasks](move-tasks.md).



1.  (Optional) Continue editing the project in *`Workfront`*. For information about editing projects, see [Edit projects](edit-projects.md).


   The status of a new project created from a template corresponds with the status defined by your *`Workfront administrator`* in the Project Preferences area `or by a` *`group administrator`* `in the Group Project Preferences area.` For information about configuring project preferences, see [Configure system-wide project preferences](set-project-preferences.md).



