---
filename: project-condition-and-condition-type
title: Overview of Project Condition and Condition Type
content-type: overview
product-area: projects
navigation-topic: manage-projects
---



# Overview of Project Condition and Condition Type {#overview-of-project-condition-and-condition-type}



##  

The project Condition is a visual representation of how the project is progressing. It is a reportable variable determined by the relationship between the planned, projected, and estimated dates of the project.



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
     <li> <p>Contribute permissions to a project to edit the Condition&nbsp;Type in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit the Condition&nbsp;Type in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.



## Project Condition overview {#project-condition-overview}

The Condition of a project can be set in the following ways:



* Manually, by users who have access to Manage the project and when the Condition Type of the project is set to Manual.
* Automatically, by *`Adobe Workfront`*, when the Condition Type of the project is set to Progress Status. The Progress Status of the project is determined by the progress of the tasks on the project. 


For information about how to update the Condition Type of the project, see the section [Set the Condition Type for a project](#set) in this article. 


Consider the following in understanding the Condition of a project: 



* As the project owner, you can decide whether the Condition Type of a project is set manually, or if *`Workfront`* specifies the project Condition, based on the Progress Status of the project. The progress of the tasks on the project influence the Progress Status of the project. For information about the Progress Status of the project, see [Project Progress Status overview](project-progress-status.md).

*  When allowing *`Workfront`* to estimate the Condition of the project automatically, we recommend that you use predecessors on your tasks so that the task progress reflects in the actual progress and the Progress Status of the project.
*  As a project owner, you can change the project to use a Manual Condition Type instead of using the Progress Status by changing the Condition Type from Progress Status to Manual.


  >[!NOTE]
  >
  >Projects that are in any of the following statuses are always marked as On Target, no matter what the dates of the tasks and their progress are:  

  >
  >    
  >    
  >    * Idea
  >    * Requested
  >    * Approved
  >    * Rejected 
  >    
  >    








## Set the Condition Type for a project {#set-the-condition-type-for-a-project}




1. Go to the project for which you want to update the Condition Type. 
1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">More</span> menu  <img src="assets/qs-more-menu.png"> to the right of the project name, then click  <span class="bold">Edit</span>. </MadCap:conditionalText>`   

1. In the `Condition Type` field, choose one of the following: 
    
    
    * `Manual:`The project owner sets the Condition on the project manually.
    
    
      In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. 
    
    * `Progress Status:` *`Workfront`* sets the Condition based on the Progress Status of the project.   

    
    

1. Click `Save Changes`. 




## How *`Workfront`* updates Project Condition based on Progress Status {#how-workfront-updates-project-condition-based-on-progress-status}

When the Condition Type of the project is set to Manual, you can determine what the Condition of the project is independently from the Progress Status of the project. 


However, we recommend that you set the Condition Type of the project to Progress Status so that you can have a clear indication of what the true progress of the project is, based on the progress of your tasks. For information about how *`Workfront`* calculates the Progress Status of projects, see [Project Progress Status overview](project-progress-status.md).


In this case, the values for the Project Condition can be:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 402px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;text-align: left;">Project&nbsp;Condition</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;text-align: left;">Project Progress Status</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;text-align: left;"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Condition Indicator</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="text-align: left;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">On Target</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <li>When Progress Status of the project of On Time, the Condition of the project is <span class="bold">On&nbsp;Target</span>.</li> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="text-align: center;"> <img src="assets/on-target-condition-icon.png"> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">At Risk</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">When the Progress Status of the project is <span class="bold">Behind</span> or <span class="bold">At Risk</span>, then the Condition of the project is <span class="bold">At Risk</span>.</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="text-align: center;"> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">In Trouble</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">When the Progress Status of the project is <span class="bold">Late</span>, then the Condition of the project is <span class="bold">In Trouble</span>. </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="text-align: center;"> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">&nbsp;</td> 
  </tr> 
 </tbody> 
</table>



>[!NOTE]
>
>Conditions can be customized for your environment, so you may find more than three options for Condition in your environment. The names of the Conditions might be different than the ones listed above. For information about customizing Conditions in , see the article [Create or edit a custom condition](create-edit-custom-conditions.md).




## Report on Project Condition, Project Condition Update, and Last Condition Note {#report-on-project-condition-project-condition-update-and-last-condition-note}

In the view of a project report, you can show the following fields related to the Condition of the project:



* `Project Condition:` Shows the current Condition of the project. 
* `Project Condition Update`: Shows the most recent update that the project owner has provided in the update stream of the project, along with the new Condition.   
  Comments made on Condition updates are not displayed in the `Condition Update` column; only the main update is displayed. 

* `Last Condition Note`: Displays the update last entered on an object by the owner of the object. This field is helpful to display the owner's most recent activity or interaction on an object.   
  The `Last Condition Note` column is empty if the note text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column.



For information about how to create a report, see the article [Create a custom report](create-custom-report.md).  

