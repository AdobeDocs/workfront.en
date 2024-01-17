---
title: Create records
description: In Adobe Maestro, a record is an instance of a record type. You must create record types before you can create individual records.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
---
<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Create records

>[!IMPORTANT]
>
>The information in this article refers to Adobe Maestro which is a new offering from Adobe Workfront. 
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. You must be a Workfront customer to use Maestro capabilities.
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro-overview.md).

In Adobe Maestro, a record is an instance of a record type. 

You can have the following types of records:

* **Operational records**: They represent work-related objects. For example, for an operational record called "Campaign", you can have named records like "Monthly Newsletter" or "Summer Sale."
* **Taxonomy records**: They represent attributes that can be associated with operational records. For example, for a taxonomy record type called "Channel", you can have named taxonomies like "Email", "Social Media", or "Advertising". 

Creating operational records is identical to creating taxonomy records, or taxonomies. 

You can create records in Maestro by doing one of the following:

* Manually create them for Maestro record types
* Connect them to Maestro records from third-party applications. 
* Create records by copying and pasting information from an external list. 

This article describes how you can create Maestro records. For information about managing records in the table or timeline views, see the following articles:

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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Maestro </p>  
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
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
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

{#step1-to-maestro}
  
  The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type card. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    The record type page opens in the view that you last accessed. By default, a record type page opens in the table view. 
    All the records of the selected type display in the table view. 

1. (Conditional) If the record type page does not open in the table view, click the **View** drop-down menu, and select either an existing **Table view** ![](assets/table-view-icon.png) or click **Create view > Table** to create a table view. 

1. To add new records, click **New < Record type name >** in the last row of the table 

    Or 

    Click **Shift + Enter** on your keyboard from any column or row of the table. This ads an empty row. 

    ![](assets/adding-a-new-campaign-in-table-row.png)

1. Start typing information in the new row about the new record. 

    >[!NOTE]
    >
    >  * There are no mandatory fields for records. However, we recommend that you add a Name for the record as it is helpful to identify records when linking records to one another. 
    >
    >  * Fields that refer to other record types or calculated fields are read-only fields. 

1. Continue adding information on each row, then click **Enter** on your keyboard to save your changes. 

1. (Optional) Use the following keyboard shortcuts to undo or redo adding new records: 

    * CTRL + Z (⌘ + Z for Mac) to undo a change 
    * CTRL + Shift + Z (⌘ + Shift + Z for Mac) to redo a change

## Create records by connecting them from another application

You can import records from other applications by linking them to Maestro linked records. This creates a Maestro record type for the third-party application connected object. Records you connect to the original Maestro records display in the third-party application connected object Maestro record type table view. 

1. Create a Maestro record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create Maestro records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from a third-party application for the Maestro record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add records from the third-party application to the Maestro records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the third-party record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront projects, a read-only record type named "Workfront projects" is created in the same workspace. 
    * Read-only records in the third-party record type page. The records imported from the third-party application remain read-only and can only be updated in their original application. 

## Create records by copying and pasting information from an external list

1. In Maestro, start creating records in the Table view, as described in the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

    Ensure that the Maestro table view has the columns (or the fields) that you want to populate with the new record information. 

1. Click **New < Record type name >** in the last row of the table to add as many new rows to the table as you want your new records to be. 

    For example, add 10 rows to the table view if you want to paste the information for 10 new records from another application. 

1. In another application, create a list of records that you want to import in Maestro. 
    
    For example, you can use an Excel spreadsheet to create your list. 

    The list should contain information in a tabular format.

    >[!TIP]
    >
    > The columns of the list should contain information for the existing fields you have in Maestro. 
    >
    > Ensure you have the desired fields already created in Maestro and that the information in your sheet displays in the correct format that matches that of each field in Maestro.

1. From the third-party application, select several rows and columns, then paste the information in the record type table view, starting with the first new record. 

    The following information is imported in Maestro:
    
    * The rows contain the new records
    * The columns populate information for the fields of the records.
