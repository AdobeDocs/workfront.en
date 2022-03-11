---
filename: reference-collections-report
product-area: reporting
navigation-topic: text-mode-reporting
title: Reference collections in a report
description: Building a report in Adobe Workfront allows you to display a set of objects, their respective fields, or linked objects in a list, a grid, or a chart format.
---

# Reference collections in a report

Building a report in Adobe Workfront allows you to display a set of objects, their respective fields, or linked objects in a list, a grid, or a chart format.

For more information about building a report in Workfront, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>Manage permissions to a view, filter, or grouping </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Understand collections

A collection is a list of objects that are linked to another object.

You have the following two relationships between objects in Workfront:

* `A one-to-one relationship`: One object can be linked to only one other object at a time.  
  For example, a project can only be linked to one portfolio at a time.

* `A one-to-many relationship`: One object can be linked to several other objects at a time.  
  For example, a project can have multiple tasks. In this case, the list of tasks forms a collection for the project.

>[!IMPORTANT]
>
>You can build a report showing the one-to-one relationship between objects by using the standard report builder. However, you can only build a report showing the one-to-many relationship between objects by using the text mode interface in the report builder.

For more information about building a report in the standard report builder, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

For more information about building a report using the text mode interface, see:

* [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md) 
* [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Find collection objects and their fields in the API Explorer

Not all collections can be reported on.

To understand what objects can be associated with a collection of other, you must use the API Explorer.  
For more information about the API Explorer table, see the [API Explorer](../../../wf-api/general/api-explorer.md).

To find out what collections can be reported on:

<ol> 
 <li value="1"> Go to the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </li> 
 <li value="2"> Find the object of your report. </li> 
 <li value="3"> Select the <span class="bold">collections</span>&nbsp;tab.<br> <note type="note">  Only the objects listed on this tab can be represented as a collection in a report for the object you selected. 
  </note></li> 
 <li value="4"> Expand the object of your collection by clicking it. </li> 
 <li value="5"> Click the link displayed to go to the object of your collection.<br>This opens the <span class="bold">fields</span> tab for the object of your collection.<br> <note type="note">  Only the fields listed on this tab can be referenced in the collection report, or the fields associated with objects listed on this tab. 
  </note></li> 
</ol>

## Reference collections in reports

You can reference objects from a collection in the following reporting elements:

* Views
* Filters
* Prompts

You cannot reference objects from a collection in the following reporting elements:

* Groupings
* Chart

For example, you could reference the task or issue collections from a project report, to show task or issue information&nbsp;at the project level.

* [Reference a collection in the View of a report](#referencing-a-collection-in-the-view) 
* [Reference a collection in the Filter of a report](#referencing-a-collection-in-a-filter) 
* [Reference a collection in the custom prompt of a report](#referencing-a-collection-in-the-custom-prompt)

### Reference a collection in the View of a report

You can reference a collection of objects in the view of a report, to show attributes of objects associated with the object of the report.

For example, you can show task or issue information in a project report, by building a collection column for tasks or issue in the view of the report.

You can display information about the tasks or issues, like names, dates, primary assignees, percent complete, etc in the collection view.

The view displays task or issue information in a list format, with every line of the list representing information about a task or an issue. The list of tasks or issues and their fields appears on the same line as the project the tasks or issues belong to.  
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Add a collection column in a report View](#adding-a-collection-column-in-a-report) 
* [Understand the lines of a collection View in Text Mode](#understanding-the-lines-of-a-collection-view-in-text-mode) 
* [Limitations of a collection View](#limitations-of-a-collection-view)

#### `Add a collection column in a report View`

To add a collection column in a report view:

<ol> 
 <li value="1"> Click the Main menu , then click Reports. </li> 
 <li value="2">Click <span class="bold">New Report</span>.</li> 
 <li value="3">Select the object of your report.</li> 
 <li value="4">Navigate away from your report, and using the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>, determine what collections are available for the object you selected for your report.<br>For more information about selecting the object of your collection, see the section <a href="#finding-collection-objects-and-their-fields-in-the-api" class="MCXref xref">Find collection objects and their fields in the API Explorer</a> in this article.<br>Make a note of what the name of the object for the collection is.<br></li> 
 <li value="5"> Using the&nbsp;<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>, go to the list of fields for the object you want to display in the collection.<br>For more information about finding the fields of the object of your collection, see the section <a href="#finding-collection-objects-and-their-fields-in-the-api" class="MCXref xref">Find collection objects and their fields in the API Explorer</a> in this article.<br> Make a note of what the name of the field you want to display in the collection is. </li> 
 <li value="6"> Navigate back to your report, and in the <span class="bold">Columns (View)</span> tab, click <span class="bold">Add Column</span>. </li> 
 <li value="7">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="8">Mouse over the dialog box, and click <span class="bold">Click to edit text</span>.</li> 
 <li value="9">Select all text in the <span class="bold">Text Mode</span> dialog box and remove it, then paste the following code if you are referencing a field of&nbsp;the collection object:<br><pre>valueformat=HTML<br>textmode=true<br>type=iterate<br>listdelimiter=<p><br>displayname=<span class="bold">Column Name<br></span>listmethod=nested(<span class="bold">collection object name</span>).lists<br>valuefield=<span class="bold">collection object field</span></pre></li> 
 <li value="10">Replace <span class="bold">Column Name</span> with the name of your column in the <code>displayname</code> line.</li> 
 <li value="11">Replace <span class="bold">collection object name&nbsp;</span>with the name of your collection object in the <code>listmethod</code> line, as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</li> 
 <li value="12"> <p>Replace <span class="bold">collection object field</span> with the name of the field of your collection object in the <code>valuefield</code> line, as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p> You can replace <span class="bold">valuefield</span> with <span class="bold">valueexpression</span>, if you want to create a custom expression in your view.<br>For more information about calculated custom expressions, see <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Calculated data expressions</a>.</p> <p>For example, if you want to display a list of the tasks in a project report. This collection uses a <code>valuefield </code>line for referencing the names of the tasks.</p> <p>Do one of the following:</p> 
  <ul> 
   <li> <p>Use the following code to build your column:</p> <p><code>valueformat=HTML<br>textmode=true<br>type=iterate<br>listdelimiter=<p><br>displayname=Project Tasks&nbsp;Names<br>listmethod=nested(tasks).lists<br>valuefield=name</code> </p> </li> 
   <li> <p>Use the following code to display a list of issues in the report:</p> 
    <div> <code>displayname=Project Issues Names<br> listdelimiter=<p><br>listmethod=nested(issues).lists<br>textmode=true<br>type=iterate<br>valuefield=name<br>valueformat=HTML</code> 
    </div> <p> Notice that in a collection you must use <span class="bold">issues</span> for the&nbsp;<span class="bold">listmethod</span> line, instead of <span class="bold">opTasks</span> which is the database name for Issues. For information about when to use <span class="bold">issue</span> and when to use <span class="bold">opTask</span> when referring to issues, see <a href="../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md" class="MCXref xref">Use "opTask" and "issue" when referencing issues</a>.</p> </li> 
   <li> <p>If you&nbsp;want to display a list of the tasks in a project report along with their primary assignee, you would use a&nbsp;<span class="bold">valueexpression</span>&nbsp;line for referencing the names of the tasks adjacent to the names of their primary assignees instead of <span class="bold">valuefield</span>.<br>Use the following code to build your column:</p> <p><code>valueformat=HTML<br>textmode=true<br>type=iterate<br>listdelimiter=<p><br>displayname=Tasks&nbsp;Names - Primary Assignee<br>listmethod=nested(tasks).lists<br>valueexpression=CONCAT({name},' - ',{assignedTo}.{name})</code> <br> </p> </li> 
  </ul> </li> 
 <li value="13"> <p>The following column displays in the project report, listing all tasks in each project alongside their primary assignees:</p> <p> <img src="assets/project-report-with-task-and-assignee-collection-view-350x350.png" alt="project_report_with_task_and_assignee_collection_view.png" style="width: 350;height: 350;"> <br> </p> </li> 
 <li value="14">Click <span class="bold">Save</span>.</li> 
 <li value="15"> <p>(Optional) Continue editing the report.<br>Or</p> <p>Click <span class="bold">Save + Close</span> to save the report.</p> </li> 
</ol>

#### `Understand the lines of a collection View in Text Mode`

The lines in a text mode view for a collection are outlined in the following table: 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Sample Line</span> </th> 
   <th><span class="bold">Description</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>You can use various values for this line, but we recommend that the <code style="font-weight: normal;">valueformat</code> for a collection list should be <span class="bold">HTML.</span></p> <p> <!--
      For more information about conditional formatting in a view, see Use conditional formatting in Text Mode.
     --></p> </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>This line indicates that the column has been configured using text mode. If you remove this line, Workfront adds it back by default.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>The <code>type</code> of a list is always <code>iterate</code>, when building a view.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>This is the delimiter which is used to separate the values in&nbsp;your list.<br>We recommend to use <code>&lt;p&gt;</code>&nbsp;which adds a line break between the values.</p> <p>You can also use the following:</p> <p><code>&amp;zwj;</code> (zero-width joiner).&nbsp;The&nbsp;values of the collection have no separation between them.<br><span class="bold">,</span> =comma separator.&nbsp;The values of the collection are separated by a comma followed by no space.<br><span class="bold">/</span> = slash separator.&nbsp;The values of the collection are separated by a slash.<br><span class="bold">-</span> = dash separator. The values of the collection are separated by a dash.<br>Leaving this line empty adds a comma followed by a space between the values of the collection, by default.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Column Name</em> </td> 
   <td> <p>Replace <span class="bold">Column Name</span> with the actual name of your new column.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> This line defines the collection&nbsp;you are referencing.</p> <p>Replace <span class="bold">collection object name</span> with the name of the object you are referencing in your collection, as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. This value is typically the plural form of the collection object name.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>This line defines what field you&nbsp;are referencing from the collection object.</p> <p>Replace&nbsp;<span class="bold">collection object field</span>&nbsp;with the name of the field of the object&nbsp;you are referencing in your collection, as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>You can replace&nbsp;this line with:</p> <p><span class="bold">valueexpression</span>=calculated collection object field/ fields</p> <p>Using <span class="bold">valueexpression</span>, you can &nbsp;display a calculated&nbsp;custom expression in the column.</p> <p>For more information about how to format <span class="bold">valueexpression</span> lines, see <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Text mode syntax overview</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `Limitations of a collection View`

Consider the&nbsp;following limitations when you are building a collection view:

* You cannot control the order in which collection&nbsp;data is displayed.
* You cannot apply conditional formatting to&nbsp;a collection view.
* You cannot make an object in a collection a clickable link.
* You cannot build a collection view of another collection.  
  For example, you cannot display all the assignees on each task in a project report. You can only display the primary assignee on each task in a project view.

### Reference a collection in the Filter of a report

You can reference a collection of objects in the filter&nbsp;of a report, to filter for the&nbsp;attributes of objects associated with the object of the report.

For example, you can filter for task or issue information in a project report by using a reference to the attributes of tasks or issues on the project in the filter statement.

To add a reference to a collection&nbsp;in a report filter:

<ol> 
 <li value="1"> Click the Main menu , then click Reports. </li> 
 <li value="2">Click&nbsp;<span class="bold">New Report</span>.</li> 
 <li value="3">Select the object of your report.</li> 
 <li value="4">Navigate away from your report, and using the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>, determine what collections are available for the object you selected for your report.<br>For more information about selecting the object of your collection, see the section <a href="#finding-collection-objects-and-their-fields-in-the-api" class="MCXref xref">Find collection objects and their fields in the API Explorer</a> in this article.<br>Make a note of what the name of the object for the collection is.<br></li> 
 <li value="5"> Using the&nbsp;<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>, go to the list of fields for the object you want to display in the collection.<br>For more information about finding the fields of the object of your collection, see the section <a href="#finding-collection-objects-and-their-fields-in-the-api" class="MCXref xref">Find collection objects and their fields in the API Explorer</a> in this article.<br> Make a note of the field you want to display in the collection. </li> 
 <li value="6"> Navigate back to your report, and in the <span class="bold">Filters</span>&nbsp;tab, click&nbsp;<span class="bold">Switch to Text Mode</span>.</li> 
 <li value="7">In the <span class="bold">Set Filter Rules for your Report</span> area, paste the following code:<br><pre>collection object name:collection object field=collection object value<br>collection object name:collection object field_Mod=value of the modifier</pre></li> 
 <li value="8">Replace&nbsp;<span class="bold">collection object name</span>&nbsp;with the name of your collection object as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.&nbsp;This value is typically the plural form of the collection object name.</li> 
 <li value="9">Replace&nbsp;<span class="bold">collection object field</span>&nbsp;with the name of the field of your collection object in, as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</li> 
 <li value="10">Replace <span class="bold">collection object value</span> with the value of the collection object as it appears in Workfront.</li> 
 <li value="11">Replace <span class="bold">value of the modifier</span> with a valid modifier.<br>For a list of modifiers, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.<br>For example, to build a project report that&nbsp;displays only projects with tasks that have "Marketing" in their name, use&nbsp;the following code:<br><pre>tasks:name=Marketing<br>tasks:name_Mod=cicontains</pre> This report only displays projects which have at least one&nbsp;task that has the word "marketing" in their name.<br><img src="assets/marketing-only-tasks-in-project-report-350x298.png" alt="marketing_only_tasks_in_project_report.png" style="width: 350;height: 298;"><br>To filter for the name of an issue, use the following code:<br><pre>issues:name=Marketing
issues:name_Mod=cicontains</pre> <note type="important">  Notice that you must use 
   <span class="bold">issues</span> for the collection object name. 
  </note></li> 
 <li value="12">Click&nbsp;<span class="bold">Done</span>.</li> 
 <li value="13"> <p>(Optional) Continue editing the report.<br>Or</p> <p>Click&nbsp;<span class="bold">Save + Close&nbsp;</span>to save the report.</p> </li> 
</ol>

### Reference a collection in the custom prompt of a report

You can reference a collection of objects in the custom prompt&nbsp;of a report, to&nbsp;filter the results of the report for the&nbsp;attributes of objects associated with the object of the report.

For example, you can prompt&nbsp;for task information in a project report by using a reference to the attributes of tasks on the project in the custom prompt of the report.

>[!NOTE]
>
>You cannot reference collections in a standard prompt.

A custom prompt is a custom filter where the statements are joined by&nbsp;ampersand symbols. We recommend that you build your statement in a filter, first, then join the lines of the statements with ampersands.

For more information about building a filter statement with a collection reference, see the section [Reference a collection in the Filter of a report](#referencing-a-collection-in-a-filter) in this article.

To add a reference to a collection&nbsp;in the&nbsp;custom prompt of a report:

<ol> 
 <li value="1"> Click the Main menu , then click Reports. </li> 
 <li value="2">Click&nbsp;<span class="bold">New Report</span>.</li> 
 <li value="3">Select the object of your report.</li> 
 <li value="4">Build a filter with a collection reference as described in&nbsp;the section <a href="#referencing-a-collection-in-a-filter" class="MCXref xref">Reference a collection in the Filter of a report</a> in this article.</li> 
 <li value="5">Click <span class="bold">Report Settings</span>.</li> 
 <li value="6">Click <span class="bold">Report Prompts</span>.</li> 
 <li value="7">Click <span class="bold">Add Prompt</span>.</li> 
 <li value="8">Click <span class="bold">Custom Prompt</span>.</li> 
 <li value="9">Specify the name of the prompt in the&nbsp;<span class="bold">Field</span><span class="bold">name</span> field.</li> 
 <li value="10">Specify a <span class="bold">Dropdown Item Label</span>.</li> 
 <li value="11">Specify the following in the <span class="bold">Condition</span> field:<br><pre>collection object name:collection object field_Mod=value of the modifier</pre></li> 
 <li value="12">(Optional) Specify if this choice is displayed by default in the prompt.</li> 
 <li value="13"> Replace&nbsp;<span class="bold">collection object name</span>&nbsp;with the name of your collection object as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.&nbsp;This value is typically the plural form of the collection object name.</li> 
 <li value="14">Replace&nbsp;<span class="bold">collection object field</span>&nbsp;with the name of the field of your collection object, as it appears in the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</li> 
 <li value="15">Replace&nbsp;<span class="bold">collection object value</span>&nbsp;with the value of the collection object as it appears in Workfront.<br>For example, if you are filtering for projects in which the name of the task contains "Marketing", replace&nbsp;<span class="bold">collection object value</span>&nbsp;with&nbsp;<span class="bold">marketing</span>.</li> 
 <li value="16"> <p>Replace&nbsp;<span class="bold">value of the modifier</span>&nbsp;with a valid modifier.</p> <p>For a list of modifiers, see&nbsp;<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</p> 
  <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
   <p>For example, to build a project report with a custom prompt where you want to display only projects that have at least one task assigned to a specific user, use the code below:<br></p> 
   <p><code>tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in</code> </p> 
   <p>This generates a report where all the projects listed have at least one task assigned to the user whose GUID is&nbsp;57cf1b7a000077c9f02f66cb09c8f86c.</p> <note type="note">
     You cannot reference the name of the primary assignee ("Assigned To" field) of a task, according to the 
    <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. You can only reference the&nbsp;ID of the primary assignee.
   </note> 
   <p>For example, to filter for any projects where any of the project issues are assigned to a specific user use the following code for your custom prompt:</p> 
   <p><code>issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in</code> </p> 
   <p>This generates a report where all the projects listed have at least one issue assigned to the user whose GUID is&nbsp;57cf1b7a000077c9f02f66cb09c8f86c.</p> <note type="note">  Notice that you must use 
    <span class="bold">issues</span> for the collection object name. The API Explorer&nbsp; does not offer a collection object name for issues at this time. 
    <br> 
   </note> 
  </div> </li> 
 <li value="17">Click&nbsp;<span class="bold">Done</span>.</li> 
 <li value="18"> <p>(Optional) Continue editing the report.<br>Or</p> <p>Click&nbsp;<span class="bold">Save + Close</span> to save the report.</p> </li> 
</ol>

