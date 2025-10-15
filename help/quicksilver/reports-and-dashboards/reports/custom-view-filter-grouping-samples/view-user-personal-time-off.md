---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: user personal time off'
description: 'View: User Personal Time Off'
author: Nolan
feature: Reports and Dashboards
exl-id: 9b55b302-5cdc-4437-9ce4-a15b5b43dccb
---
# View: user personal time off

<!--Audited: 11/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider hiding this article because this is not a custom view anymore.)</p>
-->

You can build a Time Off report to capture users' time off information.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a view </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## View user personal time off

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **Reports > New Report**. 
1. From the drop-down menu, select **Time Off**.
1. Click **Save + Close**.

   The report displays the following fields in the view by default:

   | User |The name of the user who indicated the time off in their profile. |
   |---|---|
   | Start Date |The Start&nbsp;Date of the period of time off that the user indicated. |
   | End Date |The End Date of the period of time off that the user indicated. |

   {style="table-layout:auto"}

1. (Optional) Finish creating the report by editing any of the following tabs:

   * Columns (View)
   * Groupings
   * Filters
   * Chart

   For information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   >[!TIP]
   >
   >We recommend adding a grouping for the User object, to make the report easier to read.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Add Time Off information to a user report</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: old way of doing this, not working anymore)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To add a column to a user view or report to display a list of future days which have been marked for time off by users:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/time-off-report-350x61.png" alt="time_off_report.png" style="width: 350;height: 61;"> </p>
-->

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;<strong>Reports > New Report.</strong> </li>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the&nbsp;<strong>New Report</strong> drop-down menu, select&nbsp;<strong>User Report</strong>.</li>
   -->

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Add Column</strong>.</li>
   -->

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the <strong>View</strong> drop-down menu, select <strong>New View</strong>.</li>
   -->

   <!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the header of the new column, then click<strong>Switch to Text Mode</strong>.</li>
   -->

   <!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Mouse over the text mode area, and click <strong>Click to edit text</strong>.</li>
   -->

   <!--
   <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">Remove the text you find in the <strong>Text Mode</strong> box, and replace it with the following code:<br><!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">displayname=Personal Time Off<br>listdelimiter=<span><br>listmethod=nested(reservedTimes).lists<br>name=Upcoming Time Off<br>stretch=0<br>textmode=true<br>type=iterate<br>valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'')<br>valueformat=HTML<br>width=150</pre>
   </li>
   -->

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <strong>Save</strong>+<strong>Close</strong>.</li>
   -->
