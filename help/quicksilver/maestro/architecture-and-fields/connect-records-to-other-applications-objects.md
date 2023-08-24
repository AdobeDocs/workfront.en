---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
hidefromtoc: yes
hide: yes
---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Manage relationship fields" article-->

# Connect records and objects

You can connect Adobe Maestro records to one another or to objects from other applications. 

You must first connect two record types together or a record type to an object from another application, and then you can use the Table view of the record type to connect records to one another or records to other objects. 

You can connect the following: 

* Two Maestro operation record types to one another
* A Maestro operational record type to a taxonomy record type
* Two Maestro taxonomy record types together
* A Maestro record type and an object type from another application. 

  The following applications and object types are currently supported: 
  
  * From Adobe Workfront

    * Projects
    * Portfolios
    * Programs

  This article describes how you can connect a Maestro record with a Workfront object. Connecting two Maestro records to one another is similar.   <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->


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
   <td><p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td> <p>Any, to create Maestro records</p> 
<p>Work or higher to view projects in Workfront</p>
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td> <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level*</p></td>
   <td> <p>Any, to create Maestro records</p>
<p>View or higher access to Projects</p> 
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td> <p>View or higher permissions to the projects you want to link with Maestro records  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).


## Connect records overview

### Considerations about connecting records

* You can connect Maestro record types to one another or a Maestro record type with a Workfront object type by creating a new connection for a Maestro record type.
* After you connect a Maestro record type to another record type or to a Workfront object type, you can connect records to individual objects. 
* After the connection between the objects and records is established, the values of any of the linked fields from the linked records or from the Workfront objects populate in the Maestro record that you are linking from automatically. 
* You cannot update the values of linked fields manually on the records you are linking from. <!--LEFT HERE - August 24, 2023-->
* Everyone with access to Maestro can see the connections you make between Maestro records or between Maestro records and Workfront objects. Also, you can view and edit everyone else's connections. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
<!-- this is not possible yet; just projects for now: * You can connect one Maestro record to one or multiple Workfront objects. -->
* You cannot connect taxonomies to record types or to Workfront objects. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->

### Connect Maestro records


## Requirements for connecting Maestro records with Workfront objects

To link Maestro records with Workfront objects you must have the following:

* Workfront objects you want to link from Maestro. For example, projects, portfolios, or programs in Workfront.
* Maestro workspaces, record types, and records. For more information, see the following articles:

  * [Create workspaces](../architecture-and-fields/create-workspaces.md)
  * [Create record types](../architecture-and-fields/create-record-types.md)
  * [Create records](../records/create-records.md)

## Considerations about connecting objects from Workfront

<!-- this heading might need to be updated when more applications accessible??-->

* You can connect Workfront object types to Maestro record types in the same way you connect two Maestro record types, by creating a new connection for a Maestro record type and using Workfront object types as the Linked record type. 
* After you connect a Maestro record type with a Workfront object type, you can connect records to individual objects. Connecting records to objects automatically creates a Workfront record type in Maestro. This is a read-only record type which cannot be deleted. <!-- is this still accurate??-->  The Workfront objects connected to Maestro records are also read-only in Maestro and display on the Workfront record type page as read-only records.
* After the connection between the objects and records is established, the values of any of the linked fields from the Workfront objects populate in Maestro record fields automatically. 
* You cannot update the values of Workfront objects or their fields from Maestro. The synchronization of information is unilateral: only changes made in Workfront are automatically visible in Maestro.
* Everyone with access to Maestro can see the connections you make between Maestro records and Workfront objects. Also, you can see everyone else's connections. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* You can connect one Maestro record to one or multiple Workfront objects.
* You cannot connect a Workfront object to a Maestro record from Workfront. You can only connect records to objects from Maestro. 
* There is no indication in Workfront that an object is linked to Maestro records. Any changes made to the Maestro records do not reflect on the objects linked from Workfront. <!--this will change at some point; they'll probably add some indication in the Details section in WF, per Artur-->
* You cannot connect taxonomies to Workfront objects. You can only connect operational record types. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->

## Connect Workfront object types and fields to Maestro record types

You must connect Maestro record types with Workfront object types before you can connect individual records to objects. 

Connecting record types to object types from Workfront is similar to creating a Relationship-type field in Maestro. 

For information, see [Manage Relationship-type fields in Adobe Maestro](../architecture-and-fields/manage-relationship-fields.md). 

## Connect Workfront objects and fields to Maestro records

After you created a Relationship-type field between a Maestro record type and a Workfront object type, you can connect individual records to objects in Workfront. You can also connect fields from the Workfront object to the Maestro record type you linked to the object. 

1. Find the record type you created the linked record field for. 

    For information, see the section [Connect Workfront object types and fields to Maestro record types](#connect-workfront-object-types-and-fields-to-maestro-record-types) in this article. 
1. Select a Table view from the **View** drop-down menu in the upper-right corner of the record type page. 

1. From a record listed in the table view, go to the linked record column and hover over the cell corresponding to the record that you want to link with Workfront objects, then click the **+** icon. 

    The **Connect objects** box displays. 

    ![](assets/connect-objects-box-to-select-projects.png)

1. Start typing the name of a Workfront object in the search box, then select it when it displays in the list

    Or

    Select the name of one or multiple objects in the box, then click **Connect objects** in the upper-right corner of the Connect objects box. 

    The following are added to Maestro:

    * The selected Workfront objects are added to the linked record field. 
    * A new linked field (or a lookup field) is created for every linked field that you selected when adding the fields to your linked record. The linked field from the linked Workfront object type is named according to this pattern: 

      `<Name of the original field on the Workfront object type> (from <Name of your linked field>)`

      For example, if you linked the Budget field from Workfront projects and you named your relationship-type field "Linked Workfront project", the linked Budget field is named "Budget (From Linked Workfront project)".  
    * A new record type called "Workfront project" is created in the same workspace as the Maestro record you are linking from. 
    
        This is a read-only record type and it displays projects that are selected in the new relationship-type field you created from the Maestro record. The linked fields of the linked object also display on the read-only linked Workfront records.  
        
        Any existing information from the fields of the Workfront objects displays in the linked or lookup fields. 

        >[!TIP]
        >
        >*  We use "linked fields" and "lookup fields" interchangeably. 
        >
        >* If you enabled the Allow multiple records setting, the values of the multiple objects are either displayed separated by commas or are aggregated according to the aggregator you chose.
    
1. (Optional) Close the Maestro record type page and go to the Workspace you selected. Click the card for the Workfront object record type. For example, click the **Workfront project** card. The record type card should open in the Table view. 

    This is a read-only Workfront linked record type. 
    
    >[!NOTE]
    >
    >    * The records listed in the Workfront record type are read-only Workfront objects. The fields linked from the Maestro record type also display as  read-only columns. 
    >
    >    * To display the Workfront object record type in the Timeline view, you must have at least two date fields displayed in the Table view of the read-only Workfront record type page. 

1. (Optional) Click the **More** menu ![](assets/more-menu.png) next to the Workfront object record type name in the header of the page, then click **Rename** to edit the name of the record. 

    >[!NOTE]
    >
    >    You cannot delete a linked Workfront record type or any objects from the Workfront record type page. 

1. (Optional) Click the add fields icon ![](assets/add-fields-icon.png) in the upper-right corner of the table view on the Workfront record type page, to add or remove Workfront fields from the Workfront record type.

    >[!NOTE]
    >
    >  The fields you add or remove in the Workfront object record type page are not added nor removed from the Maestro record type that links to the Workfront object type. The fields are only visible on the read-only Workfront record type page, so you can review them in Maestro.
    
    
    
   
 



    


 
