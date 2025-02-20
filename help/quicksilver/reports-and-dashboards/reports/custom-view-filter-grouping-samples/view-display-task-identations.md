---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Display Task Indentations in a Task List'
description: In this task view, you can add code to the Task Name column to display the tasks indented according to the Work Breakdown Structure of the project.
author: Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
---
# View: display task indentations in a task list

<!--Audited: 11/2024-->

In this task view, you can add code to the Task Name column to display the tasks indented according to the Work Breakdown Structure of the project.

![View task indentation](assets/view-text-mode-indentation-task-list-350x171.png)

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
    <p>New:</p>
   <ul><li><p>Contributor to modify a filter </p></li>
   <li><p>Standard to modify a report</p></li> </ul>

   <p>Current:</p>
   <ul><li><p>Request to modify a filter </p></li>
   <li><p>Plan to modify a report</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Display task indentations in a column of a task list

1. Go to a list of tasks.
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column** and start typing "Task Name" in the **Show in this column** field then select it when it displays in the list.

1. From the new column, click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the `valuefield=` line and replace it with the following code:

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Click **Done**, then **Save View**.
1. (Optional) Update the view name, then click **Save View**.
