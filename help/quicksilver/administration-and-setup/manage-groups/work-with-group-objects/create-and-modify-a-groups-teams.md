---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Create and modify a group's teams
description: When you are viewing a group that you manage in the Groups area, you can view and work with teams associated with the group and any of its subgroups.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
---
# Create and modify a group's teams

When you are viewing a group that you manage in the Groups area, you can view and work with teams associated with the group and any of its subgroups.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

For information about how users with a Plan license can create a team, see [Create a team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

For information about how a Workfront administrator can create a team, see [Create a team from the Setup area](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## View, work with, and create teams for your group from the Groups area

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Click the name of the group for which you want to create or modify teams.
1. In the left panel, click **Teams** ![](assets/teams.png) to list the teams associated with the group and with any subgroups it may have.

1. Do any of the following:

   * **Add a team**: Click **New Team**, then use the following options to configure it:

   <!-- WRITER please check table below. I stripped out wonky conditions-->

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Team Name</td> 
       <td>Type a name for the team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Group</td> 
       <td> <p> The system fills in the Group field for the new team with the group you are viewing. If you want to associate the team with a different group, start typing the name of the group, then select the name when it appears.</p> <p>You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTE</b>: When a team is assigned to a group or subgroup, any group administrators of that group or subgroup can manage the team without being a member of it. Group administrators can go to the Teams area from the Main Menu and click the Switch Teams arrow <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Team Members</td> 
       <td> <p>Begin typing the name of a user to be on the team, then select the name when in appears in the drop-down list. Repeat this process to add multiple users to the team.</p> <p>There is no limit to how many users you can add to a team. However, we recommend to not have an excessively large number of users in one team, because the team's work management might become too complex.</p> </td> 
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
       <td>Select the status that you want set for items when the Done button is clicked.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Edit teams**: Select at least one team, click **the** Edit icon ![](assets/edit-icon.png), then use the following options to configure it:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Team Name</td> 
       <td>Type a name for the team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Group</td> 
       <td> <p>Associate the team with a group. Start typing the name of the group, then select the name when it appears.</p> <p>You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTE</b>: When a team is assigned to a group or subgroup, any group administrators of that group or subgroup can manage the team without being a member of it. Group administrators can go to the Teams area from the Main Menu and click the Switch Teams arrow <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Owner</td> 
       <td>Select an owner for the team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Team Members</td> 
       <td> <p>Add and team members. Start typing the name of a user, then select the name when it appears. Repeat this process to add multiple users to the team.</p> <p><b>TIP</b>: There is no limit to how many users you can add to a team. However, we recommend to not have an excessively large number of users in one team, because the team's work management might become too complex.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Description</td> 
       <td>Type a description for the team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Layout Template</td> 
       <td> <p>Start typing the name of the layout template you want the team to use, then click it when it appears.</p> <p>When you designate the team with this layout template as the Home Team of users, all users in this team will see the customizations in this layout template.<br>Their individual layout template settings will override the settings of the home team layout template. </p> </td> 
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
     </table>

   * **Delete teams**: Select at least one team, then click the Delete icon ![](assets/delete.png).
   * **Export the list of teams**: Click **Export** ![](assets/export.png), then select the file format you want for the exported list.
