---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: display only items in an approval status'
description: You can display only items in a certain status which is currently in Pending Approval. This works the same for any other object with an approval status.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
---
# Filter: display only items in an approval status

You can display only items in a certain status which is currently in Pending Approval. This works the same for any other object with an approval status.

You can place the following objects in an approval status:

* Tasks
* Issues 
* Projects

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
   <td> <p>Request to modify a filter </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Display only items in approval status

1. Go to the filter you want to customize for a list of projects, for example.
1. Click **Add a Filter Rule** for the **Status** field of the object of your list.  
   For example, in a project report, add **Status Equal Planning**, if you want to display only projects which are in a status of **Planning - Pending Approval**.

1. Click **Switch to Text Mode**.
1. Modify the 

   ```
   status
   ```

   line by adding **:A** to the 3-letter key of the status:  
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Click **Done**, then **Save Filter**.

   The list displays only projects that are in a status of Planning - Pending Approval.
