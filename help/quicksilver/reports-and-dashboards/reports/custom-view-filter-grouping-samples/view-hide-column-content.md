---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: hide the content of a column'
description: You might want to hide information in the column of a view. You can do this by modifying the text mode of the column.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
---
# View: hide the content of a column

You might want to hide information in the column of a view. You can do this by modifying the text mode of the column.

>[!TIP]
>
>* You can use hidden columns to sort by a certain object that you do not want to display in the view.  
>  For example, you can sort by Task Number in a task view and hide the Task Number information from the view. In this case, the object referenced in the column helps sorting the view, but the information of that object does not display in the view.
>* When you hide a column, note that the information in the column is hidden, but the column still exists in the view.
>

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
   <td> <p>Request to modify a view </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Example: Sort and hide the Task Number column in a task view:

1. Go to a list of tasks.
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column** and start typing "Task Number" in the **Show in this column** field then select it when it displays in the list.

1. Click **Switch to Text Mode**.
1. Hover over the text mode area, and click **Click to edit text**.
1. Remove the text you find in the **Text Mode** box, and replace it with the following code:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>The important changes in this code which make the column hidden are:
   
     ```   
     displayname
     ```   
   
     this line must be blank.
   
     ```   
     valuefield
     ```   
   
     This has been replaced by *value*, and must be blank.
   
     ```   
     width
     ```   
   
     : Depending on the field, this must have a value of *0* or *1*.

1. Click **Save**, then **Save View**.
