---
product-area: resource-management
navigation-topic: resource-pools
title: Create resource pools
description: Resource pools are collections of users that help you manage resources easier in Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
---
# Create resource pools

{{highlighted-preview}}

Resource pools are collections of users that help you manage resources easier in Adobe Workfront. For more information about resource pools, see [Resource pools overview](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Resource Management that includes access to Manage Resource Pools</p> <p>Edit access to Users, Projects, and Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions for the projects and templates that you want to associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Create a Resource Pool {#create-a-resource-pool}

{{step1-to-resourcing}}

1. Click **Resource Pools** in the left panel.   
   
   <span class="preview">Sample image in the Preview environment:</span>
   <span class="preview">![Resource Pools](assets/list-of-resource-pools.png)</span>

   Sample image in the Production environment:
   ![Resource Pools](assets/resource-pools-tab-350x198.png)

1. Click **New Resource Pool**.
1. Specify the following:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Name</strong></td>
      <td>This is the name of the Resource Pool.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Description</strong></td>
      <td>This is a brief description about this Resource Pool. For example, you can specify for what purpose it should be used.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Pool Members</strong></td>
      <td><p> Add users to the Resource Pool individually.<br>Or <br>To add a large amount of users to the Resource Pool at one time. You can add one of the following entities associated with users or collection of users:
        <ul>
         <li><strong>Teams</strong>: all members of the team are added to the Resource Pool.</li>
         <li><strong>Groups</strong>: all members of the group are added to the Resource Pool.</li>
         <li><strong>Roles</strong>: all users associated with that role are added to the Resource Pool.</li>
         <li><strong>Companies</strong>: all users in the company are added to the Resource Pool.</li>
        </ul><p>Tip: You can only add active users, teams, <span>roles,</span> or companies.</p><br>You might need to scroll down in the dialog to see all of the users in the Resource Pool.
        <p>Note:  If a user becomes a member of a group, team, company or is associated with a job role after the group, team, company or job role have been added to the Resource Pool, the new member is not automatically added to the Resource Pool. <br>If a user belongs to the team, group, company, and job role you are adding, at the same time, the user is added only once to the Resource Pool.<br>Users who are deactivated after having been added to the Resource Pool appear dimmed in the list of users and are marked as being deactivated.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Optional) Use the **Undo** link to remove the users added through a group, team, company or job role.

   >[!NOTE]
   >
   >There is no limit to how many users you can have in a Resource Pool. However, we recommend not adding too many users to a Resource Pool, as Resource Management could become a challenge otherwise. The list of users only shows the first 2,000 users in the Resource Pool, and they are listed alphabetically.

   <span class="preview">Sample image in the Preview environment:</span>
   <span class="preview">![Users added to Resource Pool](assets/users-in-resource-pool2.png)</span>

   Sample image in the Production environment:
   ![Users added to Resource Pool](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Optional) Click the X icon to the right of a user's name to remove a user. For more information about removing users from a resource pool, see [Remove users from resource pools](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Optional) Use the **Search** option to find a user in the Resource Pool.
1. Click **Create**.
