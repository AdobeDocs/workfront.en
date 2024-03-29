---
title: Create record types
description: Record types are the object types of Adobe Workfront planning. In Workfront planning, you can create custom record types which illustrate the work items needed in your organization's lifecycle.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
---
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Create record types

{{maestro-important-intro}}

Record types are the object types of Adobe Workfront planning. In Workfront planning, you can create custom record types which illustrate the work-related items needed in your organization's lifecycle. 
Record types can be one of the following:

For more information about record types, see [Overview of record types](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Workfront planning closed beta program. Contact your account representative to inquire about this new offering. </p>
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
   <p>Current: Plan</p>
   Or
   <p>New: Standard </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>--> 

## Considerations about creating record types 

* You can create record types in a workspace in the following ways:

    * Automatically: 
        * When you create a workspace using a template. 
        
            For information, see [Create workspaces](../architecture/create-workspaces.md).

        * When you import them using an Excel or CSV file. 

            >[!IMPORTANT]
            >
            >This functionality has been temporarily disabled since March 21, 2024. It will be enabled at a later date.

        <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
    * Manually:

        * From scratch.

            This article describes how you create generic record types from scratch in a workspace that you created from scratch.   

* You can move record types within a section and from one section of a workspace to another. You cannot move record types from one workspace to another workspace. 

## Create record types using a workspace template

You can create record types automatically when you create a workspace using a Workfront planning template. Each template contains sample record types. 

When you create a workspace from a template, the record types are grouped in the following sections:

* Operational record types
* Taxonomies

You can manually add record types in both the Operational Record Types and Taxonomies sections. 

For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).

For information about what record types are included with each template, see [List of workspace templates](../architecture/workspace-templates.md). 

## Create a record type from scratch

This article describes how to create record types from scratch.

{{step1-to-maestro}}

The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to create record types for.
1. Click **Add record type**. 
1. (Conditional) If you are creating an operational record type, click **From scratch**. 

    The Add record type box opens. 

    ![](assets/add-record-type-box-with-appearance-options.png)

1. Update the following information:

    * **Record type name**: Replace "Untitled Operational Record Type" with the name of your future record type. 
    * **Appearance**: Define the color and shape of the icon associated with the record type. Do the following: 
        * Select a color to identify your new record type. This is the color of the record type icon. Gray is selected by default.
        * Select an icon from the list, or start typing the name of an icon to describe what it represents, then select it when it displays. This is the icon of the record type. A file icon is selected by default. 

1. Click outside the **Add record type** box to save the record type. 

    The record type card is added to the workspace you selected. 
    The number of fields that the record type contains displays on the card. 
1. (Optional) Click the record type card to open the record type page. 

    ![](assets/operational-record-type-blank.png)

    The record type page displays in the Table view by default. The columns of the table are fields associated with the new record type. Each row is a unique record that you must add. 

    By default, the following fields display in the table view columns of an operational record type:

    * Name
    * Description
    * Start Date
    * End Date
    * Status

1. (Optional) Update the record type name in the header of the page

    Or

    Click the **More** icon ![](assets/more-menu.png) to the right of the record type name and click **Rename** to rename it. 

1. (Optional) Click **+ New record** to add records of the selected record type. For more information, see [Create records](../records/create-records.md). 
1. (Optional) Click the **+** icon in the upper-right corner of the table to add more fields to the record type. 

    For more information about creating fields, see [Create fields](../fields/create-fields.md).
    
1. (Optional) Click the left-pointing arrow to the left of the record type name to go back to the selected workspace. 

    The record type card displays the number of fields and connections the record type contains. 

    ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

    For additional information about adding records, deleting or editing record types, or updating the view in the record type page, see the following articles:

      * [Create records](../records/create-records.md)
      * [Delete record types](../architecture/delete-record-types.md)
      * [Edit record types](../architecture/edit-record-types.md)
      * [Manage record views](../views/manage-record-views.md) 

1. (Optional) From the workspace, click to drag and drop a record type in a desired spot, or to move it to another section. 

    The changes are saved automatically, after you dropped the selected record type card. 

## Create record types by importing an Excel or CSV file

>[!IMPORTANT]
>
>This functionality has been temporarily disabled since March 21, 2024. It will be enabled at a later date.


Consider the following when importing record types using an Excel or CSV file: 

* Each sheet of the Excel file becomes a record type. 
* The columns of each sheet become the fields associated with each record type. 
* Fields are unique for their respective record types. 
* Each row in each sheet becomes a unique record associated with its respective record type. 
* Each sheet of the Excel file should not exceed the following: 
    * 50,000 rows
    * 500 columns
* The Excel file should not be larger than 5MB.
* Empty sheets are not supported. 

To import record types using an Excel file: 

{{step1-to-maestro}}

The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to create record types for.
1. Click **Add record type**. 
1. Click **Excel/CSV**.
1. Drag and drop an Excel or CSV file previously saved on your computer, or click **Select a CSV or Excel file** to browse for one. 
1. Click **Review your data**.
    
    The Preview and edit box displays with the following information: 

    * The names of the sheets or of the future record types display in the left panel. Workfront planning selects an icon and a color for each new record type by default.
    * The first sheet or record type is selected and the names of the fields associated with it display as the column headers. The type of each field is selected by default. 
    * Each row represents a new record. Only the first 10 records display in the Preview and edit box. 

    ![](assets/preview-and-edit-box.png)

1. (Optional) Click the name of each sheet in the left panel to review the information it contains. 

    >[!NOTE]
    >
    >    Sheets that are empty are not supported and are dimmed. 


1. (Optional) Click the **Select sheets to import** drop-down menu and deselect the sheets that you don't want to import. 

    ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

    Sheets you deselected display with a gray background. 

1. Click **Import** when you are ready to import your file. 

    The following information imports in to Workfront planning:

    * New record types
    * New fields associated with each record type
    * New records associated with each record type

    You can start managing fields and records on the record types pages. 
    
    Everyone with access to Workfront planning can now view and edit the imported record types and their information. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->