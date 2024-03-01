---
title: Delete workspaces
description: You can delete workspaces when they are no longer relevant.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
---
<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Delete workspaces

{{maestro-important-intro}}

In Adobe Maestro, workspaces are centralized locations for teams to plan work. For more information, see [Create workspaces](../architecture/delete-workspaces.md). 

You can delete workspaces that are no longer relevant. 

We recommend recreating some or all of the record types and taxonomies associated with the workspace that you want to delete in another workspace before deleting it.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Maestro</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
    
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerations about deleting workspaces

* When you delete workspaces, all the record types, taxonomies, records, and their fields are also deleted. 
* Deleted workspaces and the information they contain cannot be recovered. 

## Delete a workspace

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available, then click **Maestro** ![](assets/maestro-icon.png).

    This opens the last workspace you accessed. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to delete. 
1. Click the **More** menu ![](assets/more-menu.png) next to the workspace name, then click **Delete**.
1. Click **Delete** to confirm.

    The workspace is deleted and cannot be recovered. Any record types, taxonomies, their records, and the fields associated with them are also deleted. <!--ensure this is right after closed beta-->
