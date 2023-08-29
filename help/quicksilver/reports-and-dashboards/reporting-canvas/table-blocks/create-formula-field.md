---
title: Build a formula field in Reporting Canvas
description: Build a formula field in Reporting Canvas
hidefromtoc: yes
hide: yes
---

# Build a formula field in Reporting Canvas

The field builder in Reporting Canvas allows you to create fields that perform custom calculations.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas beta: overview](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

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
   | IF | Compare two arguments based on a selected modifier, then perform a specified action based on the resulting True (Is True:) or False (Is False:) value. Note: currently, the second argument cannot be a static True or False value. Instead, you can use a nested function like ISBLANK(Project Name) that always returns False as a workaround. |True/False, Date, Number, or String |
   | CONCAT |Merge two or more strings together end-to-end to create a new string. |String |
   | CONTAINS |Evaluate if a string argument field (Find text) is contained within another string argument field (Within text). |True/False |
   | IN |Evaluate if the value of an argument field (Find) matches the value of at least one other argument field (Within) |True/False |
   | ISBLANK |Evaluate if an argument field is blank. |True/False |
   | LEN |Measure the length (in number of characters) of an argument field. |Number |
   | ROUND |Returns a rounded number based on the selected precision. |Number |
   | FLOOR |Returns the nearest whole number, rounded down. |Number |
   | NUMBER |Returns the greatest interger less than the value of a numerical argument (identical to a Floor function). |Number |
   | STRING |Converts the contents of an argument field into a string |String |
   | SUBSTR |Create a new string from a larger string, which contains the characters between one index number (Start) through another (End). |String |
   | LEFT |Create a new string from a larger string, which contains characters starting with the left-most and counting right a number of characters (Length). |String |
   | RIGHT |Create a new string from a larger string, which contains characters starting with the right-most and counting left a number of characters (Length). |String |
   | SUM |Add the values of two or more argument fields together. |Number |
   | SUB |Subtract the values of two or more argument fields (in order from left to right). |Number |
   | PROD |Multiply the values of two or more argument fields together. |Number |
   | DIV |Divide the value of two or more argument fields (in order from left to right). |Number |
   | MONTH |Returns a number equal to the month value for a date. |Number |
   | YEAR |Returns a number equal to the year value for a date. |Number |
   | DATEDIFF |Calculates the total number of days between two dates, rounded to one decimal place. |Number |
   | WEEKDAYDIFF |Calculates the number of weekdays between two dates, rounded to one decimal place. |Number |   

   {style="table-layout:auto"}

1. Click the **Go back** arrow in the top-left corner of the screen to return to your table.
