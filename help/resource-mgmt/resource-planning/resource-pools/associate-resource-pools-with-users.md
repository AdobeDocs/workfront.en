---
filename: associate-resource-pools-with-users
product-area: resource-management
navigation-topic: resource-pools
title: Associate resource pools with users in Adobe Workfront
description: Resource pools are collections of users what help you manage resources in Adobe Workfront.
---

# Associate resource pools with users in *Adobe Workfront*

Resource pools are collections of users what help you manage resources in *Adobe Workfront*.

You must create a resource pool before you can associate it with users.

You can associate users with resource pools when you are creating your resource pools.

If you create resource pools without populating them with users, you can later associate them with users as you are editing or creating new users.

For information about resource pools, see [Resource pools overview in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

For information about creating resource pools, see [Create resource pools in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Edit access to&nbsp;Resource Management that includes access to Manage Resource Pools</p> <p>Edit access to Projects, Templates, and Users</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>Manage permissions for the projects, templates, and users you associate the resource pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions for the projects, templates, and users you associate the resource pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Associate resource pools with one user

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Users</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Users</span>. 
  </MadCap:conditionalText> </li> 
 <li value="3">Check the box next to the name of a user from the list, then click <span class="bold">Edit</span>.</li> 
 <li value="4">Click <span class="bold">Resource Planning</span>.</li> 
 <li value="5">Start typing the name of a resource pool that you want to associate with the user in the <span class="bold">Resource Pools</span> field, then select it from the list, when it appears.<br>You can associate multiple resource pools with one user.<br><img src="assets/add-resource-pool-to-user-350x307.png" alt="add_resource_pool_to_user.png" style="width: 350;height: 307;"><br></li> 
 <li value="6">Click <span class="bold">Save Changes</span>.</li> 
</ol>

For more information about editing users, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

For more information about creating new users, see [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associate resource pools with users in bulk

You can edit multiple users in bulk and associate the same resource pools with all of them at the same time.

To associate resource pools with several users in bulk:

<ol> 
 <li value="1"> Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Users</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Users</span>. 
  </MadCap:conditionalText></li> 
 <li value="3">Select several users on the list, and click <span class="bold">Edit</span>.</li> 
 <li value="4">Click <span class="bold">Resource Planning</span>.</li> 
 <li value="5">Start typing the name of a resource pool that you want to associate with the users in the <span class="bold">Resource Pools</span> field, then select it from the list, when it appears.<br>You can associate multiple resource pools with multiple users.<br><note type="note">
    Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.
  </note> <br><br></li> 
 <li value="6">Click <span class="bold">Save Changes</span>.</li> 
</ol>

For more information about how to edit users in bulk, see [Edit user profiles in bulk](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md). 
