

# Build a formula field in Reporting Canvas

The field builder in Reporting Canvas allows you to create fields that perform custom calculations.

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

## Create a formula field

1. Create or navigate to a table block, as described in [Add or edit a table block in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. On the table header in the report, click the **Edit** icon ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >If you just created the table and haven't yet added any fields, click the Edit button in the center of the table instead.

1. Click **New +** at the top of the **Fields** list on the right panel.
1. In the new page that opens, click the **Edit** icon ![](assets/edit-icon.png) next to the field name in the top-left corner to change the name of the formula field.
1. Drag **Functions** or **Fields** from the left panel onto the field builder in the center to add them to your formula field.

   >[!TIP]
   >
   >As you build your formula field, the **Field preview** on the right displays examples of the resulting field.

   Each function contains a number of empty dotted rectangles that will be used as arguments in calculating a result. These may be populated by entering static text or numbers, dragging and dropping a field from the left panel (using the field's value in the calculation), or by dragging and dropping another function (creating a nested function). Possible functions include:

   | Function |Description |Output |
   |---|---|---|
   | CONCAT |Merge two or more strings together end-to-end to create a new string. |String |
   | CONTAINS |Evaluate if an argument field ("Find text" string) is contained within another argument field ("Within text" string). |True/False |
   | IF |&nbsp; |&nbsp; |
   | ISBLANK |Evaluate if an argument field is blank. |True/False |
   | LEN |Measure the length (in number of characters) of an argument field. |Number |
   | ROUND |&nbsp; |&nbsp; |
   | SUBSTR |Create a new string from a larger string, which contains the characters between one index number (Start) through another (End). |String |

   <!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(Optional)&nbsp;You can edit, reorder, or delete multiple functions in a field.</p> </li>
   -->

1. Click the **Go back** arrow in the top-left corner of the screen to return to your table.

