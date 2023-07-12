---
title: Import records from Adobe Workfront
description: You can import record types from another application when you create a Relationship-type field linked to object fields from other applications. 
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Import records from Adobe Workfront


You can import record types from another application when you create a Relationship-type field linked to object fields from other applications. 

For example, you can create record types by creating a Relationship field on a Maestro record type linked to project fields in Workfront. As a result, the Workfront projects are imported into Maestro as a read-only record type. 
    
You can import the following objects from the following applications: 

* Projects from Workfront. This article describes how you can import Workfront projects in Maestro.  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->


## Access requirements

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
>*If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Requirements for connecting Maestro records with Workfront objects

To link Maestro records with Workfront objects you must have the following:

* Workfront objects you want to link from Maestro. For example, projects in Workfront.
* Maestro workspaces and record types. For more information, see the following articles:

  * [Create workspaces](create-workspaces.md)
  * [Create record types](create-record-types.md)

## Considerations about importing record types from Workfront

<!-- this heading might need to be updated when more applications accessible??-->

* You can import Workfront projects to Maestro by creating a Relationship-type field for a Maestro record and using Workfront projects as the Linked record type. This action connects the Maestro record type with the Workfront project object type. 
* A Workfront project record type is automatically created in Maestro and it is a read-only record type. The fields associated with the Workfront project record type are Workfront fields that display on the Details page of a project. 
* Everyone with access to Maestro can see the connections you make between Maestro records and Workfront objects. Also, you can see everyone else's connections. 
<!-- this is not possible yet; just projects for now: * You can connect one Maestro record to one or multiple Workfront objects. -->
* You can connect multiple Maestro records to the same Workfront project record type. 
* You cannot connect a Workfront object to a Maestro record from Workfront. You can only connect records to objects from Maestro. 
* Once the connection between the objects and records is established, the values of any of the linked fields from the Workfront objects populate in Maestro records automatically. 
* You cannot update Workfront objects or their field values from Maestro. The synchronization of information is unilateral: only changes made in Workfront are automatically visible in Maestro. 
* There is no indication in Workfront that an object is linked to Maestro records. Any changes made to the Maestro records do not reflect on the objects linked from Workfront. <!--this will change at some point; they'll probably add some indication in the Details section in WF, per Artur-->
* You cannot connect taxonomies to Workfront objects. You can only connect operational record types. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->

## Import record types from Workfront

Importing record types from Workfront is similar to creating a Relationship-type field in Maestro. For information, see [Manage Relationship-type fields in Adobe Maestro](../maestro/manage-relationship-fields.md)

1. Go to a record type whose records you want to connect to Workfront objects.
1. Select a **Table** view from the **View** drop-down menu in the upper-right corner of the record type page. 
1. Click the **+** icon in the upper-right corner of the table, to add a new field. 
1. Select **Relationship** from the **Field type** drop-down menu. You cannot change the field type after you save the field. 
1. Start typing a **Name** for the new field. 

   >[!TIP]
   >
   >We recommend that you include the name of the record you are linking to in the name of the relationship-type field to capture what record type the new field is coming from. The name of the linked record is not visible in the new linked field.
   >
   >For example, if you are linking the record to Workfront projects, you can name the new field "Linked Workfront project". 

1. (Optional) Add a description for this field. The description displays in the table view, when you hover over the column header of this field. 
1. Select **Workfront project** in the **Linked record type** field. This is a mandatory field and you cannot edit this selection after you save the field.  <!--check the names of the links here and the screen shot-->

    ![](assets/connector-to-workfront-projects-record-in-linked-record-type-field-drop-down.png)

1. Select **Allow multiple records** if you want to be able to link more than one Workfront object from one record. You cannot change this option after you save the field. 
1. (Optional) Select any of the fields available from the Workfront object. Standard and custom Workfront fields that display in the Project Details section in Workfront display in the list. If you don't select any fields, the **Name** field is selected by default, even when left unselected. 

1. (Conditional and optional) For date, number, currency, or percentage fields, select an aggregator from the drop-down to the right of the field name. For more information, see [Manage Relationship-type fields in Adobe Maestro](../maestro/manage-relationship-fields.md). 

    ![](assets/linked-field-aggregators-for-relationship-fields.png)

1. Click **Create**. <!-- is this the right button? I asked Lusine to replace with "add"-->

    The following are created:
    
    * The relationship-ype field is created with the new name you selected in step 5. <!--ensure this stays accurate-->
    
    >[!TIP]
    >
    >You can select the name of a Workfront object in the new relationship-type field you are creating. 

    * A new linked field is created for every linked field that you selected for the Workfront object type. The linked field from the linked Workfront object type is named according to this pattern: 

      `<Name of the original field on the Workfront object type> (from <Name of your linked field>)`

      For example, if you linked the Budget field from Workfront projects and you named your relationship-type field "Linked Workfront project", the linked Budget field is named "Budget (From Linked Workfront project)". 
    
    * A new record type called "Workfront project" is created in the workspace you selected. This is a read-only record type and it will display projects that are selected in the new relationship-type field.

1. (Optional) If you want to view which record type the linked fields come from, click the drop-down menu to the right of the relationship-type field, click **Edit field**, then view the name of the linked record type in the **Linked record type** field.  

    ![](assets/linked-record-type-from-workfront-grayed-out-highlighted.png)

1. (Optional) To connect records with objects, click the cell in the table of a Maestro record that contains the relationship-type field you created, then click the **+** icon to add Workfront objects.

    The **Connect objects** box displays. 
1. (Optional) Start typing the name of a Workfront objects in the search box, then select it when it displays on the screen

    Or

    Select the name of one or multiple projects in the box, then click **Connect objects** in the upper-right corner of the Connect objects box. 

    ![](assets/connect-objects-box-to-select-projects.png)

    The connected objects display in the relationship-type field you created. 

    ![](assets/connected-projects-highlighed-on-campaign-record-table.png)

1. (Conditional) If you selected to link more than one field from Workfront, additional columns display in the Maestro record table and the Workfront field values also display in their respective columns. If you did not select an aggregator for fields that have them available and you select more than one Workfront object, the field values display separated by commas. Otherwise, they display according to the selected aggregator. 



 
