---
filename: manually-tie-resolution-of-issue-to-ptis
product-area: projects
navigation-topic: convert-issues
---



# Manually tie the resolution of an issue to other issues, tasks, or projects {#manually-tie-the-resolution-of-an-issue-to-other-issues-tasks-or-projects}

You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue. 


>[!TIP] {type="tip"}
>
>When you tie the resolution of an issue to the resolution of another object you can no longer manually edit the status of the original issue. 


For more information about resolving and resolvable objects, see [Overview of Resolving and Resolvable Objects](resolving-and-resolvable-objects.md).


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Issues,&nbsp;Tasks, Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you begin, you must:



*  Have an issue whose resolution you want to tie to the resolution of another issue, task, or project





* Have an additional issue, task, or project 





## Tie the resolution of an issue to the resolution of a another issue, task, or project {#tie-the-resolution-of-an-issue-to-the-resolution-of-a-another-issue-task-or-project}




1. Navigate to an issue whose resolution you want to tie to the resolution of another issue or a task or project.
1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Issue Details</span> >  <span class="bold">Overview </span>area.</MadCap:conditionalText>`


   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)



1.  Go to the `Overview` area in the `Issue Details` section. 
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Resolved By</span> field,</MadCap:conditionalText>` and select from the following types of resolving objects: &nbsp; 
    
    
    * `Project`
    * `Task`
    * `Issue`
    
    

1. The field for the resolving object displays. 
1. After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. 
1. Click `Save`  `Changes`.  
   The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5. This means that the original issue completes when the resolving object (the project, task, or issue you linked it to) is completed.   


   >[!NOTE]
   >
   >One project, task, or issue may have multiple issues as Resolvable Objects.





&nbsp;
