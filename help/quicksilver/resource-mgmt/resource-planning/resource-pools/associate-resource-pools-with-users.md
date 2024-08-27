---
product-area: resource-management
navigation-topic: resource-pools
title: Associate resource pools with users
description: You must create a resource pool before you can associate it with users. You can associate users with resource pools when you are creating your resource pools.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
---
# Associate resource pools with users

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Resource pools are collections of users what help you manage resources in Adobe Workfront.

You must create a resource pool before you can associate it with users.

You can associate users with resource pools when you are creating your resource pools.

If you create resource pools without populating them with users, you can later associate them with users as you are editing or creating new users.

For information about resource pools, see [Resource pools overview](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

For information about creating resource pools, see [Create resource pools](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Access requirements

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
   <td> <p>Edit access to&nbsp;Resource Management that includes access to Manage Resource Pools</p> <p>Edit access to Projects, Templates, and Users</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions for the projects, templates, and users you associate the resource pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Associate resource pools with one user

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Users**.  
1. Check the box next to the name of a user from the list, then click **Edit**.
1. Click **Resource Planning**.
1. Start typing the name of a resource pool that you want to associate with the user in the **Resource Pools** field, then select it from the list, when it appears.  
   You can associate multiple resource pools with one user.  
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)  

1. Click **Save Changes**.

For more information about editing users, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

For more information about creating new users, see [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associate resource pools with users in bulk

You can edit multiple users in bulk and associate the same resource pools with all of them at the same time.

To associate resource pools with several users in bulk:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Users**. 
1. Select several users on the list, and click **Edit**.
1. Click **Resource Planning**.
1. Start typing the name of a resource pool that you want to associate with the users in the **Resource Pools** field, then select it from the list, when it appears.  
   You can associate multiple resource pools with multiple users.

   >[!NOTE]
   >
   >Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.

1. Click **Save Changes**.

For more information about how to edit users in bulk, see [Edit user profiles in bulk](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
