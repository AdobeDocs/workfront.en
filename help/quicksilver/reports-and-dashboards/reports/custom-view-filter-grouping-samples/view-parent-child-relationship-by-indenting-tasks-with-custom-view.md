---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Display the Parent-Child Relationship in a Task by Indenting the Tasks'
description: You can maintain the distinction of parent - child relationships in an exported task list by adding a custom view to the task list and ensuring this view is selected before you export the list.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
---
# View: display the parent-child relationship in a task by indenting the tasks

<!--Audited: 11/2024-->

You can maintain the distinction of parent - child relationships in an exported task list by adding a custom view to the task list and ensuring this view is selected before you export the list. 

![](assets/parent-child-indented-custom-view-350x94.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p> Current: 
   <ul>
   <li>Request to modify a view</li> 
   <li>Plan to modify a report</li>
   </ul>
     </p>
     <p> New: 
   <ul>
   <li>Contributor to modify a view</li> 
   <li>Standard to modify a report</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Display the parent-child relationship in a task by indenting the tasks

1. Go to the project with the task list you'd like to export.
1. Click the **View** drop-down menu, and select **New View**.
1. Click in the **Task Name** column header.  
1. Select **Switch to Text Mode** in the top-right corner.
1. Click **Edit Text Mode** and remove all existing text.
1. Paste the following text:  

   
   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ``` 

1. Click **Done** > **Save View**.
