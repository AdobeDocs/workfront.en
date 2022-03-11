---
filename: column-show-name-parent-tasks-all-caps
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: View: show name of parent tasks as all caps
description: You can add this column to a task view to display the name of the parent tasks in all capital letters.
---

# View: show name of parent tasks as all caps

You can add this column to a task view to display the name of the parent tasks in all capital letters.

![](assets/column-task-with-all-caps-parent-350x112.png)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Show name of parent tasks as all caps

To build this column in a task view:

1. Go to a list of tasks.
1. From the `View` drop-down menu, select `Customize View`.  
   Or  
   From the `View` drop-down menu, select `New View`.

1. In the `Column Preview` area, click the header of the column that shows the task name in the list.
1. Click `Switch to Text Mode`.
1. Mouse over the text mode area, and click `Click to edit text`.
1. Remove the text you find in the `Text Mode` box, and replace it with the following code: <pre><br>descriptionkey=name<br>displayname=Task Name<br>textmode=true<br>valueexpression=IF({numberOfChildren}>"0",UPPER({name}),{name})<br>valueformat=HTML<br>width=150<br></pre>

1. Click `Save View`.

