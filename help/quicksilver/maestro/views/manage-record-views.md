---
title: Manage record views
description: You can display records in a table, timeline, or calendar view when using the Adobe Workfront planning capabilities.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
---
# Manage record views

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

After selecting a record type in the Adobe Workfront planning capabilities area, you can display all the records of that type in the following views: 

* Table
    
    For more information, see [Manage the table view](../views/manage-the-table-view.md). 

* Timeline

    For more information, see [Manage the timeline view](../views/manage-the-timeline-view.md). 

* Calendar 

    For more information, see [Manage the calendar view](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

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
<p>Your organization must be enrolled in the Adobe Workfront planning capabilities closed beta program. Contact your account representative to inquire about this new offering. </p>
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
   <td> <p>There are no access level controls for Workfront planning capabilities</p>  
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

## Considerations when working with record views

* Views in the Workfront planning capabilities area are record type-specific. You cannot apply the same view to two different record types. 
* Views that you create are visible only to you and users who you share the views with. 
* Building views for operational record types is identical to building views for taxonomy record types. 
* When you modify or delete a view, it is modified and deleted for all users who have permissions to the view. 
* The following elements are unique to each record view:

    * Filter
    * Grouping
    * Sort
    
    <!-- some of these are not available in all of the views - edit above-->

    For example, when creating a filter in a table view, the filter results are visible only in the view selected and not from all the views listed in the View drop-down menu. 

    >[!NOTE]
    >
    > Because the Adobe Workfront planning capabilities are currently in a beta state, some view elements might not be available to all views.

This article describes the following information about record views:

* [Create and edit a view](#create-or-edit-record-views) 
* [Delete a view](#delete-views)
<!--* [Duplicate a view](#duplicate-views)-->
<!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Share a view](#share-a-view)

## Similarities and differences between record views

The following table shows the similarities and differences between the table, timeline, and calendar views: 

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Feature                                                               | Table view | Timeline view | Calendar view|
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Display records in a list or table                                    |    ✓          |              | |
| Display all fields as columns in the table, by default |     ✓       |              |    |
| Hide or show fields (or columns)       | ✓          |               |    |
| Edit field values for each record                           | ✓          |               |             |
| Add records as new rows in the view                                               | ✓          |               |        |
| Add fields as new columns in the view                                               | ✓          |               |         |
| Copy rows from an external list and paste them in a table             | ✓          |               |          |
| Display records in a timeline        |            |      ✓        |             | 
| Filter records            |     ✓     |✓             |           |
| Display records on a calendar                               |           |              |        ✓|
| Group records                                      |      ✓     | ✓             |
| Sort records                                       | ✓          |              |
| Color-code records                     |           | ✓              |          ✓     |
| Color-code groupings                     |           | ✓              |
| Search for specific records                     |  ✓         | ✓              |
| Share view                     |  ✓         | ✓              |       ✓     |
| Open the record's Details page from the view                    |  ✓         | ✓              |    |


## Create or edit views {#create-or-edit-views}

{{step1-to-maestro}} 
    
    
The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).

1. Click a record type card. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the selected type display in the table view. 

<!--
1. Click **+ View** to add a new view. 
1. Select from the following types of views: 

    * Table
    * Timeline
    * Calendar

    A new tab is created with the selected view. 

    Depending on the width of your screen, additional views might display in the **More** menu ![](assets/more-menu.png).   
-->

>[!TIP]
>
>When you create a record type, the table view is also created by default. 
>
>To create a timeline or a calendar view, the record type you build the view for must have at least two date fields. Otherwise, the Timeline and the Calendar options are dimmed.
>

1. Click the **View** drop-down menu, and select either an existing **Table view** ![](assets/table-view-icon.png) or click **Create view > Table** to create a table view

    Or
    
    Select an existing **Timeline view** ![](assets/timeline-view-icon.png) or click **Create view > Timeline** to create a timeline view.

    Or 

    Select an existing **Calendar view** ![](assets/calendar-view-icon.png) or click **Create View > Calendar** to create a calendar view. 

    ![](assets/view-types-drop-down-from-record-type-list.png)

    >[!NOTE]
    >
    >    To create a timeline or a calendar view, the record type you build the view for must have at least two date fields. Otherwise, the Timeline or the Calendar options are dimmed.

1. (Conditional) Click **Next**, when creating a timeline or calendar view.
    
    By default, Workfront gives the view one of the following names: 
    
    * `Table < number >`    
    * `Timeline < number >`
    * `Calendar < number >`
    
    The number is an automatically generated increment. 

1. (Conditional) Select the **Start** and **End dates** for the records that will display in the timeline or calendar view.
1. Click **Create**.

    <!--add for view redesign: The view displays as a new tab. Views display in the chronological order from when they were created or shared with you. -->
<!--1. (Optional) Click the **More** menu ![](assets/more-caret-down-icon-views.png) next to the last view to view all views for the selected record type. 

    Additional views display under the **More** menu after the last view tab. The number next to the **More** menu shows the number of additional views. -->
1. (Optional) To rename a view after it is created, click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) > **Rename** to update the view name. <!--ensure there is not another saving step here?!-->
<!--1. (Optional) To rename a view after it is created, double-click the view name and start typing the new name, or click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Rename**.-->
1. (Optional) To manage a specific type of view, see the following articles: 

    * [Manage the table view](../views/manage-the-table-view.md)
    * [Manage the timeline view](../views/manage-the-timeline-view.md)
    * [Manage the calendar view](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## Delete views

{{step1-to-maestro}}

The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).

1. Click a record type card. 

    For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the selected type display in the table view. 

<!--1. Hover over one the of the view's names in the view tab, then click **More** ![](assets/more-menu.png) to the left of the view name, then click **Delete**. (********delete the instructions in the point below but keep the last step***********)
First, you might need to click **More** to the left of the last tab to find the view you want to delete. -->

1. Click the view drop-down menu, hover over one of the views in the list, then click the **More** menu ![](assets/more-menu.png) > **Delete**. 
1. Click **Delete** to confirm. <!--ensure there is not another saving step here?!-->
    
    The view is deleted for all users who can access the records area and it cannot be recovered. 

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
