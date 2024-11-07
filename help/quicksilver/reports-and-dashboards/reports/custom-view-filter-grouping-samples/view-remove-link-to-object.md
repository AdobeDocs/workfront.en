---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Remove Link to an Object in a Column'
description: Some objects that you display in a view link to the Details page of the object, by default. For example, the column that displays the Name of a project is a link to the project; the column that displays the Name of a user is a link to the user's profile page.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
---
# View: remove link to an object in a column

<!--Audited: 11/2024-->

Some objects that you display in a view link to the Details page of the object, by default. For example, the column that displays the Name of a project is a link to the project; the column that displays the Name of a user is a link to the user's profile page.

You can remove this link using text mode in columns that display in all views.

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


## Example: Remove the link to a task from the Task Name column in a task view:

1. Go to a list of tasks.
1. From the **View** drop-down menu, click **New View** to create a new view.

   Or

   Click  the **Edit icon** ![](assets/edit-icon.png)

   to edit an existing view, then select the view.

1. Click **Add Column** to add a new column.

   Or

   Click an existing column with a link to an object.

1. Click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >You can use similar code for other objects by doing adjusting the following:
   >
   >* Replace the `valuefield` line of the code with `valueexpression` and keep the same name included in curly brackets after the equal sign.
   >* Eliminate all the lines that start with `link.` from the original text of the column. For example, eliminate all the following lines:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Click **Done**, then **Save View**.

