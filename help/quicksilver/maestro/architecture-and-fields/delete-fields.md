---
title: Delete fields in Adobe Maestro
description: In Adobe Maestro, you can delete custom fields that are no longer relevant. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Delete fields in Adobe Maestro

In Adobe Maestro, you can create custom fields to store information about records. 

For information about creating Maestro records, see [Create Maestro fields](../architecture-and-fields/create-fields.md). 

You can delete Maestro fields that are no longer relevant. 

Consider the following when deleting Maestro fields:

* You can delete fields that you created or fields created by other users. <!--this will change with access levels/ permissions-->
* You can delete a field in the record type table. You cannot delete a field from the Details page of a record. 
* Any information stored in the field is deleted and cannot be recovered. 
<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->
* Deleted fields cannot be recovered. 

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

## Delete fields

<!--When they release the sharing of fields between other records, revise this section.  -->

1. Go to the record type you want to delete a field from. 
1. Find the field you want to delete in the column headers, and hover over the column header, then click the downward-pointing arrow after the field name. 
1. Click **Delete**. <!-- check this: they might replace it with **Delete field**-->

    ![](assets/field-menu-in-table.png)

1. Click **Delete** to confirm. 

    The field is deleted and can no longer be associated with any records. 