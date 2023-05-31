---
title: Manage record views in Adobe Maestro
description: You can display records in a table or a timeline view when using Adobe Maestro. 
hidefromtoc: yes
hide: yes
---

# Manage record views in Adobe Maestro

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

After selecting a record type in Adobe Maestro, you can display all the records of that type in the following views: 

* Table
* Timeline

Consider the following when working with Maestro views: 

* Views in Maestro are record type-specific. You cannot apply the same view to two different record types. 
* Views that you create are only visible to you. <!-- this is not yet possible: You can share views with others if you want them to also apply them to the same record types.-->
* Building views for operational record types is identical to building views for taxonomical record types. 

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

## Create or edit record views {#create-or-edit-record-views}

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../maestro/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create operational record types](../maestro/create-operational-record-types.md).

    By default, all the records of the type selected display in the table view. 

1. Click the **View** drop-down menu, and select either an existing **table view** ![](assets/table-view-icon.png) or click **Create view > Table** to create a table view

    Or
    
    Select an existing **timeline view** ![](assets/timeline-view-icon.png) or click **Create a view > Timeline** to create a timeline view.

1. (Optional) Give the new view a name, then click **Create** to save it. 
    
    By default, Maestro names the view "Table < number >" or "Timeline < number >". The number is an automatically generated increment. 
1. (Conditional) When building a table view, follow the steps in [Manage the table view](#manage-the-table-view)

1. (Conditional) When building a timeline view, follow the steps in [Manage the timeline view](#manage-the-timeline-view).

1. (Optional) Click the name of a view in the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) > **Edit** to update the view name. <!--ensure there is not another saving step here?!-->


## Manage the table view {#manage-the-table-view}

<!--insert screen shot of table view-->

When creating a table view, all records of the selected record type display in a table. Each row is a unique record and each column is a record field. All fields and all records display by default. 

To manage a table view: 

1. Create a table view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. Update the following view elements as described in the subsections below:
    * [Columns](#add-columns)
    * [Rows](#add-rows)
    * [Filters](#add-filters) 
    * [Grouping](#add-groupings)
    * [Sort](#sort-information)  


### Add columns {#add-columns}

The column headers of a Maestro table view display fields associated with the records in the view. The same fields displayed in the table view also display in the Details section of a Maestro record. For more information, see [Edit records](../maestro/edit-records.md).

You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the timeline view is limited and you cannot add columns in addition to those selected by default. <!--ensure that there is a table for the timeline view - right not there is not, but they are working to add a table to the left of the timeline-->

You must create fields before you can display them in a view. 

You can add up to 500 fields (or columns) in a table view. Adding columns to a table view is identical to adding fields. For information, see [Create Maestro fields](../maestro/create-fields.md). 

### Add rows {#add-rows}

The rows of a Maestro table view display individual records of the selected record type. 

You can add up to 10,000 records (or rows) to a table in Maestro. 
Adding rows to a Maestro table view is identical to creating records in a table. For information, see [Create records](../maestro/create-records.md). 

### Add filters {#add-filters}

Filters help you reduce the amount of information displayed on the screen.

You can apply filters to both the table and timeline views. 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. Select a table or a timeline view, then click **Filters**.    
1. Start typing a field in the **Select a field** box, then click it when it appears in the list. This is the field that you want to filter by. 
1. Select one of available modifiers from the **Select an option** drop-down menu. 


    The following table lists the available modifiers for each type of field:

    <table>
    <thead>
    <tr>
        <th><b>Field type</b></th>
        <th><b>Modifiers</b></th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>Single-line, paragraph </td>
        <td><p>Contains</p>
        <p>Does not contain</p>
        <p>Is</p>
        <p>Is not</p>
        <p>Is empty</p>
        <p>Is not empty</p></td>
    </tr>
    <tr><td>Single-select</td>
        <td><p>Is</p>
        <p>Is not</p>
        <p>Is any of</p>
        <p>Is none of</p>
        <p>Is empty</p>
        <p>Is not empty</p></td>
    </tr>
    <tr>
        <td>Multi-select</td>
        <td><p>Has any of</p>
        <p>Has all of</p>
        <p>Is exactly</p>
        <p>Has none of</p>
        <p>Is empty</p>
        <p>Is not empty</p></td>
    </tr>
    <tr>
        <td>Numeric, percentage, currency</td>
        <td><p>=</p>
        <p>≠</p>
        <p><</p>
        <p>></p>
        <p>≤</p>
        <p>≥</p>
        <p>Is empty</p>
        <p>Is not empty</p></td>
    </tr>
    <tr>
        <td>Date</td>
        <td><p>Is</p>
        <p>Is not</p>
        <p>Is after</p>
        <p>Is before</p>
        <p>Is between</p><p>Is not between</p>
        <p>Is empty</p><p>Is not empty</p></td>
    </tr>
    </tbody>
    </table>

1. Type the value for the field that you want to filter for.
1. (Optional) Click **Add filter condition** to add another filtering option and repeat the above steps. 
1. Click the following operators to indicate how the filter conditions are joined and should be applied:

    * **And**: All specified conditions must be met. 
    * **Or**: Any of the specified conditions must be met.
    
    The results found after applying the filter display automatically. <!--at this time, you can't name and save the filter - but will this change?!-->
    <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->
1. (Optional) Click **Filters**, then click the **x** icon to remove a filter.

### Add groupings {#add-groupings}

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. 
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. <!--start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!-->
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. <!-- did they rename this to "Grouping"?!-->
        <!--insert screen shot-->
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. The grouping is applied automatically to the timeline and records display inside the grouping box.    <!-- ensure this is correct functionality here-->
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. <!--ensure this says "grouping" and not "group"-->
    
    1. (Optional) Click **Clear all** to remove all groupings.  


### Sort information {#sort-information}

By applying a sort, you can organize information in a given order. 

You can sort the following information:

* All records in a table or timeline view. <!--verify this is the case for the timeline view-->
* All groupings. 

To sort ungrouped records, do the following:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. <!--add steps here for sorting records with no groupings-->

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. <!--add steps here for sorting grouped records-->

## Manage the timeline view {#manage-the-timeline-view}

<!--insert screen shot of timeline view-->

When creating a timeline view, all records of the selected record type display in a chronological timeline.

Consider the following: 

* You can create a Timeline view only when you have at least two date fields associated with a record type. When you have one or no date fields associated with a record type, the Timeline view option is dimmed. 

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
--> 

Manage the timeline view: 

1. Start creating or accessing an existing timeline view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. Update the following view elements as described in the subsections below:
    * [Filters](#add-filters) 
    * [Grouping](#add-groupings)
    * [Sort](#sort-information) <!-- not sure if this is present in timeline views?!-->
    * [Settings]

### Edit the timeline view settings {#edit-the-timeline-view-settings}

Update the timeline view settings to indicate what information should display in the timeline section of the view. 

1. Create a timeline view, as described in [Create or edit record views](#create-or-edit-record-views).
1. Click **Settings**. 
1. Click **Date and time**, then select a **Star date** and an **End date** to display on the timeline. You can choose the default Start and End dates, or you can choose any date field that you created. Start dates are required. The bars representing the records start on the date you indicate for the Start date and end on the date corresponding with the End date. 
1. Click **Record details**, then start typing the name of a field in the **Search field** box. 

    You can select up to 4 fields to display on each record's bar. By default, only the Name field displays and cannot be removed. You must create the fields before you can add them to the record bars. 
1. Click **Save**.
    The timeline view is applied with the settings you selected. 


## Similarities and differences between the table and timeline views

The following table shows the similarities and differences between the table and timeline views in Maestro: 

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

## Add a view as a favorite

## Share views

## Delete views




