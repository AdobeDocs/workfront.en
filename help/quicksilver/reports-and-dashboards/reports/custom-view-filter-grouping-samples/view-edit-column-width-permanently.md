---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: permanently edit the width of a column'
description: You can temporarily modify to width of columns by dragging and dropping their margins to match the desired width. For more information, see Modify column width and order.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
---
# View: permanently edit the width of a column

<!-- Audited: 1/2024 -->

You can temporarily modify to width of columns by dragging and dropping their margins to match the desired width. For more information, see [Modify column width and order](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

To permanently change the width of any column of any view, you must use text mode in the column as you edit the view.

## Access requirements

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
   <td> <p>New:<ul><li>Contributor to modify a view</li><li>Standard to modify a report</li></ul></p><p>Or</p>Current:<ul><li>Request to modify a view</li><li>Plan to modify a report</li></ul></p> </td> 
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

## Permanently edit the width of a column

>[!IMPORTANT]
>
>If you manually modify the width of a column as described in the section [Modify width and order of columns temporarily](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) in the article [Modify column width and order](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) after you have permanently modified the width of the column, the width of the column is preserved according to your manual resizing. In this case, the width of the column updated according to the following steps is overwritten. You can view the column according to the width defined in the following steps after you clear your cache or log in from another browser.
>
>For additional information about customizing the width of columns when using the Text Mode interface, see the "width" and "stretch" definitions in the [Glossary of Adobe Workfront terminology](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md). 

1. Go to a list of objects.
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column** to add a new column.

   Or

   Click the column header of any existing column.

1. Click **Switch to Text Mode**.
1. Hover over the text mode area, and click **Click to edit text**.
1. Add the following code to the text mode of the column:

   ```
   width=200
   usewidths=true
   ```

   For the **width** line, specify any number (in pixels) that represents how wide you want the column to display in the view.

1. Click **Save**, then **Save View**.


