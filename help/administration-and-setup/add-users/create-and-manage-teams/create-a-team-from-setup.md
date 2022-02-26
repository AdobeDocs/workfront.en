---
filename: create-a-team-from-setup
title: Grant administrator access
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
title: Create a team from the Setup area
description: As an Adobe Workfront administrator, you can create a team from the Setup area. For information about teams, see Teams overview.
---

# Create a team from the Setup area

As an *Adobe Workfront administrator*, you can create a team from the Setup area. For information about teams, see [Teams overview](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* A *group administrator* can create a team for a group they administer from the Setup area. For more information, see [Create and modify a group’s teams](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>
>* A user with a *Plan* license can also create a team from the People area. For more information, see [Create a team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>

##  

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create a team

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Teams</span>, then click <span class="bold">New Team</span>.</li> 
 <li value="3"> <p>In the <b>New Team</b> box that displays, specify the following information:</p> 
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
     <td> <p>If you want to associate the team with a group, start typing the name of the group, then select the name when it appears.</p> <draft-comment>
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
    </tr> <draft-comment>
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">This is an Agile Team</td> 
      <td>Select this item if you want to configure this new team to be an agile team. For more information about agile teams, see <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Create an agile team</a>.</td> 
     </tr>
    </draft-comment>
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
     <td>Select the status that you want set for&nbsp;items when the Done button is clicked.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">Click&nbsp;<span class="bold">Create Team</span>.</li> 
</ol>

## Team owners

When you create a team you become the team owner, by default.

You can view team owners for all the teams when you create a report for teams and include the Owner Name field in your report. (For more information about creating a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
