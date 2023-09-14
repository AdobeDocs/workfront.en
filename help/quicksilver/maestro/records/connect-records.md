---
title: Connect records
description: After you create connections between record types, you can connect individual records to one another. 
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
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connect records 

>[!IMPORTANT]
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. 
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro-overview.md).

You can connect Adobe Maestro records to one another or to objects from other applications. 

You must first connect two record types together or a record type to an object type from another application, and then you can use the Table view of the record type to connect records to one another or records to other objects. 

For information about connecting record types to one another or to object types from other applications, see [Connect record types](../architecture-and-fields/connect-record-types.md).

For an example of connecting record types, see [Example of connecting record types and records](../architecture-and-fields/example-connect-record-types-and-records.md).

You can connect the following: 

* Maestro operational records 
* Maestro operational records to taxonomy records
* Maestro operational records and objects from other applications. 

  The following applications and object types are currently supported: 
  
  * Adobe Workfront

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto">
 <col>
<tbody>
<td>
   <p> Adobe product</p> </td>
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
   <td><p>Any, to create Maestro records</p> 
<p>Work or higher to view projects in Workfront</p>
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Adobe Workfront licenses overview</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any, to create Maestro records</p>
<p>View or higher access to Projects, Portfolios, Programs</p> 
<p>Additional access to Groups and Companies, when viewing groups or companies users don't belong to</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td> <p>View or higher permissions to the objects you want to link with Maestro records  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p></td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>--> 

## Connect records

### Considerations about connecting records

* After the connection between record types is established, the connected record types display as linked record fields in the table of the record types they are linked from. 
* You can browse and add records and objects of the linked record and object types from the linked record fields. 
* You can add fields from the linked record types to the table of the record type you are linking from. 
* You cannot manually update the values of linked fields on the records you are linking from. 

  The values of the linked fields from the linked records populate the Maestro record that you are linking from automatically. 

* Everyone with access to Maestro can see the connections that you make between Maestro records or between Maestro records and Workfront objects. Also, you can view and edit everyone else's connections. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* You can connect one Maestro record to one or multiple objects from another application.
* You cannot connect taxonomies to record types or to objects from another application. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Currently, you can link Maestro records only to Workfront objects. To link Maestro records with Workfront objects, you must have the following:

  * Workfront objects. For example, you must first create projects, portfolios, programs, companies, or groups in Workfront.
  * Maestro workspaces, record types, and records. For more information, see the following articles:

    * [Create workspaces](../architecture-and-fields/create-workspaces.md)
    * [Create record types](../architecture-and-fields/create-record-types.md)
    * [Create records](../records/create-records.md)

  * Connections between record types, or between record types and objects from other applications. For information, see [Connect record types](../architecture-and-fields/connect-record-types.md). 
  
### Connect Maestro records

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to connect records from.
1. Click the card of a record type to open the record type page. 
1. Select a Table view from the **View** drop-down menu in the upper-right corner of the record type page. 
1. Add a connection to another record or object type from the selected record type. For information, see [Connect record types](../architecture-and-fields/connect-record-types.md). 

  A new column is added to the table to display the linked record type. 

1. Add records to the record type that you selected by adding a new row to the table. For information, see [Create records](../../maestro/records/create-records.md). 
1. From a record listed in the table view, go to the linked record column and hover over the cell corresponding to the record that you want to link with other Maestro records, then click the **+** icon. 

    The **Connect objects** box displays. 

    ![](assets/connected-objects-table-for-records.png)

1. Start typing the name of a record in the search box, then select it when it displays in the list

    Or

    Select the name of one or multiple records in the box, then click **Connect objects** in the upper-right corner of the Connect objects box. 

    The following are added:

    * The linked records display in the linked record field of the record that you selected in step 3. Updating the linked records automatically updates the linked record fields for the records that you are linking from. <!--ensure the number of the step stays accurate--> 
    * The linked fields that belong to the linked records are automatically populated with the information from the original linked records. You cannot manually edit linked fields. 
        
        >[!TIP]
        >
        >*  We use "linked fields" and "lookup fields" interchangeably. 
        >
        >* If you enabled the Allow multiple records setting when you connected the record types, the values of fields for the multiple selected objects are either displayed separated by commas or are aggregated according to the aggregator you chose.
    
1. (Optional) Close the Maestro record type page and go to the Workspace you selected. 
1. Click the card for the record type that you linked to. 

    For example, if you connected the Campaign record with the Product record, click the **Product** card. 
  
    The record type card should open in the Table view. 
  
    Notice that the Campaign linked record field displays the names of the campaigns you linked to products in the Product record type page. Updating the Campaign information automatically updates the Campaign linked record field for the Product record type. 

### Connect Maestro records to Workfront objects

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

After you created a connection between a Maestro record type and a Workfront object type, you can connect individual Maestro records to objects in Workfront. You can also connect fields from the Workfront object to the Maestro record type. 

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to connect records from.
1. Click the card of a record type to open the record type page. 
1. Select a Table view from the **View** drop-down menu in the upper-right corner of the record type page. 
1. Add a new connection to an object type from Workfront the selected record type. Select from the following objects under the Workfront section: 

    * Project
    * Portfolio
    * Program
    * Company
    * Group

    For more information, see [Connect record types](../architecture-and-fields/connect-record-types.md).

    A new column is added to the table to display the linked object type. 

1. Add individual records to the record type that you selected by adding a new row to the table. For information, see [Create records](../../maestro/records/create-records.md). 
1. From a record listed in the table view, go to the linked object column and hover over the cell corresponding to the record that you want to link with other objects from Workfront, then click the **+** icon. <!--change Workfront to other applications, when this will be possible-->

    The **Connect objects** box displays. 

    ![](assets/connect-objects-box-to-select-projects.png)

1. Start typing the name of a Workfront object in the search box, then select it when it displays in the list

    Or

    Select the name of one or multiple objects in the box, then click **Connect objects** in the upper-right corner of the Connect objects box. 

    The following are added to Maestro:

    * The selected Workfront objects are added to the linked record field. 
    * A new linked field (or a lookup field) is created for every linked field that you selected when adding the fields to your linked record.  
    * A new record type called "Workfront object" is created in the same workspace as the Maestro record you are linking from. The name of the object is part of this record type's name. For example, linking to Workfront projects creates the Workfront project record type in Maestro. 

      This is a read-only record type and it displays Workfront objects that are selected in the new linked object field you created from the Maestro record. The linked fields of the linked object also display on the read-only linked Workfront records.

      >[!IMPORTANT]
      >
      > The read-only Workfront object record type is created only when individual projects are added to Maestro records. Simply creating a connection between a Maestro record type and a Workfront object type does not create the Workfront record type. 

       Any existing information from the fields of the Workfront objects displays in the linked or lookup fields. 

        >[!TIP]
        >
        >
        >* If you enabled the Allow multiple records setting, the values of the multiple objects are either displayed separated by commas or are aggregated according to the aggregator you chose.
        >
        >* A linked record field to the Maestro linked records is not created for the linked Workfront objects. 
      
    
1. (Optional) Close the Maestro record type page and go to the Workspace you selected. 
1. Click the card for the Workfront object record type. For example, click the **Workfront project** card, if you linked to Workfront projects. The read-only Workfront record type card should open in the Table view. 

    >[!NOTE]
    >
    >    * The records listed in the Workfront record type page are read-only Workfront objects. The fields linked from the Workfront record type also display as read-only columns and they are populated automatically when they are populated in Workfront.
    >    * You cannot manually update Workfront fields in Maestro. Workfront object fields must be populated in Workfront and the field values display automatically on the Workfront record in Maestro.  
    >
    >    * To display the Workfront object record type in the Timeline view, you must have at least two date fields displayed in the Table view of the read-only Workfront record type page. 

1. (Optional) Click the **More** menu ![](assets/more-menu.png) next to the Workfront object record type name in the header of the page, then click **Rename** to edit the name of the record. 

    >[!NOTE]
    >
    >    You cannot delete a linked Workfront record type or any objects from the Workfront record type page. 

1. (Optional) Click the **Add fields** icon ![](assets/add-fields-icon.png) in the upper-right corner of the table view on the Workfront record type page, to add or remove Workfront fields from the Workfront record type.

    >[!NOTE]
    >
    >  The fields you add or remove in the Workfront object record type page are not added nor removed from the Maestro record type that links to the Workfront object type. The fields are only visible on the read-only Workfront record type page, so you can review them in Maestro.

1. (Optional) From the View drop-down menu on the Workfront object record type page, choose the Timeline view to display the Workfront linked objects in the timeline view. 
    
    
    
   
 



    


 
