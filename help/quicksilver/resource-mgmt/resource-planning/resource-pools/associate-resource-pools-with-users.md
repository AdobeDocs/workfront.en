---
product-area: resource-management
navigation-topic: resource-pools
title: Associate Resource Pools with Users
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

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>New: Any</p>
       <p>or</p>
       <p>Current: Pro and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>or</p>
       <p>Current: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Resource Management that includes access to Manage Resource Pools</p> <p>Edit access to Projects, Templates, and Users</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td>Manage permissions for the projects, templates, and users that you want to associate the Resource Pools with</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Associate resource pools with one user

{{step-1-to-users}}

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

{{step-1-to-users}}

1. Select several users on the list, and click **Edit**.
1. Click **Resource Planning**.
1. Start typing the name of a resource pool that you want to associate with the users in the **Resource Pools** field, then select it from the list, when it appears.  
   You can associate multiple resource pools with multiple users.

   >[!NOTE]
   >
   >Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.

1. Click **Save Changes**.

For more information about how to edit users in bulk, see [Edit user profiles in bulk](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
