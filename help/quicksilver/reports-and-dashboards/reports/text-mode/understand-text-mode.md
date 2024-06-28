---
product-area: reporting
navigation-topic: text-mode-reporting
title: Text Mode overview
description: You can build a report or a list in Adobe Workfront by using either the standard or the text mode interface when creating the elements that make up the report or the list. 
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
---
# Text Mode overview

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time) </p>
-->

You can build a report or a list in Adobe Workfront by using either the standard or the text mode interface when creating the elements that make up the report or the list. 

The standard interface allows you to reference fields and their attributes that are readily available in the Workfront interface. 

Using text mode you can reference fields and attributes that might not be available in standard mode, but are available in the Workfront database.

For more information about creating reports using text mode, including classes, videos, and tutorials, see the Learn section on the Adobe Experience League site. 

## Considerations before using text mode

>[!TIP]
>
>You can also expand the capabilities of calculated custom fields by using a version of text mode for custom fields. The syntax and rules for creating a calculated custom field are different than those you use in reports and lists. For information about adding a calculated custom field, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Before you start using text mode in your reports, we strongly recommend that you take our classes on advanced reporting, to gain a deeper understanding of our text mode language. <!--outdated: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* We recommend that you use standard mode to ensure the reports you create remain intact when the Workfront software is updated. While text mode enables you to create more complex views, filters, and groupings, it is also more complicated to maintain and is not guaranteed when the Workfront software is updated.
* We recommend that you always try to build all reporting elements in the standard interface and switch to the text mode builder only for few adjustments.

  >[!TIP]
  >
  >Using the standard builder gives you important building blocks and patterns of code that you can then use when modifying the code in text mode.

* There are a set of rules and a unique syntax that you must use in order to successfully build reports and lists in text mode. Make sure you are familiar with the Workfront syntax for text mode before you begin.

  For information about the syntax and rules for using text mode, see [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* After you customize a reporting element in text mode, you might either not be able to switch back to standard mode (in a view) or the code for the element you created might be deleted (in filters and groupings.) This is because not all fields that are supported in text mode are supported in standard mode.

## Standard Mode interface

The Standard Mode interface displays fields to map the application elements that you want to display in a report or a list. The standard mode interface is a set of drop-down menus from which you can select the fields you want to display in your reports or lists.

For more information about the standard mode interface and to learn how to create a report or a list, see:

* [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 
* [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Text Mode interface

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add a section or note with a link to an another article about the syntax of text mode >> link to the Calc custom fields vc calc. columns)</p>
-->

Text mode enables you to create more complex views, filters, groupings, and prompts by allowing you to use fields that are not available in the standard mode interface. In&nbsp;Workfront text mode is a collection of coded statements that indicate what objects you want to display in a report or a list.

For a complete list of all our reportable fields, see the [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Not all the fields available through the API are available through the text mode interface. If you use the correct field in your text mode code and you do not display the results you expect, then the field might only be reportable through the API.

## Access reporting elements and edit text mode {#access-reporting-elements-and-edit-text-mode}

Accessing the text mode interface is similar for views, groupings and filters when accessing them from a report or a list.

For information about using text mode in views, filters, and groupings, see:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see what articles these sections are linked to and edit those articles to link to the individual ones)</p>
-->

* [Edit a view using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md) 
* [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md) 
* [Edit text mode in a grouping](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Custom prompts can only be edited in text mode. You can access prompts only from a report.

For information about accessing the text mode interface for custom prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Common reasons to use Text Mode {#common-reasons-to-use-text-mode}

Outside of creating custom prompts which can only be configured using text mode, we recommend that you use the report builder to build your views, filters and groupings. However, there are some instances where you can use text mode to enhance your reports and lists.

For more information about common uses for text mode, see [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).


  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Editing the text mode code inside views, filters, and groupings has some differences outlined below.</p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below, and the four subsections >>> drafted and created individual articles.)</p>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-text-mode-in-a-view" class="MCXref xref">Edit text mode in a view</a> </li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-text-mode-in-a-filter" class="MCXref xref">Edit text mode in a filter</a> </li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-text-mode-in-a-grouping" class="MCXref xref">Edit text mode in a grouping</a> </li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-a-custom-prompt" class="MCXref xref">Edit a custom prompt</a> </li>
  -->

  <!--
  <h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-text-mode-in-a-view"><strong>Edit text mode in a view</strong> </h4>
  -->

  <!--
  <note type="tip">
  We recommend that you build as much of the view as possible in standard mode, then convert it to text mode to edit it.
  </note>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To access the text mode interface for a view:</p>
  -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Find the report you want to modify in text mode.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have manage permissions to a report in order to be able to edit it.</p>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>. </li>
   -->

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit</strong>.</li>
   -->

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Columns (View)</strong> tab of the report builder, select a column in the report.</li>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Switch to Text Mode</strong> in the upper-right corner of the report builder.</p>
   -->

   <!--
   <note type="note">
   When you edit a column in text mode, Workfront adds the
   <code>textmode=true</code> line of code to the column. This indicates that the column is modified in text mode.
   </note>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following table outlines the key lines in a text mode view or grouping:</p>
   -->

   <!--
   <table style="table-layout:auto">
   <col>
   <col>
   <thead>
   <tr>
   <th data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Sample Line</strong> </th>
   <th data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Description</strong> </th>
   </tr>
   </thead>
   <tbody>
   <tr>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>valuefield</strong>=</p>
   </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following scenarios exist:</p>
   <ol>
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is: <code>valuefield=plannedStartDate</code></li>
   <li value="2">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valuefield=More information</code> </p>
   </li>
   <li value="3">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to display objects that are related to other objects in a view using the <code>valuefield</code> line of code the object names and attributes are separated by colons. </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valuefield=project:portfolio:owner:name</code> </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). </p>
   </li>
   </ol>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p>
   <note type="note">
   If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column.
   </note>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>valueformat=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information. </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p>
   </td>
   </tr>
   <tr>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>valueexpression=</strong> </p>
   </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can add this line to replace <code>valuefield</code>, if you want to display a calculated field in the column.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following scenarios exist: </p>
   <ol>
   <li value="1">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to display a field in a column in upper case, you would use:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpression=UPPER({valuefield})</code> </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The <code>valuefield</code> of the object is spelled as it appears in the API Explorer. </p>
   </li>
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to add multiple <code>valuefields</code> by stringing them together, you must separate them by a period.</li>
   <li value="3">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you want to display the name of the Primary Assignee of a task using <code>valueexpression</code>, you would use:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpreesion={assignedTo}.{name}</code> </p>
   </li>
   <li value="4">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. </p>
   <note type="important">
   <span>When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see</span>
   <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a></span>.
   </note>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following <code>valueexpression</code> to indicate this:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpression=UPPER({DE:Developer Name}</code>) </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p>
   </li>
   </ol> </td>
   </tr>
   <tr>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>descriptionkey= / description=</strong> </p>
   </td>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: <code>description=Your Value</code>.</td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>namekey= / name=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines the column label. In this case it is using the abbreviated value based on the key.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to modify the column name you can change this value to: <code>name=Your Value</code></p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>Name</code> allows you to enter any text for the column name, while<code>namekey</code> requires you enter a key that is used to translate the name of a column.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To change the column name you can also add the <code>displayname </code>line, if one is not present.</p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>displayname =</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can add the following line to change the name of a column, which suspends the <code>namekey/name</code> value:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>displayname=Your Value</code> </p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>querysort=</strong> </td>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run.</td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>width=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">When you modify this field manually in text mode, you must also add the <code>usewidths=true</code> value to your column.</p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>usewidths=true</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must use this line in addition to the <code>width=</code> line when customizing the width of a column. </p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>makeFieldEditable=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines whether the value displayed in a column is inline editable or not. If this line equals <strong>true,</strong> the value in the column is inline editable. If this line equals <code>false</code>, the value in the column is not inline editable.</p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>link.valuefield=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the <code>valuefield=</code> line. When you insert this, you must also add the <code>link.valueformat=</code> line. </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> For example, you can insert link.valuefield=priority in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page.</p>
   --> </td>
   </tr>
   <tr> <!--
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>link.valueformat=</strong> </td>
<td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Insert this line only when you have inserted the <code>link.valuefield</code> line to add a link to the value in a column. The link opens the details page of the object. This value should match the <code>valueformat=</code> line and indicates the format used to display the <code>valuefield</code>. </p>
   <note type="important">
   When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are
   <code> link.valuefield</code> and
   <code>link.valueformat</code>.
   </note>
   </td>
   </tr>
   </tbody>
   </table>
   -->

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</li>
   -->

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</li>
   -->

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-text-mode-in-a-filter"><strong>Edit text mode in a filter</strong> </h4>
-->

<!--
<note type="tip">
We recommend that you build as much of the filter of the report as possible in standard mode, then convert the filter to text mode to edit it.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about building filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To access the text mode interface for a filter:</p>
-->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Find the report you want to modify in text mode.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have manage permissions to a report in order to be able to edit it.</p>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>.</li>
   -->

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit</strong>.</li>
   -->

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Filters</strong> tab of the report, choose either <strong>Apply Existing Filter</strong>, or <strong>Add a Filter Rule.</strong></li>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Define the conditions of your filter.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Use the filter modifiers to define the condition of your filter. For more information about filter modifiers, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Switch to Text Mode</strong> in the upper-right corner of the report builder.</p>
   -->

   <!--
   <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">When using filter modifiers that are available only in text mode, remember that for each filter condition you have two lines of code: one defines the condition and the second one defines the modifier of the filter.</li>
   -->

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you want to filter for users who are in the same Home Group but not in the same Home Team as the logged in user, your filter should look like the following, in text mode:</li>
   -->

   <!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeGroupID=$$USER.homeGroupID</pre>
   -->

   <!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeGroupID_Mod=in</pre>
   -->

   <!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeTeamID=$$USER.homeTeamID</pre>
   -->

   <!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeTeamID_Mod=notin</pre>
   -->

   <!--
   <li value="13" data-mc-conditions="QuicksilverOrClassic.Draft mode">For a complete list of filter modifiers in text mode, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</li>
   -->

   <!--
   <li value="14" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</li>
   -->

   <!--
   <li value="15" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</li>
   -->

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-text-mode-in-a-grouping"><strong>Edit text mode in a grouping</strong> </h4>
-->

<!--
<note type="tip">
We recommend that you build as much of the grouping as possible in standard mode, then convert it to text mode to edit it.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To access the text mode interface for a grouping:</p>
-->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Find the report you want to modify in text mode.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have manage permissions to a report in order to be able to edit it.</p>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>.</li>
   -->

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit</strong>.</li>
   -->

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Groupings</strong> tab of the report builder, choose either <strong>Apply Existing Grouping</strong>, or <strong>Add Grouping.</strong></li>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Start typing the name of a field that you want to group by.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the name of the field when you see it in the list.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <strong>Switch to Text Mode</strong> in the upper-right corner of the report builder.</p>
   -->

   <!--
   <note type="note">
   When you edit a grouping in text mode, Workfront adds the
   <code>textmode=true</code> line of code to the grouping. This indicates that the grouping is modified in text mode.
   </note>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/grouping-switch-to-text-mode-350x173.png" alt="grouping_switch_to_text_mode.png" style="width: 350;height: 173;"> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The grouping is then displayed in text mode. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you want to group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode: </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>textmode=true</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.linkedname=project</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.namekey=view.relatedcolumn</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.valuefield=project:name</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.namekeyargkey.0=project</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.namekeyargkey.1=name</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.valueformat=string</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.linkedname=assignedTo</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.namekey=view.relatedcolumn</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.valuefield=assignedTo:name</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.namekeyargkey.1=nam</code>e</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.valueformat=string</code> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Each field in the grouping has several lines of code that refer to that field. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The lines of code that refer to the same field selected in the grouping are numbered with the same number, as follows:</p>
   -->

  <!--   
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The first grouping of the report has a group number of 0. All lines referring to the first grouping start with <code>group.0.</code></li>   
  -->

  <!--   
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The second grouping of the report has a group number of 1. All lines referring to the second grouping start with <em><code>group.1</code>.</em></li>   
  -->

  <!--   
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The third grouping of the report has a group number of 2. All lines referring to the third grouping start with <em><code>group.2</code>.</em></li>   
  -->

  <!--   
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Only in text mode, you can add a group number of 3, for a fourth grouping. All lines referring to the fourth grouping start with <em><code>group.3</code>.</em></li>   
  -->

   <!--
   <note type="note">
   Four groupings are not supported in the report builder. They are only supported when using text mode. Workfront does not support more than four levels of groupings.
   </note>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The key lines in a text mode grouping are similar to the fields available in views. The only lines that are not found in a grouping but are found in a view are <code>width</code> and <code>makeFieldEditable</code>. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about the key lines in text mode in a view or grouping, see the section <a href="#edit-text-mode-in-a-view" class="MCXref xref">Edit text mode in a view</a> in this article. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Add one of the following lines of code to any grouping to indicate whether the results in the grouping should display in an expanded or collapsed list. By default, groupings display expanded:</p>
   -->

   <!--   
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.iscollapsed=true </code>if you want the grouping to display with the results collapsed</li>   
   -->   

   <!--   
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.iscollapsed=false</code> if you want the grouping to display with the results expanded</p>   
   -->

   <!--   
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report)</p>   
   -->

  <!--
   >[!TIP]
   >
   >When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.
   >
   >The results of a grouping always display expanded after accessing them from a chart element.
   -->

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</li>
   -->

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</li>
   -->

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-a-custom-prompt">Edit a custom prompt</h4>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Custom prompts can only be edited in text mode. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about creating a custom prompt, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p>
-->


