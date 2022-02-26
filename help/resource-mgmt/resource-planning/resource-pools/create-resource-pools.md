---
filename: create-resource-pools
product-area: resource-management
navigation-topic: resource-pools
title: Create resource pools in Adobe Workfront
description: Resource pools are collections of users that help you manage resources easier in Adobe Workfront. For more information about resource pools, see Resource pools overview in Adobe Workfront.
---

# Create resource pools in *Adobe Workfront*

Resource pools are collections of users that help you manage resources easier in *Adobe Workfront*. For more information about resource pools, see [Resource pools overview in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Resource Management that includes access to Manage Resource Pools</p> <p>Edit access to Users</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create a Resource Pool

<ol> 
 <li value="1">Log in as a user who has access to edit Resource Pools.<br>For more information, see <a href="#access-to-edit-resource-pools" class="MCXref xref">Create a Resource Pool</a>.</li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li> 
 <li value="3"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Resourcing</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Resourcing</span>. 
  </MadCap:conditionalText></li> 
 <li value="4"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Resource Pools</span> in the left panel. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Resource Pools</span> in the left panel. 
  </MadCap:conditionalText><br><img src="assets/resource-pools-tab-350x198.png" alt="resource_pools_tab.png" style="width: 350;height: 198;"></li> 
 <li value="5">Click <span class="bold">New Resource Pool</span>.</li> 
 <li value="6">Specify the following: <p>
   <table cellspacing="0">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><span class="bold">Name</span></td>
      <td>This is the name of the Resource Pool.</td>
     </tr>
     <tr>
      <td role="rowheader"><span class="bold">Description</span></td>
      <td>This is a brief description about this Resource Pool. For example, you can specify for what purpose it should be used.</td>
     </tr>
     <tr>
      <td role="rowheader"><span class="bold">Pool Members</span></td>
      <td><p> Add users to the Resource Pool individually.<br>Or <br>To add a large amount of users to the Resource Pool at one time. You can add one of the following entities associated with users or collection of users:
        <ul>
         <li><span class="bold">Teams</span>: all members of the team are added to the Resource Pool.</li>
         <li><span class="bold">Groups</span>: all members of the group are added to the Resource Pool.</li>
         <li><span class="bold">Roles</span>: all users associated with that role are added to the Resource Pool.</li>
         <li><span class="bold">Companies</span>: all users in the company are added to the Resource Pool.</li>
        </ul><note type="tip">
         You can only add active users, teams, 
         <span>roles,</span> or companies.
        </note><note type="note">
          If a user becomes a member of a group, team, company or is associated with a job role after the group, team, company or job role have been added to the Resource Pool, the new member is not automatically added to the Resource Pool. 
         <br>If a user belongs to the team, group, company, and job role you are adding, at the same time, the user is added only once to the Resource Pool.
         <br>Users who are deactivated after having been added to the Resource Pool appear dimmed in the list of users and are marked as being deactivated.
        </note></p></td>
     </tr>
    </tbody>
   </table></p></li> 
 <li value="7"> <p>(Optional) Use the <span class="bold">Undo</span> link to remove the users added through a group, team, company or job role.</p> <note type="note">
    There is no limit to how many users you can have in a Resource Pool. However, we recommend not adding too many users to a Resource Pool, as Resource Management could become a challenge otherwise. The list of users only shows the first 2,000 users in the Resource Pool, and they are listed alphabetically. 
  </note> <p> <img src="assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png" alt="Resource_pools_NEW___UNDO_button_for_teams_groups_etc.png" style="width: 350;height: 113;"> </p> </li> 
 <li value="8">(Optional)&nbsp;Click the X icon to the right of a user's name to remove a user.&nbsp;For more information about removing users from a resource pool, see <a href="../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md" class="MCXref xref">Remove users from resource pools in&nbsp;Adobe Workfront</a>.</li> 
 <li value="9">(Optional) Use the <span class="bold">Search</span> option to find a user in the Resource Pool.</li> 
 <li value="10">Click <span class="bold">Create</span>.</li> 
</ol>

