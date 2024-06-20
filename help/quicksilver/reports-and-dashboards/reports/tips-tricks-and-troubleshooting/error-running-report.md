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

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

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
