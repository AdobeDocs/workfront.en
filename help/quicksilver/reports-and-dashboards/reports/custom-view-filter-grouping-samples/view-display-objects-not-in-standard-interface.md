---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Display Objects that Are Not Included in the Standard Interface'
description: You can display in a view objects that are not included in the standard mode interface. You can do this only by referencing them via text mode. 
author: Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
---
# View:&nbsp;display objects that are not included in the standard interface

You can display in a view objects that are not included in the standard mode interface. You can do this only by referencing them via text mode.  
You can determine which fields can be included in a view in either of the following ways:

* Use the [API Explorer](../../../wf-api/general/api-explorer.md) to discover other objects that can be referenced via text mode.  
  Not all the fields documented in the API Explorer are valid fields for text mode. Some fields are only reportable through the API.

* Find the object 's ID field in a column. Most objects that have a field ID also have a corresponding column or field name which may not be accessible through the standard mode interface.

  You can use text mode to include in a view the column or field name instead of the ID by replacing the `fieldnameID` with the `fieldname:name`.

  For example, in the standard mode interface, the **Portfolio Owner ID** field is available for a project view, but the **Portfolio Owner Name** field is not. You can use text mode to display the **Portfolio Owner Name** in the column of a view.

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

## Example: add the Portfolio Owner Name column to a project view

1. Go to a list of projects.
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column** then start typing "Portfolio Owner ID" in the **Show in this column** field, then select it when it displays in the list.

1. Click **Switch to Text Mode**, then **Edit Text Mode**.
1. Replace the `valuefield` line (`valuefield=portfolio:ownerID`) with the following line: 

   `valuefield=portfolio:owner:name`
  
   Or

   Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:

    ```
    valuefield=portfolio:owner:name
    querysort=portfolio:ownerID
    valueformat=HTML
    displayname=Portfolio Owner Name
    linkedname=portfolio
    ```

   In this particular example, the report will sort the report by the Portfolio Owner ID, as indicated by the `querysort` line.

   >[!TIP]
   >
   >To replace any field `ID` with the field `name` using text mode, always replace `ID` with `:name` in the `valuefield` line.

1. Click **Done**, then **Save View**.
