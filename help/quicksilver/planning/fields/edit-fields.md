---
title: Edit Field Settings
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created. This article describes how you can edit the settings for Workfront Planning fields.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
---

# Edit field settings

{{planning-important-intro}}

You can edit the field settings for fields that are already created in Adobe Workfront Planning. 

For information about creating Adobe Workfront Planning fields, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

This article describes how you can edit the settings for Workfront Planning fields. For information about editing field values for records, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

You must have the following to be able to access Workfront Planning:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--
OLD

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
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

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

## Edit field settings

{{step1-to-planning}}

1. Click the workspace whose record fields you want to edit.

    The workspace opens and all the record types in the workspace display on cards. 

1. Click the card of a record type. 

   This opens the record type's page. 

1. (Conditional) Click the tab of a **Table view**.

    All existing records associated with the record type display in the rows of the table view.
1. Hover over the column header of a field you want to edit, then click the downward-pointing arrow after the field name, then click **Edit field**

    Or 
    
    Double-click the column header for the field.

    ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)
    
1. Update information about the field and click **Save**. <!--insert screen shot when finalized-->

    >[!TIP]
    >
    >* You cannot update the field type after the field is saved.
    >
    >* When you modify field configurations (field options or formula expressions), records that already contain information in the modified fields will update their values in real-time. There is no warning and no audit log for the value changes triggered by field configuration changes. All users who view the fields will immediately see the new values with the modifications.

    The field information updates for everyone with access to view the workspace. 

1. (Conditional) For linked record fields, click **Edit lookup fields** and add or remove any of the fields from the linked record type.

    For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

