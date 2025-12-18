---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Error message on calendar: 'This calendar has the view rights of a deactivated user.'"
description: Learn about 'This calendar has the view rights of a deactivated user' error message.
author: Jenny
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
---
# Error message on calendar: "This calendar has the view rights of a deactivated user."

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
     <p>Standard</p>
     <p>Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a calendar</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problem

You receive the following error when accessing a calendar shared with you:&nbsp;

*This calendar has the view rights of a deactivated user. Please have an administrator fix the calendar privileges.*

## Cause

The user who has created this calendar (its original owner) is a user who has been deactivated.&nbsp;

## Solution

You can resolve this in the following way:

1. Copy the original calendar. When you copy a calendar, you become the owner of the calendar. The copied calendar should show all the information from the original calendar.  
   For more information about copying a calendar, see [Copy a calendar report](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Share the copied calendar with the same users as the original calendar. All users should see the same information on the new calendar.
1. (Optional and conditional) If you have permissions to manage the original calendar, remove all other users with whom the calendar is shared from the calendar Sharing area. This eliminates the confusion of the users trying to display the wrong calendar.
