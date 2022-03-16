---
filename: view-user-personal-time-off
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: View: user personal time off
description: You can build a Time Off report to capture users' time off information.
---

# View: user personal time off

You can build a Time Off report to capture users' time off information.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## View user personal time off

1. Click Reporting in your Global Navigation Area, then Reports > New Report. 
1. From the drop-down menu, select `Time Off`.
1. Click `Save + Close`.

   The report displays the following fields in the view by default:

   | User |The name of the user who indicated the time off in their profile. |
   |---|---|
   | Start Date |The Start&nbsp;Date of the period of time off that the user indicated. |
   | End Date |The End Date of the period of time off that the user indicated. |

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
Add Time Off information to a user report
-->

<!--
To add a column to a user view or report to display a list of future days which have been marked for time off by users:
-->

<!--

-->

   <!--
   Click Reporting in your Global Navigation Area, then Reports > New Report.
   -->

   <!--
   From the New Report drop-down menu, select User Report.
   -->

   <!--
   Click Add Column.
   -->

   <!--
   From the View drop-down menu, select New View.
   -->

   <!--
   Click the header of the new column, then click Switch to Text Mode.
   -->

   <!--
   Mouse over the text mode area, and click Click to edit text.
   -->

   <!--
   Remove the text you find in the Text Mode box, and replace it with the following code: displayname=Personal Time Off listdelimiter=<span> listmethod=nested(reservedTimes).lists name=Upcoming Time Off stretch=0 textmode=true type=iterate valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'') valueformat=HTML width=150
   -->

   <!--
   Click Save+Close.
   -->

