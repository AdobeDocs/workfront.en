---
filename: create-and-modify-a-groups-teams
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
---



# Create and modify a group’s teams {#create-and-modify-a-group-s-teams}

When you are viewing a group that you manage in the Groups area, you can view and work with teams associated with the group and any of its subgroups.


If there are any groups above your group, their administrators can also do these things for your group. The same is true for *`Workfront administrators`* (for any group).


For information about how users with a *`Plan`* license can create a team, see [Create a team](create-a-team.md).


For information about how a *`Workfront administrator`* can create a team, see [Create a team from the Setup area](create-a-team-from-setup.md).


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## View, work with, and create teams for your group from the Groups area {#view-work-with-and-create-teams-for-your-group-from-the-groups-area}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1. Click the name of the group for which you want to create or modify *`teams`*.
1. In the left panel, click `Teams` ![](assets/teams.png) to list the teams associated with the group and with any subgroups it may have.

1.  Do any of the following:

    
    
    *  `Add a team`: Click `New Team`, then use the following options to configure it:
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Team Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name for the team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
      The system fills in the Group field for the new portfolio with the group you are viewing. 
     </MadCap:conditionalText>If you want to associate the team with a <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
      different 
     </MadCap:conditionalText>group, start typing the name of the group, then select the name when it appears.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
       Depending on the details configured for the group, you might also see its Business Leader and description.
     </MadCap:conditionalText></p> <p>Note: When a team is assigned to a group or subgroup, any <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> of that group or subgroup can manage the team without being a member of it. <span class="mc-variable WFVariables.AdminGroupInitCapPlur variable varname">Group administrators</span> can go to the Teams area from the Main Menu and click the Switch Teams arrow <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Team Members</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Begin typing the name of a user to be on the team, then select the name when in appears in the drop-down list. Repeat this process to add multiple users to the team.</p> <p>There is no limit to how many users you can add to a team. However, we recommend to not have an excessively large number of users in one team, because the team’s work management might become too complex.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Type a description for the team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Calendar</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Choose which calendar tab will appear for this team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Work On It</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Change the Work On It button to a Start button. When a user clicks Start, the status of the item is updated automatically.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Done Button</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Select the status that you want set for&nbsp;items when the Done button is clicked.</td> 
  </tr> 
 </tbody> 
</table>    
    
    
    *  `Edit teams`: Select at least one team, click `the`Edit icon ![](assets/edit-icon.png), then use the following options to configure it:
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Team Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name for the team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Associate the team with a group. Start typing the name of the group, then select the name when it appears.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
       Depending on the details configured for the group, you might also see its Business Leader and description.
     </MadCap:conditionalText></p> <p>Note: When a team is assigned to a group or subgroup, any <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> of that group or subgroup can manage the team without being a member of it. <span class="mc-variable WFVariables.AdminGroupInitCapPlur variable varname">Group administrators</span> can go to the Teams area from the Main Menu and click the Switch Teams arrow <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Owner</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select an owner for the team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Team Members</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Add and team members. Start typing the name of a user, then select the name when it appears. Repeat this process to add multiple users to the team.</p> <p>Tip: There is no limit to how many users you can add to a team. However, we recommend to not have an excessively large number of users in one team, because the team’s work management might become too complex.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a description for the team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Layout Template</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Start typing the name of the layout template you want the team to use, then click it when it appears.</p> <p>When you designate the team with this layout template as the Home Team of users, all users in this team will see the customizations in this layout template.<br>Their individual layout template settings will override the settings of the home team layout template.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Agile</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify whether this is an agile team. For information on agile teams and how to manage their work, see <a href="create-an-agile-team.md" class="MCXref xref">Create an agile team</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Work On It</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Change the Work On It button to a Start button. When a user clicks Start, the status of the item is updated automatically.</p> <p>For more information on how to configure the Start button, see <a href="work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Done Button</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Customize the Done button. For more information, see:</p> 
    <ul> 
     <li><a href="configure-the-done-button-for-tasks.md" class="MCXref xref">Configure the Done button for tasks</a> </li> 
     <li><a href="configure-the-done-button-for-issues.md" class="MCXref xref">Configure the Done button for issues</a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>    
    
    
    *  `Delete teams`: Select at least one team, then click the Delete icon ![](assets/delete.png).
    *  `Export the list of teams`: Click `Export` ![](assets/export.png), then select the file format you want for the exported list.
    
    



