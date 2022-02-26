---
filename: create-and-modify-a-groups-teams
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Create and modify a group’s teams
description: When you are viewing a group that you manage in the Groups area, you can view and work with teams associated with the group and any of its subgroups.
---

# Create and modify a group’s teams

When you are viewing a group that you manage in the Groups area, you can view and work with teams associated with the group and any of its subgroups.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for *Workfront administrators* (for any group).

For information about how users with a *Plan* license can create a team, see [Create a team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

For information about how a *Workfront administrator* can create a team, see [Create a team from the Setup area](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> <p>You must be a <em>group administrator</em> of the group or a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *Workfront administrator*.

## View, work with, and create teams for your group from the Groups area

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Groups</span> <img src="assets/groups-icon.png">.</li> 
 <li value="3">Click the name of the group for which you want to create or modify <em>teams</em>.</li> 
 <li value="4">In the left panel, click <span class="bold">Teams</span> <img src="assets/teams.png"> to list the teams associated with the group and with any subgroups it may have.</li> 
 <li value="5"> <p>Do any of the following:</p> 
  <ul> 
   <li> <p><span class="bold">Add a team</span>: Click <span class="bold">New Team</span>, then use the following options to configure it:</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Team Name</td> 
       <td>Type a name for the team.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Group</td> 
       <td> <p> <draft-comment>
          <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
           The system fills in the Group field for the new portfolio with the group you are viewing. 
          </MadCap:conditionalText>
         </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
          The system fills in the Group field for the new portfolio with the group you are viewing. 
         </MadCap:conditionalText>If you want to associate the team with a <draft-comment>
          <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
           different 
          </MadCap:conditionalText>
         </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
          different 
         </MadCap:conditionalText>group, start typing the name of the group, then select the name when it appears.</p> <draft-comment>
         <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<draft-comment>
           <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
             Depending on the details configured for the group, you might also see its Business Leader and description.
           </MadCap:conditionalText>
          </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
            Depending on the details configured for the group, you might also see its Business Leader and description.
          </MadCap:conditionalText></p>
        </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
           Depending on the details configured for the group, you might also see its Business Leader and description.
         </MadCap:conditionalText></p> <note type="note">
         When a team is assigned to a group or subgroup, any 
         <em>group administrators</em> of that group or subgroup can manage the team without being a member of it. 
         <em>Group administrators</em> can go to the Teams area from the Main Menu and click the Switch Teams arrow 
         <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.
        </note> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Team Members</td> 
       <td> <p>Begin typing the name of a user to be on the team, then select the name when in appears in the drop-down list. Repeat this process to add multiple users to the team.</p> <p>There is no limit to how many users you can add to a team. However, we recommend to not have an excessively large number of users in one team, because the team’s work management might become too complex.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Description</td> 
       <td>Type a description for the team.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Calendar</td> 
       <td>Choose which calendar tab will appear for this team.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Work On It</td> 
       <td>Change the Work On It button to a Start button. When a user clicks Start, the status of the item is updated automatically.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Done Button</td> 
       <td>Select the status that you want set for&nbsp;items when the Done button is clicked.</td> 
      </tr> 
     </tbody> 
    </table> </li> 
   <li> <p><span class="bold">Edit teams</span>: Select at least one team, click <span class="bold">the</span> Edit icon <img src="assets/edit-icon.png">, then use the following options to configure it:</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Team Name</td> 
       <td>Type a name for the team.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Group</td> 
       <td> <p>Associate the team with a group. Start typing the name of the group, then select the name when it appears.</p> <draft-comment>
         <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<draft-comment>
           <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
             Depending on the details configured for the group, you might also see its Business Leader and description.
           </MadCap:conditionalText>
          </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
            Depending on the details configured for the group, you might also see its Business Leader and description.
          </MadCap:conditionalText></p>
        </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
           Depending on the details configured for the group, you might also see its Business Leader and description.
         </MadCap:conditionalText></p> <note type="note">
         When a team is assigned to a group or subgroup, any 
         <em>group administrators</em> of that group or subgroup can manage the team without being a member of it. 
         <em>Group administrators</em> can go to the Teams area from the Main Menu and click the Switch Teams arrow 
         <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.
        </note> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Owner</td> 
       <td>Select an owner for the team.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Team Members</td> 
       <td> <p>Add and team members. Start typing the name of a user, then select the name when it appears. Repeat this process to add multiple users to the team.</p> <note type="tip">
         There is no limit to how many users you can add to a team. However, we recommend to not have an excessively large number of users in one team, because the team’s work management might become too complex.
        </note> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Description</td> 
       <td>Type a description for the team.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Layout Template</td> 
       <td> <p>Start typing the name of the layout template you want the team to use, then click it when it appears.</p> <p>When you designate the team with this layout template as the Home Team of users, all users in this team will see the customizations in this layout template.<br>Their individual layout template settings will override the settings of the home team layout template.&nbsp;</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Agile</td> 
       <td>Specify whether this is an agile team. For information on agile teams and how to manage their work, see <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Create an agile team</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Work On It</td> 
       <td> <p>Change the Work On It button to a Start button. When a user clicks Start, the status of the item is updated automatically.</p> <p>For more information on how to configure the Start button, see <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Done Button</td> 
       <td> <p>Customize the Done button. For more information, see:</p> 
        <ul> 
         <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configure the Done button for tasks</a> </li> 
         <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configure the Done button for issues</a> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </li> 
   <li> <p><span class="bold">Delete teams</span>: Select at least one team, then click the Delete icon <img src="assets/delete.png">.</p> </li> 
   <li> <p><span class="bold">Export the list of teams</span>: Click <span class="bold">Export</span> <img src="assets/export.png">, then select the file format you want for the exported list.</p> </li> 
  </ul> </li> 
</ol>

