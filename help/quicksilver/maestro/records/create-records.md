---
title: Create records
description: When using Adobe Workfront Planning, a record is an instance of a record type. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
---
<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Create records

{{planning-important-intro}}

In Adobe Workfront Planning, a record is an instance of a record type. 

You can create records by doing one of the following:

* Manually create them for record types
* Create records by copying and pasting information from an external list. 

This article describes how you can create records. For information about managing records in the table or timeline views, see the following articles:

* [Manage the table view](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Manage the timeline view](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
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

## Create records by manually adding them to a record type <!--in a record type table (I don't think you can create them elsewhere right now)-->

You can create records in the table view of a record type page. 

For information about editing record information, see [Edit records](/help/quicksilver/maestro/records/edit-records.md). 

{#step1-to-maestro}
  
  The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).

1. Click a record type card. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    The record type page opens in the view that you last accessed. By default, a record type page opens in the table view. 
    All the records of the selected type display in the view. 

1. (Conditional) Depending on which view you display, do one of the following: 

    * From the table view: 

        * Click **New record** in the last row of the table 

        * Click **Shift + Enter** on your keyboard from any column or row of the table. This ads an empty row. 

        ![](assets/adding-a-new-campaign-in-table-row.png)

    * From any view: 
    
        * Click **New record** in the upper-right corner of the page. The record preview box opens. 

1. Start typing information in the new row about the new record, or in the fields you see in the preview box. 

    >[!NOTE]
    >
    >  * There are no mandatory fields for records. However, we recommend that you add a Name for the record as it is helpful to identify records by their name when linking records to one another. 
    >
    >  * Fields that refer to other record types or calculated fields are read-only fields. 

1. (Conditional) When adding records in the table, continue adding information on each row, then click **Enter** on your keyboard to save your changes.

    Or 
    
    Click the new record's name or the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of the record name. A preview with the record's detailed information opens in the table. 

    >[!TIP]
    >
    >You can access the **Open Details** icon only from the name field of the record when the Name field is a primary field. 

1. Start editing the record's information in the record's preview. Workfront automatically saves your changes. 
1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the record's preview to open the record's page in a new tab. Continue editing the record on the record page.

1. (Optional) Use the following keyboard shortcuts to undo or redo adding new records or their information, when adding them in the table view: 

    * CTRL + Z (⌘ + Z for Mac) to undo a change 
    * CTRL + Shift + Z (⌘ + Shift + Z for Mac) to redo a change

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## Create records by copying and pasting information from an external list

1. Start creating records in the Table view, as described in the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

    Ensure that the table view has the columns (or the fields) that you want to populate with the new record information. 

1. Click **New < Record type name >** in the last row of the table to add as many new rows to the table as you want your new records to be. 

    For example, add 10 rows to the table view if you want to paste the information for 10 new records from another application. 

1. In another application, create a list of records that you want to import. 
    
    For example, you can use an Excel spreadsheet to create your list. 

    The list should contain information in a tabular format.

    >[!TIP]
    >
    > The columns of the list should contain information for the existing fields you have in Workfront. 
    >
    > Ensure you have the desired fields already created in Workfront and that the information in your sheet displays in the correct format that matches that of each field in Workfront.

1. From another application, select several rows and columns, then paste the information in the record type table view, starting with the first new record. 

    The following information is imported in the Workfront Planning area:
    
    * The rows contain the new records
    * The columns populate information for the fields of the records.
