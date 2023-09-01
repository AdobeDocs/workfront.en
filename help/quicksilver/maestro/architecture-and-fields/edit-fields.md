---
title: Edit fields
description: In Adobe Maestro, you can edit the field settings for fields that are already created. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Edit fields 

You can edit the field settings for fields that are already created. 

For information about creating Adobe Maestro fields, see [Create fields](../architecture-and-fields/create-fields.md). 

This article describes how you can edit the settings for Maestro fields. For information about editing field values for Maestro records, see [Edit records](../maestro/edit-records.md). 

## Considerations about editing field information

* You can edit fields that you created or fields created by other users. <!--this will change with access levels/ permissions-->
* You can edit a field in the record type table. 
* You cannot edit the Field type, after the field is saved.
* You cannot deselect the Allow negative numbers setting that was previously selected, for a Number, Percentage, or Currency field if there are already negative values stored on the records it is attached to. 
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

## Access requirements

You must have the following to perform the steps described in this article: 

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

*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Edit fields

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to delete record types for.  

    The workspace opens and the record types and taxonomies associated with it display. 
1. Click the card for the record type or the taxonomy whose fields you want to edit.

    This opens the record type's page. 
1. (Conditional) Select a **Table view** from the **View** drop-down menu in the upper-right corner of the record type page.
1. Hover over the column header of a field you want to edit, then click the downward-pointing arrow after the field name.
1. Click **Edit field**, then update information about the field and click **Save**.

    <!--insert screen shot when finalized-->

    >[!TIP]
    >
    >You cannot update the field type after the field is saved.


1. (Conditional) For linked record fields, click **Edit lookup fields** and add or remove any of the fields from the linked record type.
  
    For more information, see [Connect record types](../architecture-and-fields/connect-record-types.md). 
