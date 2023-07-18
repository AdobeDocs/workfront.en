---
title: Edit fields in Adobe Maestro
description: In Adobe Maestro, you can edit custom fields for each kind of operational record type or taxonomy. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Edit fields in Adobe Maestro

You can edit the field settings for fields that are already created. 

For information about creating Adobe Maestro fields, see [Create Mestro fields](../architecture-and-fields/create-fields.md). 

This article describes how you can edit the settings for Maestro fields. For information about editing field values for Maestro records, see [Edit records](../maestro/edit-records.md). 

Consider the following when editing fields: 

* You can edit fields that you created or fields created by other users. <!--this will change with access levels/ permissions-->
* You can edit a field in the record type table. You cannot edit a field from the Details page of a record. 
* You cannot edit the Field type, after the field is saved.
* You cannot edit the Record type of a Relationship field, after the field is saved.
* You cannot deselect the Allow negative numbers setting that was previously selected, for a Number, Percentage, or Currency field if there are already negative values stored on the records it is attached to. 
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Edit fields

1. Go to the record type you want to edit a field for. 
1. Find the field you want to edit in the column headers, hover over the column header, then click the downward-pointing arrow after the field name, and click **Edit field**.

  ![](assets/field-menu-in-table.png)

1. Update information about the field. 

    You cannot update the field type after the field is saved.

1. Click **Save**.