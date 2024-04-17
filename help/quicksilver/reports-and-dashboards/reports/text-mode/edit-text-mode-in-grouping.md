---
product-area: reporting
navigation-topic: text-mode-reporting
title: Edit text mode in a grouping
description: 'NOTE: make all FVG articles the same for editing in text mode)'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
---
# Edit text mode in a grouping

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

You can edit a grouping in a list or report using text mode to access fields that are not available in the standard interface and create more complex groupings.

>[!TIP]
>
>We recommend that you build as much of the grouping as possible in standard mode, then convert it to text mode to edit it.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
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
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit groupings in a report</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to edit groupings in a report</p> <p>Manage permissions to a grouping to edit it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before starting to use text mode in a report or list, always ensure that you are familiar with the Workfront text-mode syntax.

For more information, see:

* [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md) 
* [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md) 
* [Custom view, filter, and grouping samples: article index](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Edit text mode in a grouping

Editing a grouping using text mode is identical for reports and lists. Accessing the grouping from a report or from a list differs.

>[!NOTE]
>
>Groupings are a mandatory reporting element for creating charts in reports. Text-mode groupings are not supported in charts.&nbsp;For information about adding charts to reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

For more information about building groupings, see [Create groupings in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

For information about creating a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Do one of the following:

   1. To access the grouping from a report, go to the report, then click&nbsp;**Report Actions** > **Edit** > **Groupings** tab.
   1. To access the grouping from a list, go to the list and from the **Grouping** drop-down menu, mouse over the grouping that you want to modify and click the&nbsp;**Edit** icon ![](assets/edit-icon.png).

      The grouping builder opens.

1. Click&nbsp;**Add Grouping** to add the groupings, then click&nbsp;**Switch to Text Mode** in the upper-right corner of the builder.

   >[!TIP]
   >
   >You can add up to 3 groupings in the standard interface. You can add a 4th grouping only using text mode, and you cannot have more than 4 grouping levels in Workfront.

1. Start typing the name of a field that you want to group by.

   Select the name of the field when you see it in the list.

1. Click **Switch to Text Mode** in the upper-right corner of the builder.

   The grouping is then displayed in text mode.

   When you edit a grouping in text mode, Workfront adds the 

   ```
   textmode=true
   ```

   line of code to the grouping. This indicates that the grouping is modified in text mode.

   **Example:** To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >The lines in bold are mandatory.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Each field in the grouping has several lines of code that refer to that field.

   The table below outlines the key lines in a text mode grouping.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   >The key lines in a text mode grouping are similar to the lines required to build text-mode views.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>Sample Line</strong> </th> 
      <th><strong>Description</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>group.&lt;number&gt;.</strong> </td> 
      <td> <p>Each line of code is preceded by this text. The lines of code that refer to the same field selected in the grouping are numbered with the same number, as follows:</p> 
       <ul> 
        <li>The first grouping of the report has a group number of 0. All lines referring to the first grouping start with <code>group.0</code>.</li> 
        <li>The second grouping of the report has a group number of 1. All lines referring to the second grouping start with <em><code>group.1</code></em>.</li> 
        <li>The third grouping of the report has a group number of 2. All lines referring to the third grouping start with <em><code>group.2</code></em>.</li> 
        <li>Only in text mode, you can add a group number of 3, for a fourth grouping. All lines referring to the fourth grouping start with <em><code>group.3</code></em>.</li> 
       </ul> <p>Note: 4 groupings are not supported in the builder. They are only supported when using text mode. Workfront does not support more than 4 levels of groupings.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>The following scenarios exist:</p> 
       <ol> 
        <li value="1"> <p> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>If you want to group by objects that are related to other objects using the <code>valuefield</code> line of code the object names and attributes are separated by colons.</p> <p>For example, a grouping by Portfolio Name for a task list has the following value for the valuefield line:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>This indicates that from the object of the report (task), you can access the next related object (project); from there, you can access the following related object from project (portfolio); then the portfolio name (name).</p> </li> 
       </ol> <p>For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> <p>Note: If you choose a field in text mode that is not valid in the standard interface and you switch to the standard interface, the grouping is deleted.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p> <p>We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information.</p> <p>For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>You can add this line to replace <code>valuefield</code>, if you want to group your list by a calculation between several fields.</p> <p>You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p> <p>The following scenarios exist:</p> 
       <ol> 
        <li value="1"> <p>If you want to display the name of a grouping in upper case, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> of the object is spelled as it appears in the API Explorer.</p> </li> 
        <li value="2">If you want to add multiple <code>valuefields</code> by stringing them together in a <code>valueexpression </code>line, you must separate them by a period.<p>For example, if you want to display the name of the portfolio in upper case in a task list, you would use the following code in the <code>valueexpression</code> line:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface.</p><p>Important: <span>When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the <code>valueexpression </code>is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a></span>.</p><p>For example, if you have a custom field labeled "Developer Name" and you want to group by this field and display it in upper case, you can use the following <code>valueexpression</code> to indicate this:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>This line defines the grouping label. In this case it is using the abbreviated value based on the key.</p> <p>If you want to modify the grouping name you can change this value to the following:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> allows you to enter any text for the grouping name, while <code>namekey</code> requires you enter a key that is used to translate the name of a grouping.</p> <p>To change the grouping name you can also add the <code>displayname </code>line, if one is not present.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>You can add the following line to change the name of a column, which overwrites the <code>namekey/name</code> value:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>We recommend removing all the lines that contain <code>name </code>when you rename a grouping.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Add one of the following lines of code to any grouping to indicate whether the results in the grouping should display in an expanded or collapsed list. By default, groupings display expanded:

   
     ```   
     group.0.iscollapsed=true
     ```   
   
     if you want the grouping to display with the results collapsed
   
     ```   
     group.0.iscollapsed=false
     ```   
   
     if you want the grouping to display with the results expanded

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

     >[!TIP]
     >   
     >* When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.
     >* The results of a grouping always display expanded after accessing them from a chart element.

1. Click **Done** if you want to save your changes and continue editing the grouping or report.
1. Click **Save Grouping** in a list or **Save + Close** to save your report.
