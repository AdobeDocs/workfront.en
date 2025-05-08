---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Hide the Content of a Column'
description: You might want to hide information in the column of a view. You can do this by modifying the text mode of the column.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
---
# View: hide the content of a column

<!--Audited: 11/2024-->

You might want to hide information in the column of a view. You can do this by modifying the text mode of the column.

>[!NOTE]
>
>* You can use hidden columns to sort by a certain object that you do not want to display in the view.  
>  For example, you can sort by Task Number in a task view and hide the Task Number information from the view. In this case, the object referenced in the column helps sorting the view, but the information of that object does not display in the view.
>* When you hide a column, note that the information in the column is hidden, but the column still exists in the view.

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
   <td> <p>New:<ul><li>Contributor to modify a view</li><li>Standard to modify a report</li></ul></p><p>Current:<ul><li>Request to modify a view</li><li>Plan to modify a report</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
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

## Example: Sort and hide the Task Number column in a task view:

1. Go to a list of tasks.
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column** and start typing "Task Number" in the **Show in this column** field then select it when it displays in the list.

1. Click **Switch to Text Mode**, then **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:

    ```
    displayname=
    linkedname=direct
    querysort=taskNumber
    sortOrder=1
    sortType=asc
    textmode=true
    value=
    valueformat=int
    width=0
    ```

   The important changes in this code which make the column hidden are:

    * `displayname=`: This line must be blank. 
    * `valuefield=`: This line must be replaced by `value=`, which must be blank.
    * `width=`: Depending on the field, this must have a value of **0** or **1**.

1. Click **Done**, then **Save View**.
