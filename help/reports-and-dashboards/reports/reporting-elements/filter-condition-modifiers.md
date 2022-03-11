---
filename: filter-condition-modifiers
product-area: reporting
navigation-topic: reporting-elements
title: Filter and condition modifiers
description: The filter and condition modifiers allow you to build filters and establish conditions for formatting your report results.
---

# Filter and condition modifiers

The filter and condition modifiers allow you to build filters and establish conditions for formatting your report results.

For more information about building filters, see the article [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

For more information about using conditional formatting in Views, see the article [Use conditional formatting in Views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter and condition modifiers

For a list of built-in time frame modifiers, see the article [Filter reports by time frames](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Some modifiers are built-in and you can choose them from a drop-down menu inside your filter or conditional formatting statement. Other modifiers can only be used in text mode filters. For more information about understanding text mode, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

You can use the following condition modifiers in filters and conditional formatting statements:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><span class="bold">Built-in Modifier</span> </p> </th> 
   <th> <p><span class="bold">Text Mode Modifier</span> </p> </th> 
   <th> <p><span class="bold">Description</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><span class="bold">Is Blank</span> </p> </td> 
   <td> <p><span class="bold">blank</span> </p> </td> 
   <td> <p>The field exists for the object but the field has not yet been given a value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Is Not Blank</span> </p> </td> 
   <td> <p><span class="bold">notblank</span> </p> </td> 
   <td> <p>The field you are filtering for exists and has been given a value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">null</span> </p> </td> 
   <td> <p>The field is either blank, or does not exist. For example, you want to look for items without a parent task ID. This means that you want to see only standalone tasks. The qualifier for the "parent task ID" would be <span class="bold">null</span>, since a task without an ID (in this case the parent) does not exist. </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">notnull</span> </p> </td> 
   <td> <p>The field that you are filtering for exists and contains a value other than null.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Contains</span> </p> </td> 
   <td> <p><span class="bold">cicontains</span> </p> </td> 
   <td> <p>(Case insensitive) This is the case insensitive version of <span class="bold">contains</span>. For example: "cicontains inf" captures any value that contains either "Inf" or "inf".</p> <p> <p>Note: <span>Adobe Workfront</span> searches for the exact word or phrase that you are specifying for each filter statement. For example, if you are searching for any project that contains the phrase "new project" in the name, <span>Workfront</span> does not display projects that have just "new" or just "project", or "new main project" in the name. The filter finds only projects with the exact phrase "new project" in the name.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">cieq</span> </p> </td> 
   <td> <p>(Case insensitive) This is the case insensitive option of <span class="bold">eq</span>. It only returns an exact match of the searched value.</p> <p>For example, when searching for a task with a specific name, "task name cieq test" finds tasks where the name is "Test", "TEST", or "Test", but it does not find a task with the name "test 123."</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">ciin</span> </p> </td> 
   <td> <p>(Case insensitive) This is the case insensitive version of <span class="bold">in</span>.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">cilike</span> </p> </td> 
   <td> <p>This is the case insensitive version of <span class="bold">like</span>. For example: "cilike %Current% %Dead%" returns any notes that contain "Current to Dead" or "current to dead".</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">cinotin</span> </p> </td> 
   <td> <p>(Case insensitive) This is the case insensitive version of <span class="bold">notin</span>.</p> <p>This modifier can only be used in text mode filters. For more information about creating filters using text mode, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td>&nbsp;</td> 
   <td> <p><span class="bold">contains</span> </p> </td> 
   <td> <p>(Case sensitive) Searches for the specified text throughout an entire text string.</p> <p>For example, using "contains Inf" captures anything with "Inf" in it, such as the word "Infinity."</p> <p>This modifier can only be used in text mode filters.For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Does Not Contain</span> </p> </td> 
   <td> <p><span class="bold">cinotcontains</span> </p> </td> 
   <td> <p>(Case insensitive) It filters for items that are missing the value specified.</p> <p>For example, "does not contain inf" captures anything without "Inf" or "inf" in the name.</p> <p>Note: <span>If the field you are filtering for has multiple options, this filters out the results that contain both the choice you specify, as well as the choice you specify and any additional choices.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><span class="bold">Does Not Exist</span> </td> 
   <td><span class="bold">NOTEXISTS</span> </td> 
   <td> <p>This modifier is used only with complex filters in an EXISTS statement. These filters refer only to the following objects: </p> 
    <ul> 
     <li>Objects that span multiple levels in the object hierarchy </li> 
     <li>Objects that are missing </li> 
    </ul> <p>For information about creating complex filters using EXISTS statements see the article <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Create Complex Text-Mode Filters Using EXISTS Statements</a>. This is the only modifier used in EXISTS statements.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><span class="bold"> Equal</span> </p> </td> 
   <td> <p><span class="bold">in</span> </p> </td> 
   <td> <p>(Case sensitive) This modifier allows you to create a comma-separated list of variables to compare to a single attribute evaluated in a filter. The entire list is treated as an OR statement and returns any results that meet the criteria of one or more of the variables.</p> <p>For example, when searching for projects, using "in CUR, PLN, CPL" returns all projects that are in the Current, OR Planning, OR Complete status.</p> <p>The built-in modifier <span class="bold">Equal</span> corresponds to the text mode modifier of <span class="bold">in</span>. This means that you can choose Equal with multiple values for the field.</p> <p>For example, you are able to choose a "Status equals Current, Planning, Dead" in a project report and you can view projects in any of these statuses.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><span class="bold">eq</span> </p> </td> 
   <td> <p>(Case sensitive) This returns only an exact match of the searched value.</p> <p>For example, when searching for complete projects, "eq CPL" returns all projects in the complete status. "eq CPL, CUR" does not return a result because a project cannot be complete and current at the same time.</p> <p>This modifier can only be used in text mode filters. For more information about using text mode to create filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Greater Than</span> </p> </td> 
   <td> <p><span class="bold">gt</span> </p> </td> 
   <td> <p>This searches for all results with a value greater than the value entered, not including the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">like</span> </p> </td> 
   <td> <p>(Case sensitive) Searches for portions of a text string in similar fashion to <span class="bold">contains</span>. However, <span class="bold">like</span> provides the ability to insert wild card characters to break up the text.</p> <p>For example, when searching for notes, using "like %Current% %Dead%" returns any note that contains the phrase "Current to Dead". It does not include any notes that contain "Dead to Current". Each value is searched in the order it is listed. The % represents a wild card to replace characters or segments of text.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Less Than</span> </p> </td> 
   <td> <p><span class="bold">lt</span> </p> </td> 
   <td> <p>This searches for all results with a value less than what is entered, not including the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Greater Than Equal</span> </p> </td> 
   <td> <p><span class="bold">gte</span> </p> </td> 
   <td> <p>This searches for all results with values greater than or equal to the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Less Than Equal</span> </p> </td> 
   <td> <p><span class="bold">lte</span> </p> </td> 
   <td> <p>This searches for all results with a value less than or equal to the entered value.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Between</span> </p> </td> 
   <td> <p><span class="bold">between</span> </p> </td> 
   <td> <p>Provides two required field values and searches for all results within range of both fields including the entered values.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">notcontains</span> </p> </td> 
   <td> <p>(Case sensitive) It filters for items that are missing the value specified.</p> <p>For example, "notcontains inf" captures anything with without "inf", but it displays values that contain "Inf."</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><span class="bold">notbetween</span> </p> </td> 
   <td> <p>This is the inverse of <span class="bold">between</span>. It provides two required value fields and searches for all results outside the range of both fields including the entered values.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><span class="bold">Not Equal</span> </p> </td> 
   <td> <p><span class="bold">notin</span> </p> </td> 
   <td> <p>(Case sensitive) This is the opposite of <span class="bold">in</span>. It returns only results not in the specified list.</p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> <p>Note: <span>If the field you are filtering for has multiple options, this filters out the results that contain both the choice you specify, as well as the choice you specify and any additional choices.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td>&nbsp;</td> 
   <td><span class="bold">ne</span> </td> 
   <td> <p>(Case sensitive) This is the opposite of <span class="bold">eq</span>. It returns only results that are not an exact match of the searched value, and it also matches the case of the value.</p> <p>For example, <b>ne</b> returns any values that do not equal "Current", but it does not return any values that do not equal "current". </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td>&nbsp;</td> 
   <td><span class="bold">cine</span> </td> 
   <td> <p>(Case insensitive) This is the case insensitive option of <span class="bold">ne</span> and it is the opposite of the <b>cieq</b> modifier. It only returns results that are not an exact match of the searched value, not taking in account the case of the value.</p> <p>For example, <b>cine</b> returns any values that do not equal either "current" or "Current". </p> <p>This modifier can only be used in text mode filters. For more information about text mode in filters, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

