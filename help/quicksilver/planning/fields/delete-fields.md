---
title: Delete fields
description: In Adobe Workfront Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
---
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Delete fields

{{planning-important-intro}}

In Adobe Workfront Planning, you can create custom fields to store information about records. 

For information about creating custom fields in Workfront Planning, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

You can delete Workfront Planning fields that are no longer relevant. 

## Considerations about deleting Workfront Planning fields:

* You can delete a field only in the record type table view.
* You cannot delete the primary field of a record. 
* Any information stored in the field is deleted and cannot be recovered. 
* When you delete a linked record field, all the linked lookup fields are also deleted from the record type you link from. The linked record fields of the record types you link to are not deleted. 

   For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

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
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
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
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Delete fields

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}
    
1. Click the workspace whose record fields you want to delete. 

    The workspace opens and the record types display. 

1. Click the card of a record type. 

1. (Conditional) If not already selected, click the tab of a **Table view** on the record type page. 

     All existing records associated with the record type display in the rows of the table view.
     
1. Find the field that you want to delete in the column headers, and hover over the column header, then click the downward-pointing arrow after the field name. 

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)
   
1. Click **Delete**. <!-- check this: they might replace it with **Delete field**-->

    <!--insert screen shot when finalized-->

1. Click **Delete** to confirm. 

    The field is deleted, cannot be recovered, and can no longer be associated with any records.
