---
filename: work-with-resource-pools
product-area: resource-management
navigation-topic: resource-planning
---



# Work with Resource Pools  {#work-with-resource-pools}

As a resource manager, you can manage your resources by adding users to Resource Pools. 


Populating Resource Pools with users and attaching them to projects is a prerequisite for using the Resource Planning functionality. 


Efficient resource management cannot happen without populating your Resource Pools with users and attaching them to projects.  



For more information about the prerequisites needed before you can start using Resource Planning, see the "Prerequisites for working in the *`Resource Planner`*" section in [Resource Planner overview](get-started-resource-planner.md) .



## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> and higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Resource Management that includes access to Manage Resource Pools</p> <p>Edit access to Projects, Templates, and Users</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Overview of Resource Pools {#overview-of-resource-pools}




* A Resource Pool is a collection of users that are needed at the same time for the completion of a project.
* A Resource Pool can be shared across multiple projects, programs, or portfolios when it is associated with all the projects in the programs and portfolios. 
* You can either create a Resource Pool and populate it with existing users upon its creation, or you can create the Resource Pool and associate it with an existing user or with a new user as you are creating or editing the user. 
* After you populate your Resource Pools with users, you can associate them with projects and templates, and manage your user allocation to the projects more efficiently. 
*  You can associate as many Resource Pools as needed with a project, template, or user. 




## Create a Resource Pool {#create-a-resource-pool}




1. Log in as a user who has access to edit Resource Pools.  
   For more information, see [Create a Resource Pool](#access-to-edit-resource-pools).

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Resourcing</span>. </MadCap:conditionalText>`
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Resource Pools</span> in the left panel. </MadCap:conditionalText>`  
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)


1. Click `New Resource Pool`.
1. Specify the following: 



<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col style="width: 200px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col style="width: 50%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Name</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This is the name of the Resource Pool.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Description</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">This is a brief description about this Resource Pool. For example, you can specify for what purpose it should be used.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">(Optional) <span class="bold">Pool Members</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><p> Add users to the Resource Pool individually.<br>Or <br>To add a large amount of users to the Resource Pool at one time, you can add one of the following entities associated with users. This adds those users to the Resource Pool:
     <ul>
      <li><span class="bold">Teams</span>: all members of the team are added to the Resource Pool.</li>
      <li><span class="bold">Groups</span>: all members of the group are added to the Resource Pool.</li>
      <li><span class="bold">Roles</span>: all users associated with that role are added to the Resource Pool.</li>
      <li><span class="bold">Companies</span>: all users in the company are added to the Resource Pool.</li>
     </ul><p>Tip: You can only add active users, teams, <span>roles,</span> or companies.</p><p>Note:  If a user becomes a member of a group, team, company or is associated with a job role after the group, team, company or job role have been added to the Resource Pool, the new member is not automatically added to the Resource Pool. <br>If a user belongs to the team, group, company, and job role you are adding, at the same time, the user is added only once to the Resource Pool.<br>Users who are deactivated after having been added to the Resource Pool appear dimmed in the list of users and are marked as being deactivated.</p></p></td>
  </tr>
 </tbody>
</table>


1.  (Optional) Use the `Undo` link to remove the users added through a group, team, company or job role.


   >[!NOTE]
   >
   >There is no limit to how many users you can have in a Resource Pool. However, we recommend not adding too many users to a Resource Pool, as Resource Management could become a challenge otherwise. The list of users only shows the first 2,000 users in the Resource Pool, and they are listed alphabetically. 


   ![Resource_pools_NEW___UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)



1. (Optional) Use the `Search` option to find a user in the Resource Pool.
1. Click `Create`.




## Remove users from a Resource Pool {#remove-users-from-a-resource-pool}

You can remove users from a Resource Pool when those users are no longer needed in that pool. 


To remove a user from a Resource Pool:



1. Log in as a user who has access to edit Resource Pools.  
   For more information, see the section [Create a Resource Pool](#access-to-edit-resource-pools) in this article.

1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Resourcing</span>. </MadCap:conditionalText>` 
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Resource Pools</span> in the left panel. </MadCap:conditionalText>` 
1. Select a Resource Pool and click `Edit.  
   `Or  
   Click the name of a Resource Pool. 

1. Start typing the name of a user that you want to remove in the `Search in this Resource Pool` field.  
   Or  
   Start typing the name of a company, job role, team, or group, if you want to remove all the users associated with those entities.  
   ![search_inside_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x321.png)


1. Click the 'x' icon at the user level to remove a user from the Resource Pool. They are removed from all the lists they appear in.  
   Or  
   To remove all users associated with a job role, group, team, or company, click `Remove` at the job role, group, team level, or company level. This removes all the users associated with that job role, group, team, or company from the Resource Pool. 

1. Click `Save`. 




## Associate Resource Pools with users {#associate-resource-pools-with-users}

You must have administrative rights to editing users in order to edit or create users.   
For more information about the access needed to edit or create users, see [Grant access to users](grant-access-other-users.md).



* [How to select users for a Resource Pool](#structuring-resource-pools) 
* [Associate Resource Pools with one user](#associate-pools-with-users-subsections) 
* [Associate Resource Pools with users in bulk](#resource-pools-with-users-in-bulk) 




### How to select users for a Resource Pool {#how-to-select-users-for-a-resource-pool}

There are several ways to structure your Resource Pools. 


We recommend the following scenarios: 



* You can have all the users in the same Resource Pool belong to the same team.  
  For example, if you want all the users of a Marketing team to be available for a project, you would want a Marketing Resource Pool where you would add all the users in that team. You can then associate the Marketing Resource Pool with the project.  

*  You can have all the users in the same Resource Pool fulfill similar roles, especially if the roles are in high demand and must be budgeted separately.  
  For example, you may have external resources that work as Consultants that you want to have available for a project from time to time. You can create a Resource Pool for Consultants that you can attach to your projects, where you can place both users that are internal or external Consultants.  

* You can also create Resource Pools by department or cost center. 
* We do not recommend adding all users in the system to one Resource Pools if you have a large number of users, or if you manage resources for a large number of a projects at a time.  




### Associate Resource Pools with one user {#associate-resource-pools-with-one-user}

You can associate users with Resource Pools when you are creating your Resource Pools.   
For more information about creating a Resource Pool, see the section [Create a Resource Pool](#creating-a-resource-pool) in this article.


If you create Resource Pools without populating them with users, you can later associate them with users as you are editing or creating new users. 


The Resource Pools must be created before you can associate them with a user. 


To associate Resource Pools with users:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Users</span>. </MadCap:conditionalText>` 
1. Check the box next to the name of a user from the list, then click `Edit`.
1. Click `Resource Planning`.
1. Start typing the name of a Resource Pool that you want to associate with the user in the `Resource Pools` field, then select it from the list, when it appears.  
   You can associate multiple Resource Pools with one user.  
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)  

1. Click `Save Changes`.


For more information about editing users, see [Edit a user's profile](edit-a-users-profile.md).


For more information about creating new users, see [Add users](add-users.md).


### Associate Resource Pools with users in bulk {#associate-resource-pools-with-users-in-bulk}

You can edit multiple users in bulk and associate the same Resource Pools with all of them at the same time. 


To associate Resource Pools with several users in bulk:



1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Users</span>. </MadCap:conditionalText>`
1. Select several users on the list, and click `Edit`.
1. Click `Resource Planning`.
1. Start typing the name of a Resource Pool that you want to associate with the users in the `Resource Pools` field, then select it from the list, when it appears.  
   You can associate multiple Resource Pools with multiple users.  


   >[!NOTE]
   >
   >Only the Resource Pools that are common to all the users selected appear in this field. If the users selected have no shared Resource Pools, this field is empty. If this field is empty, the Resource Pools you specify here will overwrite their individual Resource Pools.


  
  

1. Click `Save Changes`.


For more information about how to edit users in bulk, see [Edit user profiles in bulk](edit-user-profiles-in-bulk.md). 


## Associate Resource Pools with projects and templates {#associate-resource-pools-with-projects-and-templates}

After you create Resource Pools, you can associate them with projects or templates so you can later budget your resources on the projects. 


You must have the following rights to associate Resource Pools with Projects and Templates: 



* You must have rights to Edit projects in your access level, as well as Manage permissions on the project in order to edit the project and associate it with Resource Pools.
* You must have rights to Edit templates in your access level, as well as Manage permissions on the template in order to edit the template and associate it with Resource Pools.


We recommend that you create your Resource Pools in advance, associate them with projects, and budget your resources before the project starts. 



* [Associate Resource Pools with one project or template](#associate-pools-with-one-project) 
* [Associate Resource Pools with several projects or templates in bulk](#associate-pools-with-many-projects-and-templates) 




### Associate Resource Pools with one project or template {#associate-resource-pools-with-one-project-or-template}

You can associate Resource Pools with a template in the same manner you associate Resource Pools with a project. 


To associate Resource Pools with a project: 



1. <![CDATA[				]]><![CDATA[			]]>`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a project and click the  <span class="bold">Edit</span> icon  <img src="assets/qs-edit-icon.png">in the upper-right corner.</MadCap:conditionalText>`
1.  Click `Settings`. 
1. Start typing the name of a Resource Pool in the `Resource Pools` field, then select it from the list when it appears.  
   You can associate multiple Resource Pools with one project or template.  
   ![resource_pool_to_project.png](assets/resource-pool-to-project-350x316.png)  
  

1. Click `Save Changes`.


For more information about how to edit a project and associate it with Resource Pools, see [Edit projects](edit-projects.md).


For more information about how to edit a template and associate it with Resource Pools, see [Edit project templates](edit-templates.md).


### Associate Resource Pools with several projects or templates in bulk {#associate-resource-pools-with-several-projects-or-templates-in-bulk}

You can edit multiple projects or templates in bulk and associate the same Resource Pools with all of them at the same time. 


You can associate Resource Pools with templates in the same manner you associate Resource Pools with projects. 


To associate Resource Pools with several projects in bulk:



1. Go to a list of projects.
1. Select multiple projects, then click `Edit`.
1. Click `Settings`.
1.  Start typing the name of a Resource Pool in the `Resource Pools` field, then select it from the list when it appears.  
   You can associate multiple Resource Pools with the projects or templates. 


   >[!NOTE]
   >
   >When you edit projects or templates in bulk, only the Resource Pools that are common to all the projects or templates selected appear in this field. If the projects selected have no shared Resource Pools, this field will be empty. The Resource Pools you specify here will overwrite the individual Resource Pools of the projects or templates. 



1. Click `Save Changes`.   
   When your Resource Pools are associated with your projects or your templates, you can budget user allocations for your projects inside the *`Resource Planner`*.   
   For more information about the *`Resource Planner`*, see [Resource Planner overview](get-started-resource-planner.md).



For more information about how to edit projects in bulk, see the "Edit projects in bulk" section in [Edit projects](edit-projects.md).


For more information about how to edit templates in bulk, see the "Edit templates in bulk" section in [Edit project templates](edit-templates.md).
