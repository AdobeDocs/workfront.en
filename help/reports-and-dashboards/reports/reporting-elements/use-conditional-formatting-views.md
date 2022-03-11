---
filename: use-conditional-formatting-views
product-area: reporting
navigation-topic: reporting-elements
title: Use conditional formatting in Views
description: As you share your reports with other users in Adobe Workfront, consider customizing the View of the reports, to make certain information easier to read, or just stand out.
---

# Use conditional formatting in Views

As you share your reports with other users in&nbsp;Adobe Workfront, consider customizing the View of the reports, to make certain information easier to read, or just stand out.

You can customize the Details tab of your reports by adding special or conditional formatting to the view of your reports.

You must have Manage permissions to the report, to be able to edit it and add special formatting to the View.

For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

By conditionally formatting columns in the View of the report, you can set up rules that affect the way the report is displayed. When those conditions or rules are met, the special formatting is applied.

For example, if the percent complete of a task&nbsp;is less than 20 percent, you can highlight the field by showing the percentage number in bold, red text, and a yellow background color.

With a conditionally formatted View,&nbsp;you can:

* Change the header of a column.
* You can change the value of a column to customized text or an image.
* Format the display of a field by changing the font type, color, alignment, or the color of the background.

The changes you make in the View of the report take effect only in the Details tab of the report. These changes do not affect the Summary, Matrix, or Chart tabs of the report.

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
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit a view in a report</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to create or edit a view in a report</p> <p>Manage permissions to a view</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must create a report before you can add conditional formatting to it.

For information on creating a report, see [Create a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Create a conditionally formatted View

<ol> 
 <li value="1"> Click the Main Menu icon in the upper-right corner of Workfront,then click Reports. </li> 
 <li value="2"> <p>Click the name of a report where you want to create a conditionally-formatted view.</p> <p>Or</p> <p>Click&nbsp;<span class="bold">Report Actions</span>, then click&nbsp;<span class="bold">Edit</span>.</p> </li> 
 <li value="3">(Conditional) If you edited a report, select an existing column, or create a new column.<br></li> 
 <li value="4">Click <span class="bold">Advanced Options</span>.<br></li> 
 <li value="5"> <p>Specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Custom Column Label</td> 
     <td> <p>Specify a name for the column.</p> <p>If you are editing an existing column, specifying a name here changes the existing column name.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Field Format</td> 
     <td>Choose&nbsp;the format in which the value in the column displays. Depending on what the column field is, this allows you to set how dates, numbers, or currency display.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Show this column when on a Dashboard</td> 
     <td>Select this field if you want the column to display when the report is placed on a dashboard. The column always displays when you look at the report outside a dashboard.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Click <span class="bold">Add a Rule for this&nbsp;Column</span>.</p> <note type="note">
   You cannot apply conditional formatting to a User Team ID field.
  </note> </li> 
 <li value="7">In the <span class="bold">When the:</span> section, set a condition statement for the column. For example: when the Task Percent Complete Equals (Case Sensitive) 50.</li> 
 <li value="8"> <p>In the<span class="bold"> Show the field like this:</span>&nbsp;section specify what this field looks like when the condition defined above is met.<br>Specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Text Color</td> 
     <td> <p>Select the color in which the&nbsp;text is displayed. There are 8 colors available.</p> <note type="note">
       If the field contains a hyperlink, the text color selections are not applied to this field.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Text Format</td> 
     <td>Select whether to display text in bold or italic.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Text Alignment</td> 
     <td>Select whether to&nbsp;align the text&nbsp;to the right, center, or the left within the column.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Background</td> 
     <td>Select the color of the background for the text.&nbsp;There are 8 colors available.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Show Icon</td> 
     <td>Select from one of 16 icons, if you want to display an icon instead of the actual value for this column.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Show Text</td> 
     <td> <p>Select this option to display a custom label for this column, instead of its actual value. Specify the text to show instead of the value in the field provided.</p> <note type="important">
       Selecting 
       <span class="bold">Show Text</span> disables the ability to inline edit the text in this column.
       <br>Also, you can't change the value of a Predecessor column because it contains built-in logic.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Apply to the entire row</td> 
     <td>Select this option to apply settings to the entire row rather than applying settings to just the selected column.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="9">Click <span class="bold">Add Rule</span>.<br>You can add additional rules to the same column, or add rules to other columns.<br>Rules are applied in the order that they were created.<br>For example, you can first create a rule that states when the Project Status is Building, the&nbsp;text color is purple and bold. You then create a second rule that states when the Task Name is not blank, the text color is red and italicized, and the background color is green. In this example, the following occurs:<br>
  <ul>
   <li>Tasks whose Project Status is Building are displayed in purple and bold text. If the task name is not blank, tasks also have a green background.</li>
   <li>Tasks whose Project Status is anything other than Building (and the Task Name is not blank)&nbsp;are displayed in a red and italicized text&nbsp;with a green background.</li>
  </ul></li> 
 <li value="10">Click <span class="bold">Done</span>.</li> 
 <li value="11">Click <span class="bold">Save + Close</span>.<br>On the report, users see changes to the format if the conditions specified have been met.<br></li> 
</ol>

