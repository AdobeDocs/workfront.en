---
filename: understand-text-mode
product-area: reporting
navigation-topic: text-mode-reporting
title: Text Mode overview
description: You can build a report or a list in Adobe Workfront by using either the standard or the text mode interface when creating the elements that make up the report or the list. The standard interface allows you to reference fields and their attributes that are readily available in the Workfront interface. Using text mode you can reference fields and attributes that might not be available in standard mode, but are available in the Workfront database.
---

# Text Mode overview

You can build a report or a list in Adobe Workfront by using either the standard or the text mode interface when creating the elements that make up the report or the list. The standard interface allows you to reference fields and their attributes that are readily available in the Workfront interface. Using text mode you can reference fields and attributes that might not be available in standard mode, but are available in the Workfront database.

## Considerations before using text mode

>[!TIP]
>
>You can also expand the capabilities of calculated custom fields by using a version of text mode for custom fields. The syntax and rules for creating a calculated custom field are different than those you use in reports and lists. For information about adding a calculated custom field, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

<ul> 
 <li> <p>Before you start using text mode in your reports, we strongly recommend that you take our classes on advanced reporting, to gain a deeper understanding of our text mode language. For training materials on reporting see <a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Workfront Reports and Dashboards Learning Paths</a>.</p> </li> 
 <li> <p>We recommend that you use standard mode to ensure the reports you create remain intact when the Workfront software is updated. While text mode enables you to create more complex views, filters, and groupings, it is also more complicated to maintain and is not guaranteed when the Workfront software is updated.</p> </li> 
 <li> <p>We recommend that you always try to build all reporting elements in the standard interface and switch to the text mode builder only for few adjustments.</p> <note type="tip">
   Using the standard builder gives you important building blocks and patterns of code that you can then use when modifying the code in text mode.
  </note> </li> 
 <li> <p>There are a set of rules and a unique syntax that you must use in order to successfully build reports and lists in text mode. Make sure you are familiar with the Workfront syntax for text mode before you begin.</p> <p>For information about the syntax and rules for using text mode, see <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Text mode syntax overview</a>.</p> </li> 
 <li> <p>After you customize a reporting element in text mode, you might either not be able to switch back to standard mode (in a view) or the code for the element you created might be deleted (in filters and groupings.) This is because not all fields that are supported in text mode are supported in standard mode.</p> </li> 
</ul>

## Standard Mode interface

The Standard Mode interface displays fields to map the application elements that you want to display in a report or a list. The standard mode interface is a set of drop-down menus from which you can select the fields you want to display in your reports or lists.

For more information about the standard mode interface and to learn how to create a report or a list, see:

* [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 
* [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Text Mode interface

Text mode enables you to create more complex views, filters, groupings, and prompts by allowing you to use fields that are not available in the standard mode interface. In&nbsp;Workfront text mode is a collection of coded statements that indicate what objects you want to display in a report or a list.

For a complete list of all our reportable fields, see the [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Not all the fields available through the API are available through the text mode interface. If you use the correct field in your text mode code and you do not display the results you expect, then the field might only be reportable through the API.

* [Access reporting elements and edit text mode](#accessin) 
* [Common reasons to use Text Mode](#common)

## Access reporting elements and edit text mode

Accessing the text mode interface is similar for views, groupings and filters when accessing them from a report or a list.

For information about using text mode in views, filters, and groupings, see:

* [Edit a view using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md) 
* [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md) 
* [Edit text mode in a grouping](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Custom prompts can only be edited in text mode. You can access prompts only from a report.

For information about accessing the text mode interface for custom prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

<!--
Editing the text mode code inside views, filters, and groupings has some differences outlined below.
-->

  <!--
  Edit text mode in a view
  -->

  <!--
  Edit text mode in a filter
  -->

  <!--
  Edit text mode in a grouping
  -->

  <!--
  Edit a custom prompt
  -->

<!--
Edit text mode in a view
-->

<!--
Tip: We recommend that you build as much of the view as possible in standard mode, then convert it to text mode to edit it.
-->

<!--
To access the text mode interface for a view:
-->

1. 

   <!--
   Find the report you want to modify in text mode.
   -->

   <!--
   You must have manage permissions to a report in order to be able to edit it.
   -->

   <!--
   Click Report Actions.
   -->

   <!--
   Click Edit.
   -->

   <!--
   On the Columns (View) tab of the report builder, select a column in the report.
   -->

1. 

   <!--
   Click Apply if you want to save your changes and continue editing the report.
   -->

1. 

   <!--
   Click Save + Close to save your report.
   -->

1. 

   <!--
   Click Switch to Text Mode in the upper-right corner of the report builder.
   -->

   <!--
   Note: When you edit a column in text mode, Workfront adds the textmode=true line of code to the column. This indicates that the column is modified in text mode.
   -->

   <!--
   The following table outlines the key lines in a text mode view or grouping:
   -->

   <!--
   Sample Line Description valuefield= This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see API Explorer. The following scenarios exist: If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the valuefield. For example, for the Planned Start Date of a task the code is: valuefield=plannedStartDate If you want to display a custom field, the valuefield value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is: valuefield=More information If you want to display objects that are related to other objects in a view using the valuefield line of code the object names and attributes are separated by colons. For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line: valuefield=project:portfolio:owner:name This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). For information about how objects connect to one another, see the section Interdependency and hierarchy of objects in Understand objects in Adobe Workfront. Note: If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column. valueformat= This line represents the format used to display the valuefield. The valueformat identifies whether an object or field displays as text, number, percentage, or date. We recommend using HTML for your valueformat, especially when using valueexpression, to ensure the most accurate display of your information. For information about additional values for this line, see Use conditional formatting in Text Mode. valueexpression= You can add this line to replace valuefield, if you want to display a calculated field in the column. You must enclose the valuefield of the objects in curly brackets every time you use it in a valueexpression. The following scenarios exist: If you want to display a field in a column in upper case, you would use: valueexpression=UPPER({valuefield}) The valuefield of the object is spelled as it appears in the API Explorer. If you want to add multiple valuefields by stringing them together, you must separate them by a period. For example, if you want to display the name of the Primary Assignee of a task using valueexpression, you would use: valueexpreesion={assignedTo}.{name} If you want to use a custom field in a valueexpression line you must precede the name of the field by DE: to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. Important: When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see Create or edit a custom form. For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following valueexpression to indicate this: valueexpression=UPPER({DE:Developer Name}) When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name": valueexpression=UPPER({DE:Developer Name:name}) descriptionkey= / description= This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: description=Your Value. namekey= / name= This line defines the column label. In this case it is using the abbreviated value based on the key. If you want to modify the column name you can change this value to: name=Your Value Name allows you to enter any text for the column name, whilenamekey requires you enter a key that is used to translate the name of a column. To change the column name you can also add the displayname line, if one is not present. displayname = You can add the following line to change the name of a column, which suspends the namekey/name value: displayname=Your Value querysort= This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run. width= This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view. When you modify this field manually in text mode, you must also add the usewidths=true value to your column. usewidths=true You must use this line in addition to the width= line when customizing the width of a column. makeFieldEditable= This line defines whether the value displayed in a column is inline editable or not. If this line equals true, the value in the column is inline editable. If this line equals false, the value in the column is not inline editable. link.valuefield= Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the valuefield= line. When you insert this, you must also add the link.valueformat= line. For example, you can insert link.valuefield=priority in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page. link.valueformat= Insert this line only when you have inserted the link.valuefield line to add a link to the value in a column. The link opens the details page of the object. This value should match the valueformat= line and indicates the format used to display the valuefield. Important: When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are link.valuefield and link.valueformat.
   -->

   <!--
   Click Apply if you want to save your changes and continue editing the report.
   -->

   <!--
   Click Save + Close to save your report.
   -->

<!--
Edit text mode in a filter
-->

<!--
Tip: We recommend that you build as much of the filter of the report as possible in standard mode, then convert the filter to text mode to edit it.
-->

<!--
For more information about building filters, see Filters overview in Adobe Workfront.
-->

<!--
To access the text mode interface for a filter:
-->

1. 

   <!--
   Find the report you want to modify in text mode.
   -->

   <!--
   You must have manage permissions to a report in order to be able to edit it.
   -->

   <!--
   Click Report Actions.
   -->

   <!--
   Click Edit.
   -->

   <!--
   On the Filters tab of the report, choose either Apply Existing Filter, or Add a Filter Rule.
   -->

1. 

   <!--
   Define the conditions of your filter.
   -->

   <!--
   Use the filter modifiers to define the condition of your filter. For more information about filter modifiers, see Filter and condition modifiers.
   -->

1. 

   <!--
   Click Switch to Text Mode in the upper-right corner of the report builder.
   -->

   <!--
   When using filter modifiers that are available only in text mode, remember that for each filter condition you have two lines of code: one defines the condition and the second one defines the modifier of the filter.
   -->

   <!--
   For example, if you want to filter for users who are in the same Home Group but not in the same Home Team as the logged in user, your filter should look like the following, in text mode:
   -->

1. 

   <!--
   homeGroupID=$$USER.homeGroupID
   -->

1. 

   <!--
   homeGroupID_Mod=in
   -->

1. 

   <!--
   homeTeamID=$$USER.homeTeamID
   -->

1. 

   <!--
   homeTeamID_Mod=notin
   -->

   <!--
   For a complete list of filter modifiers in text mode, see the article Filter and condition modifiers.
   -->

   <!--
   Click Apply if you want to save your changes and continue editing the report.
   -->

   <!--
   Click Save + Close to save your report.
   -->

<!--
Edit text mode in a grouping
-->

<!--
Tip: We recommend that you build as much of the grouping as possible in standard mode, then convert it to text mode to edit it.
-->

<!--
To access the text mode interface for a grouping:
-->

1. 

   <!--
   Find the report you want to modify in text mode.
   -->

   <!--
   You must have manage permissions to a report in order to be able to edit it.
   -->

   <!--
   Click Report Actions.
   -->

   <!--
   Click Edit.
   -->

   <!--
   On the Groupings tab of the report builder, choose either Apply Existing Grouping, or Add Grouping.
   -->

1. 

   <!--
   Start typing the name of a field that you want to group by.
   -->

   <!--
   Select the name of the field when you see it in the list.
   -->

1. 

   <!--
   Click Switch to Text Mode in the upper-right corner of the report builder.
   -->

   <!--
   Note: When you edit a grouping in text mode, Workfront adds the textmode=true line of code to the grouping. This indicates that the grouping is modified in text mode.
   -->

   <!--

   -->

   <!--
   The grouping is then displayed in text mode.
   -->

   <!--
   For example, if you want to group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:
   -->

   <!--
   textmode=true
   -->

   <!--
   group.0.linkedname=project
   -->

   <!--
   group.0.namekey=view.relatedcolumn
   -->

   <!--
   group.0.valuefield=project:name
   -->

   <!--
   group.0.namekeyargkey.0=project
   -->

   <!--
   group.0.namekeyargkey.1=name
   -->

   <!--
   group.0.valueformat=string
   -->

   <!--
   group.1.linkedname=assignedTo
   -->

   <!--
   group.1.namekey=view.relatedcolumn
   -->

   <!--
   group.1.valuefield=assignedTo:name
   -->

   <!--
   group.1.namekeyargkey.0=assignedTo
   -->

   <!--
   group.1.namekeyargkey.1=name
   -->

   <!--
   group.1.valueformat=string
   -->

   <!--
   Each field in the grouping has several lines of code that refer to that field.
   -->

   <!--
   The lines of code that refer to the same field selected in the grouping are numbered with the same number, as follows:
   -->

    <!--  
    The first grouping of the report has a group number of 0. All lines referring to the first grouping start with group.0.  
    -->

    <!--  
    The second grouping of the report has a group number of 1. All lines referring to the second grouping start with group.1. 
    -->

    <!--  
    The third grouping of the report has a group number of 2. All lines referring to the third grouping start with group.2.  
    -->

    <!--  
    Only in text mode, you can add a group number of 3, for a fourth grouping. All lines referring to the fourth grouping start with group.3.  
    -->

   <!--
   Note: Four groupings are not supported in the report builder. They are only supported when using text mode. Workfront does not support more than four levels of groupings.
   -->

   <!--
   The key lines in a text mode grouping are similar to the fields available in views. The only lines that are not found in a grouping but are found in a view are width and makeFieldEditable.
   -->

   <!--
   For more information about the key lines in text mode in a view or grouping, see the section Edit text mode in a view in this article.
   -->

   <!--
   Click Apply if you want to save your changes and continue editing the report.
   -->

   <!--
   Click Save + Close to save your report.
   -->

<!--
Edit a custom prompt
-->

<!--
Custom prompts can only be edited in text mode.
-->

<!--
For more information about creating a custom prompt, see Add a prompt to a report.
-->

## Common reasons to use Text Mode

Outside of creating custom prompts which can only be configured using text mode, we recommend that you use the report builder to build your views, filters and groupings. However, there are some instances where you can use text mode to enhance your reports and lists.

For more information about common uses for text mode, see [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
