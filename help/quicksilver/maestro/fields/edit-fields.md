---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created. This article describes how you can edit the settings for Workfront Planning fields.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
---
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Edit fields 

{{maestro-important-intro}}

You can edit the field settings for fields that are already created in Adobe Workfront Planning. 

For information about creating Adobe Workfront Planning fields, see [Create fields](../fields/create-fields.md).

This article describes how you can edit the settings for Workfront Planning fields. For information about editing field values for records, see [Edit records](/help/quicksilver/maestro/records/edit-records.md).

## Considerations about editing field settings

You must consider the following before making changes to a field's configuration: 

* You can edit fields that you created or fields created by other users, if you have Manage permissions to the workspace that the fields belong to. 
* You can edit a field in the record type table. 
* You cannot edit a field on the record page or in any other view, outside of the table view. 
* You cannot edit the Field type, after the field is saved.
* You cannot deselect the Allow negative numbers setting that was previously selected, for a Number, Percentage, or Currency field if there are already negative values stored on the records it is attached to. 
* You can edit the configuration of the following field elements, after you save the field:

    * The Name or the Description of any field
    * The Options of a Single-select or a Multi-select field.
    * The expression of a Formula field.

    >[!WARNING]
    >
    >When formula expressions change, or options are added or removed from a select-type field, there will be loss of data for the records that already have information stored in the fields whose configuration is modified. 
    >
    >There is no warning or indication that this data loss could happen when you change the configuration of fields. 
    >
    >There is no notification to other users that the field configuration has changed.
    
<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

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
<p>Your organization must be enrolled in the Adobe Workfront Planning beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfront Planning</p>  
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
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Edit field settings

{{step1-to-maestro}}

    The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to delete record types for.  

    The workspace opens and the record types associated with it display. 
1. Click the card for the record type whose fields you want to edit.

    This opens the record type's page. 
1. (Conditional) Click the tab of a **Table view**.
1. Hover over the column header of a field you want to edit, then click the downward-pointing arrow after the field name, then click **Edit field**

    Or 
    
    Double-click the column header for the field.

    ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)
    
1. Update information about the field and click **Save**.

    <!--insert screen shot when finalized-->

    >[!TIP]
    >
    >You cannot update the field type after the field is saved.

    The field information updates for everyone with access to view the workspace. 

    <!--After the release of the RTBE for field configurations, replace the tip with this:

    >[!TIP]
    >
    >* You cannot update the field type after the field is saved.
    >
    >* When you modify field configurations (field options or formula expressions), records that already contain information in the modified fields will update their values in real-time. There is no warning and no audit log for the value changes triggered by field configuration changes. All users who view the fields will immediately see the new values with the modifications. 
    -->


1. (Conditional) For linked record fields, click **Edit lookup fields** and add or remove any of the fields from the linked record type.
  
    For more information, see [Connect record types](../architecture/connect-record-types.md). 
