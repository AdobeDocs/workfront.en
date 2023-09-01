---
title: Delete workspaces
description: You can delete workspaces when they are no longer relevant. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Delete workspaces

In Adobe Maestro, workspaces are centralized locations for teams to plan work. For more information, see [Create workspaces](../architecture-and-fields/create-workspaces.md). 

You can delete workspaces that are no longer relevant. 

We recommend recreating some or all of the record types and taxonomies associated with the workspace that you want to delete in another workspace before deleting it.

## Access requirements

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Considerations about deleting workspaces

* You can delete any workspace that either you or anyone in your organizaton has created. <!--this will change with access levels and permissions-->
* When you delete workspaces, all the record types, taxonomies, and their fields are also deleted. <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* Deleted workspaces and the information they contain cannot be recovered. 

## Delete a workspace

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    This opens the last workspace you accessed. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to delete. 
1. Click the **More** menu ![](assets/more-menu.png) next to the workspace name, then click **Delete**.
1. Click **Delete** to confirm.

    The workspace is deleted and cannot be recovered. Any record types, taxonomies, their records and the fields associated with them are also deleted. <!--ensure this is right after closed beta-->
