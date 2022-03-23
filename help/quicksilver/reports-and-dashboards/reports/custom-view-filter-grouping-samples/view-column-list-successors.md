---
filename: view-column-list-successors
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: View: add a list of task successors in a column
description: You can add a column to a task view to show a list of the successors of the tasks. The Task Successors column includes the number of the successor as well as the name.
---

# View: add a list of task successors in a column

You can add a column to a task view to show a list of the successors of the tasks. The **Task Successors** column includes the number of the successor as well as the name.

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Add a list of task successors in a column

To add this column to a task view:

1. Go to an existing task view.
1. Expand the View drop-down menu, and select **Customize View**.
1. Click **Add Column**.
1. Click **Switch to Text Mode**.
1. Mouse over the **Show in this column** area, and click **Click to edit text**.

1. Remove all text in the Text Mode box, and replace it with the following code:  
   <pre>displayname=Task Successors<br>listdelimiter=<br><br>listmethod=nested(successors).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})<br>valueformat=HTML</pre>

1. Click **Save View**.

