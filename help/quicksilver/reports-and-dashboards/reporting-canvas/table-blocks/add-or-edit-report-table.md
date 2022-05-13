

# Add or edit a table block in Reporting Canvas

A table displays field information in columns that can be filtered, grouped, and sorted.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas Beta](../../../product-announcements/betas/reporting-canvas-beta.md).

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
   <td> <p>The contents of this article are available as part of a beta program that must be joined by a Workfront administrator. After joining, the Workfront administrator may then grant access to other users in their environment. For more information on participating in the beta and granting access to users, see <a href="../../../product-announcements/betas/reporting-canvas-beta.md" class="MCXref xref">Reporting Canvas beta</a>.</p> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit access to create reports, calendars, and dashboards</p>
    --> <!--
     <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add or edit a table block

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Reporting**.
1. Click **New report**.

   Or

   Go to an existing report, click the **More** icon ![](assets/more-icon-27x15.png) in the report header, then click **Edit**.

1. On the right side of the screen under **Add a block**, either:

   Drag the **Table** icon ![](assets/table-icon.png) onto the canvas directly to your desired location.

   Or

   Double-click the **Table** icon ![](assets/table-icon.png) to add a table to the top of the canvas.

   >[!TIP]
   >
   >You can change the size of the block after it is placed by dragging its corner handles.

1. Click **Untitled table** in the table header, then type a title for the table.

   ![](assets/table-name-350x142.png)

1. Click **Edit** in the center of the table block to configure the table.

   >[!NOTE]
   >
   >If the table was already part of the canvas (such as when editing an existing report), the **Edit** button does not display in the center of the block. To edit the table, click the **Edit** icon ![](assets/edit-icon.png) in the table header instead.
   >
   >
   >![](assets/edit-icon-table-header-350x71.png)   >
   >

1. In the **Fields** panel on the right, locate a field that you want to add as a column to the table, then either drag it onto the table where you want it or double-click it to add it as the last column in the table.

   You can type text in the **Search** box to find a specific field by name. You can also use the two drop-down menus under this box to narrow the list of displayed fields to one or both of the following:

   * The object type associated with the field you want, such as Project or Task
   * The field type you want, such as Date or Currency

   Repeat this step for each field that you want to add as a column.

   >[!TIP]
   >
   >You can change the order of columns in a table by dragging a selected column to a new position.

1. Do any of the following to configure the table further:

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Style</strong>: to change the style of the table, click the <strong>Style</strong> tab above the <strong>Fields</strong> list to see style options for the table. For more information on style options, see </p> </li>   
     -->   
   
   * **Add a formula field**: Click **New****+** at the top of the **Fields** list. For more instructions on creating a formula field, see [Build a formula field in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/create-formula-field.md).
   * **Add a filter**: Drag the field that you want the table to be filtered by onto the **Filter** section above the table. For more information on setting up filter rules, see [Filter a table in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/configure-filter-rules-for-table.md).
   * **Group rows by specific attributes**:&nbsp;Drag the field that you want the table to be grouped by onto the **Group** section above the table. For more information on creating row groups, see [Group table rows in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/group-rows-in-table.md).

