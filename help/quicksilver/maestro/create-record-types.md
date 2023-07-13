---
title: Create record types
description: You can create custom record types. Record types are Maestro objects. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->


# Create record types

Record types are the object types of Adobe Maestro. Record types can be one of the following:

* **Operational record types**: A record type that represents strategic plans, initiatives, or executed work. For example, Campaign, Activity, Tactic, Opportunity can be operational record types. 
* **Taxonomies**: Record types that capture attributes about an operational record type. For example, Region, Address, Audience can be taxonomies.  

For more information about Maestro record types, see [Overview of Adobe Maestro record types](../maestro/overview-of-record-types-and-taxonomies.md).

This article describes how to create operational record types. However, creating operational record types and taxonomies is identical. For more information about taxonomies, see [Create a taxonomy](../maestro/create-a-taxonomy.md).

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

>[!NOTE]
>
>*If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Considerations about record types 

<!--*********************************REVISE THIS - THE WORKFRONT CONNECTION IS NOT RIGHT HERE**************************-->

* Operational record types are the building blocks of workspaces in Maestro. The record types should reflect the work lifecycle of an organizational unit. For information about workspaces, see [Create workspaces](../maestro/create-workspaces.md).  
* When you create an operational record type, everyone in your organization can view, edit, or delete it. <!--this will change with access levels and permissions-->
* You can add operational record types to a workspace by doing one of the following:
    * Create them from scratch. This article describes how you can create a record type from scratch.
    * Import them from other systems by creating Relationship fields between Maestro record types and object types in other applications. 
    
        >[!TIP]
        >
        >    You cannot import taxonomy record types from other systems. <!--update this sentence when you can import taxonomies as well as operational records-->

* You must create a workspace before you can create record types for the workspace.  
* You can have a combined total of 1,000 operational record types and taxonomies in one workspace. This includes record types or taxonomies that you create from scratch or that you import from other systems. 

## Create a record type from scratch

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to create record types for.
1. Click **Add record type**. 
    
    The Add record type box opens. 

    ![](assets/add-record-type-box-with-appearance-options.png)

1. Select the following information:

    * **Record name**: Replace "Untitled Operational Record Type" with the name of your future record type. <!--correct this - I asked Garik to change this field to "Record type name"--> 
    * **Appearance**: Define the color and shape of the icon associated with the record type. Do the following: 
        * Select a color to identify your new record type. This is the color of the record type icon. Gray is selected by default.
        * Select an icon from the list, or start typing the name of an icon to describe what it represents, then select it when it displays. This is the icon of the record type. A file icon is selected by default. 

    ![](assets/operational-record-type-blank.png)

1. Click outside the **Add record type** box to save the record. 
1. (Optional) Click the name of a record type to open the Record type page. 

    The record type page displays in the Table view by default. The columns of the table are fields associated with the new record type. Each row is a unique record that you must add. 

    By default, the following fields display in the table view columns of an operational record type:

    * Name
    * Description
    * Start Date
    * End Date
    * Status

    By default, the following fields display in the table view columns of a taxonomy record type: 

    * Name

1. (Optional) Click the **+** icon in the upper-right corner of the table to add more fields to the record type. For more information, see [Create fields in Adobe Maestro](../maestro/create-fields.md).  

1. (Optional) Click the left-pointing arrow to the left of the record type name to go back to the selected workspace. 


For additional information about adding records, deleting record types, or updating the view in the record type page, see the following articles:

* [Create records](../maestro/create-records.md)
* [Delete record types and taxonomies](../maestro/delete-record-types-and-taxonomies.md)
* [Manage record views in Adobe Maestro](../maestro/manage-record-views.md) <!--add information here about the sorting and grouping when available-->

## Import record types from another application

You can import record types from another application when you create a Relationship-type field linked to object fields from other applications. 

For example, you can create record types by creating a Relationship field on a Maestro record type linked to project fields in Workfront. As a result, the Workfront projects are imported into Maestro as a read-only record type. 
    
You can import the following objects from the following applications: 

* Projects from Workfront. For more information, see [Import records from Workfront](../maestro/import-records-from-workfront.md). 



    




