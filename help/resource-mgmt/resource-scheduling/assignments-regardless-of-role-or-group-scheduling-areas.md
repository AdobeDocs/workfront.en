---
filename: assignments-regardless-of-role-or-group-scheduling-areas
product-area: resource-management;user-management
navigation-topic: resource-scheduling
---



# Allow user assignments regardless of role and group membership in the Scheduling areas {#allow-user-assignments-regardless-of-role-and-group-membership-in-the-scheduling-areas}



>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from *`Adobe Workfront`*. We recommend that you use the *`Workload Balancer`* for scheduling your resources. 
>
>
>For information about scheduling resources using the new *`Workload Balancer`*, see the section [The Workload Balancer](_workload-balancer.md).
>
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the *`Workload Balancer`*, see [Deprecation of Resource Scheduling tools in Adobe Workfront](deprecate-resource-scheduling.md).



By default, assignments can be made only to users who have a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them. 


You can configure *`Adobe Workfront`* to allow tasks and issues to be assigned to any user, regardless of whether that user has a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them. When you assign a user to a task or issue and that user does not have a role that matches the role assignment on the task or issue, the original role assignment is removed, and the role assignment changes to the role of the user you are assigning.



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View or higher access to&nbsp;Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Contribute permissions or higher to the projects, tasks, and issues you update assignments for</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Allow assignments to users regardless of role {#allow-assignments-to-users-regardless-of-role}




1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
    
    
    * **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For an individual project**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Go to a project, click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For a team**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Teams</span>, select a team, click <span class="bold"> <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span> in the left panel, then select <span class="bold"> Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    
1. Click the `Settings` icon on the scheduling timeline.
1. Disable the option `Limit Assignments to Users with Matching Role`.
1. Click `Return to Scheduling`.




## Allow assignments to users regardless of group membership {#allow-assignments-to-users-regardless-of-group-membership}

By default, assignments can be made only to users who are members of the group that is associated with the project (this is the group that is defined when editing the project).


>[!IMPORTANT] {type="important"}
>
>This setting takes into account only the members of the group associated with the project, and not any members of any subgroups of that group. 


You can configure *`Workfront`* to allow tasks and issues to be assigned to any user, regardless of whether that user is a member of the group that is associated with the project where the task or issue resides.



1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
    
    
    * **For multiple projects**:&nbsp; `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click  <span class="bold">Resourcing > <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span>, then select  <span class="bold">Scheduling</span> in the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For an individual project**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Go to a project, click the  <span class="bold"><span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span> </span> section in the left panel, then select  <span class="bold">Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    * **For a team**: `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Teams</span>, select a team, click <span class="bold"> <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span></span> in the left panel, then select <span class="bold"> Scheduling</span> from the upper-left drop-down menu. </MadCap:conditionalText>`
    
    

    
    
    *   
    
    

1. Click the `Settings` icon on the scheduling timeline.
1. Disable the option `Limit Assignments to the Group Associated with the Project`.
1. Click `Return to Scheduling`.


&nbsp;
