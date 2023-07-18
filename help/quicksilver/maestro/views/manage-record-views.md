---
title: Manage record views
description: You can display records in a table or a timeline view when using Adobe Maestro. 
hidefromtoc: yes
hide: yes
---

# Manage record views

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

After selecting a record type in Adobe Maestro, you can display all the records of that type in the following views: 

* Table. For more information, see [Manage the table view](../views/manage-the-table-view.md). 
* Timeline. For more information, see [Manage the timeline view](../views/manage-the-timeline-view.md). 

Consider the following when working with Maestro views: 

* Views in Maestro are record type-specific. You cannot apply the same view to two different record types. 
* Views that you create are visible to everyone who accesses the Maestro area. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
<!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* Building views for operational record types is identical to building views for taxonomy record types. 
* When you modify or delete a view, it is modified and deleted for all users who can access the Maestro area. 

This article describes the following information about Maestro views:

* [Create and edit a view](#create-or-edit-record-views) 
<!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
<!--* [Share a view](#share-views) - not possible yet-->
* [Delete a view](#delete-views)

## Access requirements

You must have the following access to perform the steps in this article: 

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


## Similarities and differences between the table and timeline views

The following table shows the similarities and differences between the table and timeline views in Maestro: 

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Feature                                                               | Table view | Timeline view |
|-----------------------------------------------------------------------|------------|---------------|
| Display records in a list or table                                    | ✓          | ✓             |
| Display all record fields as columns, by default                      | ✓          |               |
| Display a limited number of fields (columns) in the table, by default |            | ✓             |
| Hide columns to limit the number of visible fields in the table       | ✓          |               |
| Edit fields for each record in the table                            | ✓          |               |
| Add records as new rows                                               | ✓          |               |
| Copy rows from an external list and paste them in a table             | ✓          |               |
| View records in a timeline                                            |            | ✓             |
| Filter, group, and sort records                                       | ✓          | ✓             |
| Sort groupings                                                        | ✓          | ✓             |

## Create or edit views {#create-or-edit-views}

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the **View** drop-down menu, and select either an existing **table view** ![](assets/table-view-icon.png) or click **Create view > Table** to create a table view

    Or
    
    Select an existing **timeline view** ![](assets/timeline-view-icon.png) or click **Create a view > Timeline** to create a timeline view.

    ![](assets/view-types-drop-down-from-record-type-list.png)

1. (Optional) Update the name of the view, then click **Create** to save it. 
    
    By default, Maestro names the view "Table < number >" or "Timeline < number >". The number is an automatically generated increment. 

1. (Optional) To rename a view, click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) > **Rename** to update the view name. <!--ensure there is not another saving step here?!-->
1. (Optional) To edit a view, see the following articles for more information: 

    * [Manage the table view](../views/manage-the-table-view.md)
    * [Manage the timeline view](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Delete views

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) > **Delete**, then **Delete**. <!--ensure there is not another saving step here?!-->
    
    The view is deleted for all users who can access the Maestro area. 


