---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Error message when running a report: 'You are not currently logged in.'"
description: Learn about the 'You are not currently logged in' error message.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
---
# Error message when running a report: "You are not currently logged in."

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
   <td> <p>Manage permissions to a report</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problem

When running a report, or displaying it in a dashboard, the following error returns:  
*Let's try that again. You are not currently logged in.*

No results are displayed in the report.

## Cause

The report is currently set to run as a deactivated user.

## Solution

You must have Manage permissions to the report to be able to change the report settings.  
To adjust the report and see the results:

1. Go to the report.
1. Click **Report Actions** > **Edit** > **Report Settings**.

1. Specify the name of an active user in the **Run this report with the Access Rights of:** field.  
   Or  
   Leave the **Run this report with the Access Rights of:** field blank.

1. Click **Done**.
1. Click **Save + Close**.  
   The error should not appear again when running this report.
