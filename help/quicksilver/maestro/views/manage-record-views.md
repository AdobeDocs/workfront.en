---
title: Manage record views
description: You can display records in a table or a timeline view when using Adobe Maestro.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
---
# Manage record views

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

After selecting a record type in Adobe Maestro, you can display all the records of that type in the following views: 

* Table
    
    For more information, see [Manage the table view](../views/manage-the-table-view.md). 
* Timeline

    For more information, see [Manage the timeline view](../views/manage-the-timeline-view.md). 

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
   <td role="rowheader">Access level configuration</td>
   <td> <p>There are no access level controls for Maestro</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to the view</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Considerations when working with Maestro views

* Views in Maestro are record type-specific. You cannot apply the same view to two different record types. 
* Views that you create are visible only to you and users who you share the views with. 
* Building views for operational record types is identical to building views for taxonomy record types. 
* When you modify or delete a view, it is modified and deleted for all users who have permissions to the view. 
* The following elements are unique to each view in Maestro:

    * Filter
    * Grouping
    * Sort
    
    <!-- some of these are not available in all of the views - edit above-->

    For example, when creating a filter in a table view, the filter results are visible only in the view selected and not from all the views listed in the View drop-down menu. 

    >[!NOTE]
    >
    > Because Maestro is currently in a beta state, some view elements might not be available to both views.

This article describes the following information about Maestro views:

* [Create and edit a view](#create-or-edit-record-views) 
* [Delete a view](#delete-views)
<!--* [Duplicate a view](#duplicate-views)-->
<!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Share a view](#share-a-view)

## Similarities and differences between the table and timeline views

The following table shows the similarities and differences between the table and timeline views in Maestro: 

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Feature                                                               | Table view | Timeline view |
|-----------------------------------------------------------------------|------------|---------------|
| Display records in a list or table                                    | ✓          |              | 
| Display all fields as columns in the table, by default |     ✓       |              |
| Hide or show fields (or columns)       | ✓          |               |
| Edit field values for each record                           | ✓          |               |
| Add records as new rows in the view                                               | ✓          |               |
| Add fields as new columns in the view                                               | ✓          |               |
| Copy rows from an external list and paste them in a table             | ✓          |               |
| Display records in a timeline                                            |            | ✓             |
| Filter records                                       | ✓          | ✓             |
| Group records                                      |      ✓     | ✓             |
| Sort records                                       | ✓          |              |
| Color-code records                     |           | ✓              |
| Color-code groupings                     |           | ✓              |
| Search for specific records                     |  ✓         | ✓              |
| Share view                     |  ✓         | ✓              |
| Open the record's Details page from the view                    |  ✓         | ✓              |

## Create or edit views {#create-or-edit-views}

{{step1-to-maestro}} 
    
    
The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type card. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the selected type display in the table view. 

1. Click the **View** drop-down menu, and select either an existing **Table view** ![](assets/table-view-icon.png) or click **Create view > Table** to create a table view

    Or
    
    Select an existing **Timeline view** ![](assets/timeline-view-icon.png) view or click **Create view > Timeline** to create a timeline view.

    ![](assets/view-types-drop-down-from-record-type-list.png)

    >[!NOTE]
    >
    >    To create a timeline view, the record type you build the view for must have at least two date fields. Otherwise, the Timeline option is dimmed.

1. (Optional) Update the name of the view, then click **Create** to save it. 
    
    By default, Maestro names the view "Table < number >" or "Timeline < number >". The number is an automatically generated increment. 

1. (Optional) To rename a view after it is created, click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) > **Rename** to update the view name. <!--ensure there is not another saving step here?!-->
1. (Optional) To manage a specific type of view, see the following articles: 

    * [Manage the table view](../views/manage-the-table-view.md)
    * [Manage the timeline view](../views/manage-the-timeline-view.md)


## Delete views

{{step1-to-maestro}}

The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).

1. Click a record type card. 

    For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the selected type display in the table view. 

1. Click the view drop-down menu, hover over one of the views in the list, then click the **More** menu ![](assets/more-menu.png) > **Delete**. 
1. Click **Delete** to confirm. <!--ensure there is not another saving step here?!-->
    
    The view is deleted for all users who can access the Maestro area and it cannot be recovered. 

## Share a view

For information about sharing views, see [Share views](/help/quicksilver/maestro/access/share-views.md). 

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
