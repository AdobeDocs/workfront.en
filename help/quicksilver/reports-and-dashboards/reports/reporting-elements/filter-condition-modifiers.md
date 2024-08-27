---
product-area: reporting
navigation-topic: reporting-elements
title: Filter and condition modifiers
description: The filter and condition modifiers allow you to build filters and establish conditions for formatting your report results.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
---
# Filter and condition modifiers

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

The filter and condition modifiers allow you to build filters and establish conditions for formatting your report results.

For more information about building filters, see the article [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

For more information about using conditional formatting in Views, see the article [Use conditional formatting in views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter and condition modifiers

Some modifiers are built-in and you can choose them from a drop-down menu inside your filter or conditional formatting statement. Other modifiers can only be used in text mode filters. 

For more information about understanding text mode, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

For a list of built-in time frame modifiers, see the article [Filter reports by time frames](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

You can use the following condition modifiers in filters and conditional formatting statements:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Built-in Modifier</strong> </p> </th> 
   <th> <p><strong>Text Mode Modifier</strong> </p> </th> 
   <th> <p><strong>Description</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Is Blank</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>The field exists for the object but the field does not currently have a value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Is Not Blank</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>The field you are filtering for exists and has been given a value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>The field is either blank, or does not exist. For example, you want to look for items without a parent task ID. This means that you want to see only standalone tasks. The qualifier for the "parent task ID" would be <strong>null</strong>, since a task without an ID (in this case the parent) does not exist. </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>The field that you are filtering for exists and contains a value other than null.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contains</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> version of <strong>contains</strong>. For example: <code>cicontains inf</code> captures any value that contains either <code>Inf</code> or <code>inf</code>.</p> <p> <p>Note: Adobe Workfront searches for the exact word or phrase that you are specifying for each filter statement. For example, if you are searching for any project that contains the phrase <code>new project</code> in the name, Workfront does not display projects that have just <code>new</code> or just <code>project</code>, or <code>new main project</code> in the name. The filter finds only projects with the exact phrase <code>new project</code> in the name.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Does Not Contain</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> version of <strong>notcontains</strong>.</p><p>This modifier filters for items that are missing the value specified.</p> <p>For example, <code>does not contain inf</code> captures anything without <code>Inf</code> or <code>inf</code> in the name.</p> <p>Note: <span>If the field you are filtering for has multiple options, this filters out the results that contain both the choice you specify, as well as the choice you specify and any additional choices.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td>&nbsp;</td> 
   <td> <p><strong>contains</strong> </p> </td> 
   <td> <p> Searches for the specified <i>case sensitive</i> text throughout an entire text string.</p> <p>For example, using <code>contains Inf</code> captures anything with <code>Inf</code> in it, such as the word <code>Infinity.</code></p> <p>This modifier can only be used in text mode filters.For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>It filters for items that are missing the <i>case sensitive</i> value specified.</p> <p>For example, <code>notcontains inf</code> captures anything without <code>inf</code>, but it displays values that contain <code>Inf</code>.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> option of <strong>eq</strong>. It only returns an exact match of the searched value.</p> <p>For example, when searching for a task with a specific name, <code>task name cieq test</code> finds tasks where the name is <code>Test</code>, <code>TEST</code>, or <code>Test</code>, but it does not find a task with the name <code>test 123.</code></p> <p>When searching for a status, the <strong>cieq</strong> modifier is not supported. You should use the case sensitive modifier, <strong>eq</strong>, to search for a status.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td>&nbsp;</td> 
   <td><strong>cine</strong> </td> 
   <td> <p>This is the <i>case insensitive</i> option of <strong>ne</strong>, and it is the opposite of the <b>cieq</b> modifier. It only returns results that are not an exact match of the searched value, not taking in account the case of the value.</p> <p>For example, <b>cine</b> returns any values that do not equal either "current" or "Current". </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>This modifier returns only an exact, <i>case sensitive</i> match of the searched value.</p> <p>For example, when searching for complete projects, <code>eq CPL</code> returns all projects in the Complete status. <code>eq CPL, CUR</code> does not return a result because a project cannot be complete and current at the same time.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td>&nbsp;</td> 
   <td><strong>ne</strong> </td> 
   <td> <p>This is the <i>case sensitive</i> opposite of <strong>eq</strong>. It returns only results that are not an exact match of the searched value, and it also matches the case of the value.</p> <p>For example, <b>ne</b> returns any values that do not equal "Current", but it does not return any values that do not equal "current". </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> This is the <i>case insensitive</i> version of <strong>in</strong>.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> version of <strong>notin</strong>.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Equal</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>This modifier allows you to create a comma-separated list of <i>case sensitive</i> variables to compare to a single attribute evaluated in a filter. The entire list is treated as an OR statement and returns any results that meet the criteria of one or more of the variables.</p> <p>For example, when searching for projects, using <code>in CUR, PLN, CPL</code> returns all projects that are in the Current, OR Planning, OR Complete status.</p> <p>The built-in modifier <strong>Equal</strong> corresponds to the text mode modifier of <strong>in</strong>. This means that you can choose Equal with multiple values for the field.</p> <p>For example, you are able to choose a "Status equals Current, Planning, Dead" in a project report and you can view projects in any of these statuses.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Not Equal</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>This is the <i>case sensitive</i> opposite of <strong>in</strong>. It returns only results not in the specified list.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> <p>Note: <span>If the field you are filtering for has multiple options, this filters out the results that contain both the choice you specify, as well as the choice you specify and any additional choices.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>This modifier searches for portions of a <i>case sensitive</i> text string in similar fashion to <strong>contains</strong>. However, <strong>like</strong> provides the ability to insert wild card characters to break up the text.</p> <p>For example, when searching for notes, using <code>like %Current% %Dead%</code> returns any note that contains the phrase "Current to Dead". It does not include any notes that contain "Dead to Current". Each value is searched in the order it is listed. The % represents a wild card to replace characters or segments of text. An underscore can also be used for a single wildcard character, as in <code>like Project_</code> that returns both "Project" and "Projects". If you intend on using a <strong>like</strong> or <strong>clike</strong> modifier in your filtering, we recommend avoiding % or _ characters in custom data field names, parameter option values, or other object names.</p><p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>This is the <i>case insensitive</i> version of <strong>like</strong>. For example: <code>cilike %Current% %Dead%</code> returns any notes that contain <code>Current to Dead</code> or <code>current to dead</code>.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Does Not Exist</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>This modifier is used only with complex filters in an EXISTS statement. These filters refer only to the following objects: </p> 
    <ul> 
     <li>Objects that span multiple levels in the object hierarchy </li> 
     <li>Objects that are missing </li> 
    </ul> <p>For information about creating complex filters using EXISTS statements see the article <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Create Complex Text-Mode Filters Using EXISTS Statements</a>. This is the only modifier used in EXISTS statements.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Greater Than</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>This searches for all results with a value greater than the value entered, not including the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Less Than</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>This searches for all results with a value less than what is entered, not including the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Greater Than Equal</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>This searches for all results with values greater than or equal to the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Less Than Equal</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>This searches for all results with a value less than or equal to the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Between</strong> </p> </td> 
   <td> <p><strong>between</strong> </p> </td> 
   <td> <p>Provides two required field values and searches for all results within range of both fields, including the entered values.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>This is the inverse of <strong>between</strong>. It provides two required value fields and searches for all results outside the range of both fields including the entered values.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 

 </tbody> 
</table>
