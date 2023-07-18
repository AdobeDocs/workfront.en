---
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
---

# Manage the table view

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

You can display records and their fields in a table view, when accessing the record type page in Adobe Maestro. 

For information about Maestro views, see [Manage record views](../views/manage-record-views.md). 


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

## Manage the table view {#manage-the-table-view}

<!--insert screen shot of table view-->

When creating a table view, all records of the selected record type display in a table. Each row is a unique record and each column is a record field. All fields and all records display by default. 

To manage a table view: 

1. Create a table view, as described in the article [Manage record views](../views/manage-record-views.md). 

    ![](assets/table-view-example.png)

1. Update the following view elements as described in the subsections below:
    * [Columns](#add-columns)
    * [Rows](#add-rows)
    * [Filters](#add-filters) 
    * [Grouping](#add-groupings)
    * [Sort](#sort-information)  


### Add columns {#add-columns}

The column headers of a Maestro table view display fields associated with the records in the view. The same fields displayed in the table view also display in the Details section of a Maestro record. For more information, see [Edit records](../records/edit-records.md). 

You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default. <!--ensure that there is a table for the timeline view - right not there is not, but they are working to add a table to the left of the timeline; if the table does not come with the timeline view, take this statement out-->

Adding columns to a view is identical to adding fields to a record type.  

You can add up to 500 fields (or columns) in a table view. 

1. Start adding fields (or columns), as described in the article [Create fields](../architecture-and-fields/create-fields.md). 

    The columns you add are visible to all uses who access the record type. 
<!-- not available yet
1. To increase the width of the columns, click and drag the column separation lines and drop them in the desired spot. 
1. To reorder the columns, click a column header and drag it, then drop it in the desired spot in the table. The changes you make to the column width and order are permanent and visible to all users who access the record type. 

    >[!TIP]
    >
    >    You cannot reorder fields that belong to linked objects. ********* Not sure if this is still accurate. Check! **************

1. To hide a column, hover over the column header, then click the downward-pointing arrow, then click **Hide**.

-->

### Add rows {#add-rows}

The rows of a Maestro table view display individual records of the selected record type. 

You can add up to 10,000 records (or rows) to a table in Maestro. 

Adding rows to a Maestro table view is identical to creating records in a table. 

1. Start adding record (or rows), as described in the article [Create records](../records/create-records.md). 
<!-- this is not possible right now:

1. To reorder the rows, click the row header, drag and drop it in the desired location. 

    The changes you make to the row order are permanent and visible to all users who access the record type
-->

### Add filters {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

Filters help you reduce the amount of information displayed on the screen.

Consider the following when working with filters in the table view: 

* You can apply filters both in the table and timeline views. The filters of the table view are independent from those in the timeline view of the same record type. 

* You cannot name the filters you build and apply to a table view.

* The filters you create are preserved and all users that can access Maestro view the record table with the same filters applied as you. 

* Removing filters removes them from anyone accessing the same record type as you.

* There is no limit to how many filters you can apply to a table. 

To add a filter to a table view: 

1. Create a table view, as described in the article [Manage record views](../views/manage-record-views.md). 
1. Select a table view, then click **Filters** in the upper-right corner of the table.    
1. Start typing a field in the **Select a field** box, then click it when it appears in the list. This is the field that you want to filter by. 

    ![](assets/filter-ui-table-view.png)

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
1. (Optional) Click **Add condition** to add another filtering option and repeat the above steps. The number of filters applied displays to the right of the Filters icon. 
1. Click the following operators to indicate how the filter conditions are joined and should be applied:

    * **And**: All specified conditions must be met. 
    * **Or**: Any of the specified conditions must be met.
    
    The results found after applying the filter display automatically. <!--at this time, you can't name and save the filter - but will this change?!-->
    <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->
1. (Optional) Click **Filters**, then click the **x** icon to remove a filter.

<!-- this is not available yet

### Add groupings {#add-groupings}

*******************this section might link in the future from the timeline view; right now it's only documented there; also, check the steps below because this was not released to the table when they were written*****************

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. 
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. ***************start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!**********************
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. ************************did they rename this to "Grouping"?!****************************
        ******************insert screen shot***********
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. The grouping is applied automatically to the timeline and records display inside the grouping box.    <********************ensure this is correct functionality here*************
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. **********ensure this says "grouping" and not "group"*****************
    
    1. (Optional) Click **Clear all** to remove all groupings.  

--> 

<!--This is not available yet: 


### Sort information {#sort-information}

By applying a sort, you can organize information in a given order. 

You can sort the following information:

* All records in a table or timeline view. ***********verify this is the case for the timeline view*********************
* All groupings. 

To sort ungrouped records, do the following:

1. Create a view, as described in the article [Manage record views](../views/manage-record-views.md)
1. ********************add steps here for sorting records with no groupings************

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->