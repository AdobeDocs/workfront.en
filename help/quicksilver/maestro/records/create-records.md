---
title: Create records
description: You must create record types before you can create individual records. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create records

In Adobe Maestro, a record is an instance of a record type. 

You can have the following type of records:

* **Operational records**: They represent work. For example, for an operational record called "Campaign", you can have named records like "Monthly Newsletter" or "Summer Sale."
* **Taxonomy records**: They represent attributes that can be associated with operational records. For example, for a taxonomy record type called "Channel", you can have named taxonomies like "Email", "Social Media", or "Advertising". 

Creating operational records is identical to creating taxonomy records, or taxonomies. 

You can create records in Maestro by doing one of the following:

* Manually create them for Maestro record types
* Import them from third-party applications after connecting Maestro records to objects from other applications. 

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
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Create records by manually adding them to a record type <!--in a record type table (I don't think you can create them elsewhere right now)-->

You can create records in the table view of a record type page. 

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->, then click **Maestro** ![](assets/maestro-icon.png). 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type card. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    The record type page opens in the view that you last accessed. By default, a record type page opens in the table view. 
    All the records of the type selected display in the table view. 

1. (Conditional) If the record type page does not open in the table view, click the **View** drop-down menu, and select either an existing **table view** ![](assets/table-view-icon.png) or click **Create view > Table** to create a table view. 

1. Click **New < Record type name >** in the last row of the table to add a new row to the table. 

    ![](assets/adding-a-new-campaign-in-table-row.png)

1. Start typing information in the new row about the new record. 

    >[!NOTE]
    >
    >  * The Name field is not a mandatory field. However, we recommend that you add a name for the record as it is helpful to identify records when linking records to one another. 
    >
    >  * Fields that refer to other record types or calculated fields are read-only fields. 

1. Continue adding information on each row, then click **Enter** on your keyboard to save your changes. 

## Create records by importing them from another application

You can import records from other applications into Maestro linked record types. 

1. Create a Maestro record type, as described in the [Create record types](../architecture-and-fields/create-record-types.md).

1. Create Maestro records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a Relationship-type field to a third-party application for the Maestro record type you created, as described in [Manage Relationship-type fields](../architecture-and-fields/manage-relationship-fields.md). 

1. Add records from the third-party application to the Maestro records you created above using the Relationship-type field you created in the previous step. For information, see [Connect records to objects from other applications](../architecture-and-fields/connect-records-to-other-applications-objects.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the third-party record type you linked to in the Relationship-type field. 

      For example, if you connect a Maestro record type to Workfront projects, a read-only record type named "Workfront projects" is created in the same workspace. 
    * Read-only records in the third-party record type page. The records imported from the third-party application remain read-only and can only be updated in their original application. 