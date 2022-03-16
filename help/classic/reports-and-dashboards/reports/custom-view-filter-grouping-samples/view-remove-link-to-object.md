---
filename: view-remove-link-to-object
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: View: remove link to an object in a column
description: Some objects that you display in a view link to the Details page of the object, by default. For example, the column that displays the Name of a project is a link to the project; the column that displays the Name of a user is a link to the user's profile page.
---

# View: remove link to an object in a column

Some objects that you display in a view link to the Details page of the object, by default. For example, the column that displays the Name of a project is a link to the project; the column that displays the Name of a user is a link to the user's profile page.

You can remove this link using text mode in columns that display in all views.

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

## Example: Remove the link to a task from the Task Name column in a task view:

1. Go to a list of tasks.
1. From the `View` drop-down menu, click `New View` to create a new view.

   Or

   Click Customize View to edit an existing view, then select the view.

1. Click `Add Column` to add a new column.

   Or

   Click an existing column with a link to an object.

1. Click `Switch to Text Mode`.
1. Hover over the text mode area, and click `Click to edit text`.
1. Remove the text you find in the `Text Mode` box, and replace it with the following code:
   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><span class="bold">valueexpression={name}</span><br>valueformat=Compound</pre>
   ` `**Tips: **``  You can use similar code for other objects by doing adjusting the following:

  * Replace the `valuefield` line of the code with `valueexpression` and keep the same name included in curly brackets after the equal sign.

  * Eliminate all the lines that start with   
  
    ```  
    link.
    ```  
  
    from the original text of the column. For example, eliminate all the following lines:
    <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>

1. Click `Save`, then `Save View`.

