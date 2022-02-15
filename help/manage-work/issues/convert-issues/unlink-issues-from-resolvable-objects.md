---
filename: unlink-issues-from-resolvable-objects
product-area: projects
navigation-topic: convert-issues
---



# Unlink issues from their Resolving Objects {#unlink-issues-from-their-resolving-objects}

When you create a project or a task by converting an issue to the project or task, you have the option to keep the original issue. Your *`Adobe Workfront administrator`* must enable this preference for you to have this option during the conversion of the issue.  
For more information about converting issues to projects and tasks, see [Overview of converting issues in Adobe Workfront](convert-issues.md).


When you decide to keep the issue which was converted to the project or the task, the resolution of the issue is tied to the project or the task. The issue becomes the Resolvable Object of the project or the task. The project or task are the Resolving Objects of the issue.


You can also manually link an issue to another issue. The second issue becomes the Resolving Object for the first issue, in this case.  
For more information about Resolving Objects, see [Overview of Resolving and Resolvable Objects](resolving-and-resolvable-objects.md).


>[!TIP] {type="tip"}
>
>The issue status cannot be changed, as it changes automatically with the status of the Resolving Object. 


You can unlink the resolution of an issue from that of a project, task, or issue by removing the project, task, or issue from the issue. 


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Issues</p> <p>View access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Unlink an issue from a project, task, or issue {#unlink-an-issue-from-a-project-task-or-issue}




1. Go to the issue that is linked to a project, task, or issue.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Issue Details</span> section.</MadCap:conditionalText>`
1.  Go to the `Overview` area of the `Issue Details` section. 
1.  In the `Resolved By` field, remove the resolvable object type.   
   An issue can be resolved by a project, task or issue.  



   This removes the resolving object from the issue. 

1. Click `Save``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">Changes</span></MadCap:conditionalText>`.  
   The issue is no longer linked to a project, task, or issue, and you can now resolve the issue independently. 



