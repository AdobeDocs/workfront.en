

# Add or edit a report table in Reporting Canvas

You can add a table to a report. 

<!--
A table ...
-->

##  

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
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to create reports, calendars, and dashboards</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> Object permissions Manage access to the report For information on requesting additional access, see Request access to objects in Adobe Workfront. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta program.

<!--
For more information, see [link to Beta enrollment info].
-->

## Add or edit a table in a report

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click `Reports`.
1. Click `New report`.

   Or

   Go to an existing report, click the `More` icon ![](assets/more-icon-27x15.png) in the report header, then select `Edit`.

1. In the report builder that opens, on the right side of the screen, double-click the `Table` icon ![](assets/table-icon.png) or drag it onto the canvas.

   If you double-click the icon, the table displays at the top of the canvas in its default size

   <!--
   , which you can change by dragging its corner handles
   -->

   .

1. Click **Untitled table** in the table header, then type a title for the table.

   ![](assets/table-name-350x142.png)

1. Click `Edit` on the table block to configure the table.

   >[!NOTE]
   >
   >If the table was already added when you opened the report, the Edit button does not display. To edit the table, click the Edit icon ![](assets/edit-icon.png) in the table header.
   >
   >
   >![](assets/edit-icon-table-header-350x71.png)   >
   >

1. In the right panel, locate a field that you want to add as a column to the table, then drag it to the table to add it where you want it, or double-click it to add it as the last column in the table.

   You can type text in the `Search` box to find a field. You can also use the 2 drop-down menus under this box to narrow the list of displayed fields to one or both of the following:

  * The object type associated with the field you want, such as Project or Task
  * The field type you want, such as Date or Currency

   If you don't see the field you want, click `More fields` to display more.

1. Repeat Step 6 for each field that you want to add as a column.

   >[!TIP]
   >
   >You can change the order of columns in a table by dragging a selected column to a new position.

1. To create a formula field to add as a column, click **New** at the top of the **Fields** list.

   <!--
   A formula field [briefly describe what it is].
   -->

   For instructions on creating a formula field, see [Create a formula field in Reporting Canvas](../../reports-and-dashboards/new-reporting-experience/create-formula-field.md).

1. Do any of the following to configure the table further:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Filter the information in the table</td> 
      <td> <p>Drag the field that you want to filter by to the <span class="bold">Filter</span> section above the table.</p> <p>For information about setting up filter rules, see <a href="../../reports-and-dashboards/new-reporting-experience/configure-filter-rules-for-table.md" class="MCXref xref">Configure filter rules in Reporting Canvas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group the table information based on attributes</td> 
      <td> <p>Drag the field that you want to group by to the <span class="bold">Group</span> section above the table.</p> <p>For more information on creating row groups, see <a href="../../reports-and-dashboards/new-reporting-experience/group-rows-in-table.md" class="MCXref xref">Group table rows in Reporting Canvas</a>.</p> </td> 
     </tr> <!--
      Resize the table Click the bottom-right corner and adjust the table to the width and height that you want.
     --> 
    </tbody> 
   </table>

