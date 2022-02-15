---
filename: remove-users-from-projects
product-area: projects;user-management
navigation-topic: manage-projects
---



# Remove users from projects  {#remove-users-from-projects}

You can remove users from a project when they are no longer involved in completing work on the project. Removing users from projects has implications on task and issue assignments, as well as on project roles.&nbsp;


The users associated with a project are listed in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> People area</MadCap:conditionalText>` of a project. They represent the Project Team.&nbsp;For more information about the Project Team, see [Project Team overview](project-team-overview.md).


You can assign work to the users on the project in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> People area</MadCap:conditionalText>` of a project. 


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


## How removing a user affects existing tasks, issues, and projects&nbsp; {#how-removing-a-user-affects-existing-tasks-issues-and-projects}

When a user is removed from a project, any tasks or issues assigned to them might be affected, depending on whether the task or issue was in an Active or Complete state when the user was removed:



* `If the item is in an Active state when the user is removed:` The item is re-assigned to a Job Role if a Job Role was already assigned. If the item&nbsp;did not have a Job Role assigned, you must manually re-assign the item. An item in an Active state is any item that has not completed yet. 
* `If the item is in a Complete state when the user is removed:` The name of the removed user remains on&nbsp;the item.&nbsp;
*  If the user removed is also the creator of a project, the project is not removed from their `Projects I'm On``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> list</MadCap:conditionalText>` in the Projects area. The project is removed from the lists for all other users that filter for that project by the Entered By field. 




## Remove users from a project and Project Team {#remove-users-from-a-project-and-project-team}

When you remove a user from the project, the user is also removed from the project team. Likewise, when you remove a user from the project team, the user is also removed from the project.


You can remove users from a project from the People `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`of the project. 



* [Remove users from a project from the People area](#remove) 




### Remove users from a project from the People area {#remove-users-from-a-project-from-the-people-area}




1. Go to the project where you want to remove the users.
1. Click `People``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> in the left panel</MadCap:conditionalText>`,&nbsp;then select the users you want to remove. `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> This might be located under the  <span class="bold">Show More</span> area. </MadCap:conditionalText>`  

1. Click `Remove.`
1. Click  `Yes, Remove Selected Users` to confirm removal.


