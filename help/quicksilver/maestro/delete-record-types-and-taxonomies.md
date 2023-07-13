---
title: Delete record types
description: You can delete record types or taxonomies when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Delete record types and taxonomies

You can delete record types or taxonomies when they are no longer relevant. 

For information about record types and taxonomies, see [Overview of Adobe Maestro record types](../maestro/overview-of-record-types-and-taxonomies.md).

We recommend recreating the fields and the records associated with the record type or taxonomy that you want to delete on another record type before deleting them.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Access requirements

You must have the following access to perform the steps in this article:

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
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Considerations when deleting record types

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* You can delete any record type or taxonomy that either you or anyone in your organizaton has created. <!--this will change with access levels and permissions-->
* Deleting record types deletes all the information associated with them, including fields and records of that type. 
* You cannot recover deleted record types or their information. 

## Delete record types and taxonomies

Deleting taxonomies is identical to deleting record types. 

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to delete record types for.  

    The workspace opens and the record types and taxonomies associated with it display. 
1. Click the record type or the taxonomy that you want to delete. 
1. Click the **More** menu ![](assets/more-menu.png) to the right of the record type name, then click **Delete**. 
1. Click **Delete** to confirm. 

    The selected record type or taxonomy, along with their fields and associated records are deleted. 