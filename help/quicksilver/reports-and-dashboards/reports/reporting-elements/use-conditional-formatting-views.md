---
product-area: reporting
navigation-topic: reporting-elements
title: Use conditional formatting in views
description: As you share your reports with other users in Adobe Workfront, consider customizing the view of the reports, to make certain information easier to read, or just stand out.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
---
# Use conditional formatting in views

<!-- Audited: 11/2024 -->

As you share your reports with other users in Adobe Workfront, consider customizing the view of the reports, to make certain information easier to read, or just stand out.

You can customize the Details tab of your reports by adding special or conditional formatting to the view of your reports.

For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

By conditionally formatting columns in the view of the report, you can set up rules that affect the way the report displays. When those conditions or rules are met, the special formatting is applied.

For example, if the percent complete of a task is less than 20 percent, you can highlight the field by showing the percentage number in bold, red text, and a yellow background color.

With a conditionally formatted view, you can:

* Change the header of a column.
* Change the value of a column to customized text or an image.
* Format the display of a field by changing the font type, color, alignment, or the color of the background.

The changes you make in the view of the report take effect only in the Details tab of the report. These changes do not affect the Summary, Matrix, or Chart tabs of the report.

## Access requirements

 +++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New:</p> 
   <ul><li>Standard for report views</li>
  <li> Contributor or higher for list views</li></ul>
   <p>Current:</p>
   <ul>
    <li> Plan for report views </li>
    <li> Request or higher for list views </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to Reports, Dashboards, Calendars to edit a view in a report</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>Manage permissions to a report to create or edit a view in a report</p> <p>Manage permissions to a view</p></td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

You must create a report before you can add conditional formatting to its view.

For information on creating a report, see [Create a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Create a conditionally formatted view

{{step1-to-reports}}

1. Click the name of a report where you want to create a conditionally-formatted view
   
   Or
   
   Click **New Report**, then select an object type to build a new report.

1. (Conditional) If you edit an existing report, click **Report Actions**, then click **Edit**.

1. In the **Columns (View)** tab, click to select an existing column, or click **Add Column** to create a column.  
1. In the **Show in this column** field in the upper-left corner of the report builder, select the field you want to display in the new column. 
1. Click **Advanced Options**.  

1. Specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Custom Column Label</strong></td> 
      <td> <p>Specify a name for the column.</p> <p>If you are editing an existing column, specifying a name here changes the existing column name.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Field Format</strong></td> 
      <td>Choose the format in which the value in the column displays. Depending on what the column field is, this allows you to set how dates, numbers, or currency display. Not all columns display this option.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Show this column when on a Dashboard</strong></td> 
      <td>Select this field if you want the column to display when the report is placed on a dashboard. The column always displays when you look at the report outside a dashboard.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Add a Rule for this Column**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. In the **When the:** section, set a condition statement for the column. 
   
   For example: "when the Task Percent Complete Equals (Case Sensitive) 50."
1. In the **Show the field like this:** section specify what this field looks like when the condition defined above is met.  
   
   Specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Text Color</strong></td> 
      <td> <p>Select the color in which the text is displayed using the color selector.</p> <p><b>NOTE</b></p> <p> If the field contains a hyperlink, the text color selections are not applied to this field.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Text Format</strong></td> 
      <td>Select whether to display text in bold or italic.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Text Alignment</strong></td> 
      <td>Select whether to align the text to the right, center, or the left within the column.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Background</strong></td> 
      <td>Select the color of the background for the text using the color selector.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Show Icon</strong></td> 
      <td>Select from one of 16 icons, if you want to display an icon instead of the actual value for this column.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Show Text</strong></td> 
      <td> <p>Select this option to display a custom label for this column, instead of its actual value. Specify the text to show instead of the value in the field provided.</p> <p><b>IMPORTANT</b></p> <p>Selecting <strong>Show Text</strong> disables the ability to inline edit the text in this column.<br>Also, you can't change the value of a Predecessor column because it contains built-in logic.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Apply to the entire row</strong></td> 
      <td>Select this option to apply settings to the entire row rather than applying settings to just the selected column.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Add Rule**.  
   You can add additional rules to the same column, or add rules to other columns.

   Rules are applied in the order that they were created. They are combined but they do not overwrite each other, though a column rule takes precedence over a row rule on the same cell.

   **EXAMPLE 1**
   
   You can first create a rule that states that when a project is in the Status of Building, the text color is purple and bold. You then create a second rule that states that when a task's Name is not blank, the text color is red and italicized, and the background color is green. In this example, the following occurs:

   * Tasks whose Project Status is Building are displayed in purple and bold text. If the task name is not blank, tasks also have a green background.
   * Tasks whose Project Status is anything other than Building (and the Task Name is not blank) are displayed in a red and italicized text with a green background.

   **EXAMPLE 2**
   
   Create a rule in the Project Planned Completion Date column that affects the entire row, turning the background gray if the project is canceled (for example, when the Project Status is Dead). Then create a column rule that turns the background red when the Project Planned Completion Date is less than today (meaning the project is late). In this example, if a canceled project has a late completion date, that cell will appear red even though the other cells in the row are gray. To correct this formatting:

   * Edit the formatting for the Planned Completion Date and delete the column rule for the red background on late projects.
   * Add a column rule with the same formatting as the row rule (gray background when the Project Status = Dead.)
   * Add the column rule again for the red background on late projects.
   * When you save the rules and the view, the red background is not applied to a canceled project.

1. Click **Save**.
1. Click **Save + Close**.  
   On the report, users see changes to the format if the specified conditions have been met.
