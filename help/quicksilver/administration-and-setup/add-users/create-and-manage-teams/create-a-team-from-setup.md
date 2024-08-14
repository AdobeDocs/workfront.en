---
title: Create a Team from the Setup Area
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: As an Adobe Workfront administrator, you can create a team from the Setup area.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
---
# Create a team from the Setup area

As an Adobe Workfront administrator, you can create a team from the Setup area. For information about teams, see [Teams overview](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* A group administrator can create a team for a group they administer from the Setup area. For more information, see [Create and modify a group's teams](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* A user with a Plan license can also create a team from the People area. For more information, see [Create a team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Create a team

{{step-1-to-setup}}

1. Click **Teams**, then click **New Team**.

1. In the **New Team** box that displays, specify the following information:

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
      <td> <p>If you want to associate the team with a group, start typing the name of the group, then select the name when it appears.</p> <p>You can make sure you are associating the right group with the team by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTE</b>: When a team is assigned to a group or subgroup, any group administrators of that group or subgroup can manage the team without being a member of it. Group administrators can go to the Teams area from the Main Menu and click the Switch Teams arrow <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">This is an Agile Team</td> 
      <td>Select this item if you want to configure this new team to be an agile team. For more information about agile teams, see <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Create an agile team</a>.</td> 
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

1. Click **Create Team**.

## Team owners

When you create a team you become the team owner, by default.

You can view team owners for all the teams when you create a report for teams and include the Owner Name field in your report. (For more information about creating a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
