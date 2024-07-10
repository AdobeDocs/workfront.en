---
title: Manage the calendar view
description: You can display records and their fields in a calendar view.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
---
# Manage the calendar view

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

You can display records and their fields in a calendar view, from the record type page.

For information about Adobe Workfront Planning capabilities views and how to manage them, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

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
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
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
   <p>System administrators have access only the views they created or that are shared with them. </p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level configuration</td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to the view</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


<!--Replace above table with this: 

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
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## Manage a calendar view {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Consider the following: 

* You can create a Calendar view only when you have at least two date fields associated with a record type. When you have one or no date fields associated with a record type, the Calendar view option is dimmed. 
   
   You can select from record date fields, or lookup date fields from connected record or object types.
* The following scenarios exist:

    * When both the Start and End dates have no values, the records do not display on the calendar
    * When the Start or the End dates have no value, the record displays as a one-day event
    * When the Start date is after the End date, the record does not display on the calendar.

To manage a calendar view: 

1. Go to the record type page for which you want to view the calendar. 
1. Create a calendar view, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

    ![](assets/calendar-view-example.png)

    The records associated with the record type you selected display as bars in a calendar. The color of the bars matches the color of the record icon. 

1. Do one of the following to navigate through the calendar:

    * Click the left and right icons or use the horizontal scroll to move backwards and forwards in the calendar. 
    * Click **Today** to center the calendar to today's date. 
    * Select one of the following options from the time frame drown-down menu to update the time increments: 

        * Month
1. Update the following view elements as described in the subsections below:
    * [Filters](#add-filters)
    <!--* [Grouping](#add-grouping)-->
    <!--* [Settings](#edit-the-calendar-view-settings)-->
    <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Add filters

You can reduce the amount of information displayed on the screen by using filters.

Consider the following when working with filters in the calendar view: 

<!-- this list is almost identical to the one for the table view - update both-->

* The filters you create for a calendar view work independently from the filters in any other view applied to the same record type. 

* The filters are unique to the view that you select. Two calendar views of the same record type can have different filters applied to them. 

* Two users looking at the same calendar view see the same filter that is currently applied. 

* You cannot name the filters you build for a calendar view.

* Removing filters removes them from anyone accessing the same record type as you and who displays the same view as you do. 

* Adding filters in the calendar view is identical to adding filters in the table view. 

   For more information, see the "Add filters" section in the article [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

* You can filter by connected record fields or lookup fields, but not for those fields that allow linking to multiple records.
