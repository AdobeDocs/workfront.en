---
filename: view-display-objects-not-in-standard-interface
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: View: display objects that are not included in the standard interface
description: You can display in a view objects that are not included in the standard mode interface. You can do this only by referencing them via text mode. You can determine which fields can be included in a view in either of the following ways:
---

# View:&nbsp;display objects that are not included in the standard interface

You can display in a view objects that are not included in the standard mode interface. You can do this only by referencing them via text mode.  
You can determine which fields can be included in a view in either of the following ways:

* Use the [API Explorer](https://one.workfront.com/s/api-explorer) to discover other objects that can be referenced via text mode.  
  Not all the fields documented in the API Explorer are valid fields for text mode. Some fields are only reportable through the API.

* Find the object 's ID field in a column. Most objects that have a field ID also have a corresponding column or field name which may not be accessible through the standard mode interface.

  You can use text mode to include in a view the column or field name instead of the ID by replacing the 

  ```
  fieldnameID
  ```

  with the 

  ```
  fieldname:name
  ```

  .  
  For example, in the standard mode interface, the `Portfolio Owner ID` field is available for a project view, but the `Portfolio Owner Name` field is not. You can use text mode to display the `Portfolio Owner Name` in the column of a view.

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

## Example: add the Portfolio Owner Name column to a project view

1. Go to a list of projects.
1. From the `View` drop-down menu, click `New View`.

1. Click `Add Column` then start typing "Portfolio Owner ID" in the `Show in this column` field, then select it when it displays in the list.

1. Click `Switch to Text Mode`.
1. Hover over the text mode area, and click `Click to edit text`.
1. Replace the 

   ```
   valuefield
   ```

   line (

   ```
   valuefield=portfolio:ownerID
   ```

   ) with the following line: 

   ```
   valuefield=portfolio:owner:name
   ```

   Or

   Remove the text you find in the `Text Mode` box, and replace it with the following code:
   <pre>valuefield=portfolio:owner:name</pre><pre>querysort=portfolio:owner:name</pre><pre>valueformat=HTML</pre><pre>displayname=Portfolio Owner Name</pre><pre>linkedname=portfolio</pre>

   >[!TIP]
   >
   >To replace any field    >
   >
   >```   >
   >ID
   >```   >
   >
   >with the field    >
   >
   >```   >
   >name
   >```   >
   >
   >using text mode, always replace    >
   >
   >```   >
   >ID
   >```   >
   >
   >with    >
   >
   >```   >
   >:name
   >```   >
   >
   >in the    >
   >
   >```   >
   >valuefield
   >```   >
   >
   >line.

1. Click `Save`, then `Save View`.

