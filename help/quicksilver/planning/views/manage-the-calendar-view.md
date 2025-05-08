---
title: Manage the calendar view
description: You can display records and their fields in a calendar view. This article describes how you can create a calendar view and edit or delete an existing one.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
---
# Manage the calendar view

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can display records and their fields in a calendar view, from the record type page.

For information about Adobe Workfront Planning views and how to manage them, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

## Access requirements

+++ Expand to view access requirements. 

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
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes Planning.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have Planning enabled by default.</span></p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

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

    ![Calendar view example](assets/calendar-view-example.png)

    The records associated with the record type you selected display as bars in a calendar. The color of the bars matches the color of the record icon. 

1. Do one of the following to navigate through the calendar:

    * Click the left and right icons or use the horizontal scroll to move backwards and forwards in the calendar. 
    * Click **Today** to center the calendar to today's date. 
    * Select one of the following options from the time frame drown-down menu to update the time increments: 

        * **Month**: Records display in a monthly calendar.


        * **Week**: Records display in the following areas:

            * Records that span over multiple days display at the top of the calendar.
            * Records that last a day or less, display in the lower half of the calendar view. If you selected to display the hour of he Start and End Dates, the record displays at the appropriate time within the day that it occurs.
         

1. Update the following view elements as described in the subsections below:
    * [Filters](#add-filters)
    * [Settings](#edit-the-calendar-view-settings)
    <!--* [Grouping](#add-grouping)-->
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

* You can filter by connected record fields or lookup fields. 

* You can filter by lookup fields that display multiple values.

### Edit the calendar view settings

Editing the calendar view settings is similar to editing the settings of a timeline view.

For more information, see the "Edit the timeline view settings" section in the article [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 
