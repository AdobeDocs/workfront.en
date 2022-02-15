---
filename: assign-users-to-layout-template
title: Assign users to a Layout Template
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
---



# Assign users to a layout template {#assign-users-to-a-layout-template}

As an *`Adobe Workfront administrator`*, you can assign a layout template you have created to any user, job role, team, or group who needs to use it. 


For users that do not have a layout template assigned to them, the default layout is used. To learn about the default layout, see [About the default Adobe Workfront layout](about-the default-wf-layout.md).


Users can also assign a layout template to themselves, as described in Change the My Work and Work Requests areas with layout templates.


You can assign multiple different layout templates to the same name. For more information about which layout template is in effect for a user, role, group, or team, see [Layout template assignment priority](#layout) later in this article.


For more information about layout templates, see [Layout templates](_use-layout-templates-customize-ui.md).


For information about layout templates for groups, see [Create and modify a group’s layout templates](create-and-modify-a-groups-layout-templates.md).


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Assign a layout template to users {#assign-a-layout-template-to-users}




1.  Begin working on a layout template, as described in [Create and manage layout templates](create-and-manage-layout-templates.md).


   >[!TIP] {type="tip"}
   >
   >When you are satisfied with your layout template, we recommend that you test it, as described in [Testing a new layout template](test-a-layout-template.md).



1. Click `Assign this to` in the top section of the page.
1.  In the box that appears, click `Add a User, Job Role, Team, or Group`, start typing the name of a user, job role, team, or group, then click the name when it appears in the drop-down.


   Recently added names display with a blue background. This is helpful when you are editing an existing layout template because you can distinguish the names you have just added from those that were already in the list.


   An Info icon ![](assets/info-icon.png) displays to the right of the name of any user, job role, team, or group that is already assigned to another layout template. You can hover over the icon to see the name of that layout template and decide whether you want to override the existing assignment.

1.  Repeat the two previous steps to assign the layout template to other users, job roles, teams, or groups as needed.


   You can assign up to 100 users at a time. 

1.  Click `Done`, then click `Save` in the lower-left corner.


   This step completes the process of creating and assigning a layout template.





## Layout template assignment priority {#layout-template-assignment-priority}

You and other *`Workfront administrators`* can assign multiple different layout templates to the same user in these four different ways: 



* To the individual user
* To a particular job role the user has
* To a certain team the user is on
* To a certain group the user is in


However, only one layout template is visible to the user at any given time.&nbsp;The template that is visible is determined by the following priority hierarchy:



*  `Individual user`: The layout template assigned to the person as an individual user overrides all others. You can override a previous assignment made so an individual user by making a new assignment; the most recent one takes precedence. 
*  `Primary job role`:&nbsp;If the person is not assigned a layout template as a single user, they see the&nbsp;template assigned for their primary job role.


  Only the layout template assigned to the primary job role of a user is visible to the user. Templates assigned to any secondary job roles held by the user are not visible.

*  `Home team`: If the person is not assigned a layout template as an individual user, nor as a user with a primary job role, they see the template assigned to their Home team.


  Only the template assigned to the Home team of a user is visible to the user. Templates assigned to other teams where the a user is a member are not visible.

*  `Home group`:&nbsp;If the person is not assigned a layout template as an individual user, nor as a user with a primary job role, nor as a member of a Home team, they see the template assigned to their Home group.


  Only the template assigned to the Home group&nbsp;of a user is visible to the user. Templates assigned to any of their other groups are not visible.&nbsp;





## Large numbers of users assigned to a layout template {#large-numbers-of-users-assigned-to-a-layout-template}

If you edit a&nbsp;layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.


If you have more than 2000 users to assign to a layout template, we recommend that you do one of the following:



* Organize the users into groups or teams and assign the layout template to those groups or teams. For more information, see [Create a group](create-a-group.md) and [Create and manage teams](_create-and-mange-teams.md).

* Assign job roles to the users and assign the layout template to their primary job role. For more information, see [Create and manage job roles](create-manage-job-roles.md).


