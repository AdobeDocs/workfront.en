---
title: Build a formula field in Reporting Canvas
description: Build a formula field in Reporting Canvas
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
---

# Build a formula field in Reporting Canvas

The field builder in Reporting Canvas allows you to create fields that perform custom calculations.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas beta: overview](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

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

   {style="table-layout:auto"}

1. Click the **Go back** arrow in the top-left corner of the screen to return to your table.
