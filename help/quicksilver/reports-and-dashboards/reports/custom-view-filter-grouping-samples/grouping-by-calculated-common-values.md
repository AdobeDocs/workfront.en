---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Grouping: organize list results by a calculated value common to all objects in the grouping'
description: You might want to view your tasks grouped by Percent Complete in ranges of 0-25, 26-50, 51-75, 75-99, and 100. You can create a grouping using text mode to do this.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
---
# Grouping: organize list results by a calculated value common to all objects in the grouping

You might want to view your tasks grouped by Percent Complete in ranges of 0-25, 26-50, 51-75, 75-99, and 100. You can create a grouping using text mode to do this.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request to modify a grouping </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a grouping</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr>   
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Organize list results by a calculated value common to all objects in the grouping

To apply this grouping to a list of tasks:

1. Go to a list of tasks. 
1. From the **Grouping**drop-down menu, select **New Grouping**.

1. Click **Switch to Text Mode**.
1. In the available space, add the following code:

   ```
   textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({
   ```

   ```
   percentComplete
   ```

   ```
   }>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete
   ```

1. Click **Done**, then **Save Grouping**.
