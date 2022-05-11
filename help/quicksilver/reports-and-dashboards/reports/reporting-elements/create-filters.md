---
filename: create-filters
product-area: reporting
navigation-topic: reporting-elements
title: Create or edit filters in Adobe Workfront
description: Create or edit filters in Adobe Workfront
---

# Create or edit filters in Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***IMPORTANT: this DIV will need to be drafted/ hidden when the following DIV (that includes new filters) will be live)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: all screen shots and steps will have to be reviewed for the new filters because this was updates in 2021 and filters have had additional changes in functionality and UI since then)</p>
-->

You can use filters to reduce the amount of information you display on the screen. Filters display in various areas of Adobe Workfront. The information in this article refers to filters in lists of objects. For more information about filters, see [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add information here about modifying and copying existing filters as a way of creating new filters!) </p>
-->

You can apply the following types of filters in&nbsp;a list of objects:

* A quick filter to a list of objects to find an item in a list using a keyword.

  For information about quick filters, see [Apply the quick filter to a list](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

* A permanent filter that you can use numerous time on multiple lists and reports. This article describes how to create a permanent filter or edit an existing one.

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
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to create a filter in a report</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to create or edit a filter in a report</p> <p>Manage permissions to a filter to edit it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Walk-through

View the following video to learn how to create a filter.

This video was recorded in Adobe Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![](assets/video-create-filters-350x198.png)](https://workfront-video.wistia.com/medias/5iz0l6s4o0)

## How-to steps

1. Go to a list or a report that contains the filter that you want to customize.
1. Click the **Filter** icon ![](assets/filter-nwepng.png). 
1. 
   Click **New Filter** at the top of the list of filters

   Or

   Hover over the filter you want to modify and click the **Edit** icon ![](assets/edit-icon.png). 
   The interface builder for customizing the Filter launches.

1. Do any of the following:

   * Modify existing filter rules by clicking the existing rule and selecting a new option.
   * Add a filter rule by clicking **Add another Filter Rule**, begin typing the name of the option for which you want to add a rule in the **Start typing field name** box, then click it when it appears in the drop-down list.

     Fields associated with the object of your filter are listed in the **Start typing field name** box. 
   
   * Click **AND** or **OR** when adding a new filter rule.  
     When adding filter rules, use the filter modifiers to establish the condition of your filter. For more information about filter modifiers, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

     >[!NOTE]
     >
     >When you connect a group of AND&nbsp;statements by multiple OR statements, you must repeat the fields that are not changing between the OR statements for each group of statements. 
     >
     >
     >![](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-350x163.png)     >
     >

     >
     >When you build a filter for tasks that contain the word "marketing" and are in projects with a status of Current or Planning, you must have the following filter rules:
     ><pre>Task: Name Contains Marketing</pre><pre>AND</pre><pre>Project: Status Equals Current</pre><pre>OR</pre><pre>Task: Name Contains Marketing</pre><pre>AND</pre><pre>Project:&nbsp;Status Equal Planning</pre>Although Task: Name Contains "marketing" does not change between the two AND filter groups, it must be repeated in the second group.

   * Delete an existing filter rule by clicking the 'X' icon.

1. (Optional) Click **Switch to Text Mode** to add a filter using the Text Mode interface.

   For more information about creating a filter using the text mode interface, see [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md). 

1. Click **Save Filter** to replace the current Filter with your changes.
1. (Optional) If you no longer want to display a filter in the **Filter** drop-down menu, click **Remove Filter**.

   The My Filters dialog box is displayed.

   All filters that you have rights to remove are available to remove. Other filters are displayed as dimmed.

1. Click the (**x**) next to any filters you want to remove, then click **Done**.

## Additional information

See also:

* [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) 
* [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md) 
* [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md) 
* [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md) 
* [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md) 
* [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)

&nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters will be replaced, this will replace the content at the top; both the top content and everything starting here are in separate DIV sections to make it easier to condition and undrafte, etc.) </p>
-->
<p>You can limit the amount of information you display on the screen in a list of items with a filter. You can define certain criteria based on particular pieces of information about an object and only display those objects that meet those criteria.</p>
<p>You can apply the following types of filters in&nbsp;Adobe Workfront: </p>
<ul>
<li> <p>Quick filters in a list of objects to find an item using a keyword. These are temporary filters that you cannot save for future use. </p> <p>For information about quick filters, see <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Apply the quick filter to a list</a>. </p> </li>
<li> <p>Permanent filters that you can save and use numerous time on multiple lists and reports. This article describes how to create a permanent filter or edit an existing one in a list or report. </p> </li>
<li> <p>Filters in other areas of Workfront, outside of lists and reports. </p> <p>For a list of all filters in&nbsp;Workfront and the areas where you can apply them, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>. </p> </li>
</ul>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
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
<td> <p>Request or higher</p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to&nbsp;Filters, Views, and Groupings</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to a filter</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Types of filter-building interfaces</h2>
<p>You can create filters using the types of filter builders described in the table below: </p>
<table cellspacing="15">
<col>
<col>
<col>
<tbody>
<tr>
<td>Builder type</td>
<td> <p>Filter object</p> <p>&nbsp;</p> </td>
<td>Where available</td>
</tr>
<tr>
<td><b>Standard builder</b> </td>
<td>All objects </td>
<td>Lists and reports</td>
</tr>
<tr data-mc-conditions="">
<td><span class="preview" style="font-weight: bold;">Beta builder</span> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the Beta builder text is also in yellow)</p>
--> </td>
<td>
<div class="preview">
<ul>
<li> <p>Projects</p> </li>
<li> <p>Tasks </p> </li>
<li> <p>Issues</p> </li>
</ul>
</div> </td>
<td>
<div class="preview">
<ul>
<li> <p>Lists </p> </li>
</ul>
<ul>
<li> <p>The Projects list in the Scenario Planner</p> <p>The Scenario Planner is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Scenario Planner overview</a>. </p> </li>
</ul> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Requests area (NOTE: verify this with Vazgen - not sure if this will come out now???)</p>
-->
</div> </td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<td colspan="2"> <note type="note">
<span class="preview">Beta builders for filters are not available in reports.</span>
</note> </td>
</tr>
</tbody>
</table>
<p>For information about Workfront objects, see <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. </p>
</div>
<p><strong>Create or edit a filter  in the standard builder </strong></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: second part of the title, NWE only)</p>
-->
<div>
<p>You can create filters in lists and reports in the following ways:</p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: keep this?? this sort of applies to both this UI and the beta!)</p>
-->
<ul>
<li> <p>From scratch</p> </li>
<li> <p>Edit an existing filter and save it as a new filter</p> </li>
</ul>
</div>
<p>Regardless of the method you use to create filters, creating a filter from scratch or from an existing filter is similar. </p>
<ol>
<li value="1"> <p>Go to a list or a report where you want to create a filter or that contains the filter that you want to customize.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Filter</strong> icon <img src="assets/filter-nwepng.png">. </p> <note type="tip">
The report creator must allow for filters to be edited in order to view the&nbsp;Filter drop-down list on a report. The Report Default filter is applied to a report by default. The Report Default filter can be customized only when you edit the report.
</note> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/filter-drop-down-expanded-nwe-350x904.png" style="width: 350;height: 904;"> </p> </li>
<li value="3">
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>New Filter</strong> at the top of the list of filters</p>
<p>Or</p>
<p>Hover over the filter you want to modify and click the <strong>Edit</strong> icon <img src="assets/edit-icon.png">. </p>
</div> <p>The builder for customizing the filter opens. </p> </li>
<li value="4">Do any of the following:<br>
<ul>
<li><p>Modify existing filter rules by clicking the existing rule and selecting a new option.</p></li>
<li><p>Add a filter rule by clicking <strong>Add another Filter Rule</strong>, begin typing the name of the option for which you want to add a rule in the <strong>Start typing field name</strong> box, then click it when it appears in the drop-down list. </p><p>Fields associated with the object of your filter are listed in the <strong>Start typing field name</strong> box. </p></li>
<li><p>Click <strong>AND</strong> or <strong>OR</strong> when adding a new filter rule.<br>When adding filter rules, use the filter modifiers to establish the condition of your filter. For more information about filter modifiers, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</p> <note type="note">  
<p>When you connect a group of AND&nbsp;statements by multiple OR statements, you must repeat the fields that are not changing between the OR statements for each group of statements. </p>
<p><img src="assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-350x163.png" style="width: 350;height: 163;"></p>
<div class="example" data-mc-autonum="<b>Example: </b>">  
<p>When you build a filter for tasks that contain the word "marketing" and are in projects with a status of Current or Planning, you must have the following filter rules:</p>
<pre>Task: Name Contains Marketing</pre>
<pre>AND</pre>
<pre>Project: Status Equals Current</pre>
<pre>OR</pre>
<pre>Task: Name Contains Marketing</pre>
<pre>AND</pre>
<pre>Project:&nbsp;Status Equal Planning</pre>
<p>Although Task: Name Contains "marketing" does not change between the two AND filter groups, it must be repeated in the second group. </p>
</div>
</note></li>
<li>Delete an existing filter rule by clicking the 'X' icon.</li>
</ul></li>
<li value="5"> <p>(Optional) Click <strong>Switch to Text Mode</strong> to add a filter using the Text Mode interface.</p> <p>For more information about creating a filter using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>. </p> </li>
<li value="6"> <p>Click <strong>Save Filter</strong> to create a new filter or replace the selected one with your changes.</p> <p>Or</p> <p>Click <strong>Save as New Filter</strong> to create a new filter from the selected one. </p> <p>The new filter displays in the list of filters and it is automatically applied to the list or report you selected.</p> </li>
<li value="7"> <p>(Optional) Do one of the following:</p>
<ul>
<li> <p>Share filters you create with other users, or make them available system-wide. For information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md" class="MCXref xref">Share a filter, view, or grouping </a>. </p> </li>
<li> <p>Remove filters you no longer want to display in the list. For information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md" class="MCXref xref">Remove filters, views, and groupings</a>. </p> </li>
</ul> </li>
</ol>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2><a name="Create2"></a>Create or edit a filter in the beta builder</h2> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: yellow div and it stays NWE only)</p>
-->
<div>
<p>Consider the following when creating filters using the different interfaces:</p>
<ul>
<li> <p>You can find the beta builder in the same places you find the standard filter interface for the areas listed in the table above. </p> </li>
<li> <p>You can switch back and forth between the standard and the beta builder interface, where the beta option is available. </p> </li>
<li> <p>After you have enabled the beta builder in one area, it is the default experience for all areas where it is available. For example, if you enable the beta builder in a project list, it is the default experience for building task and issue filters in lists as well. </p> </li>
<li> <p>You can create filters using the beta builder interface in project, task, and issue lists in the following ways:</p>
<ul>
<li> <p>From scratch</p> </li>
<li> <p>Edit an existing filter </p> </li>
<li> <p>Duplicate an existing filter</p> </li>
<li> <p>Duplicate an existing filter, edit it, and save it as a new filter </p> </li>
</ul> </li>
<li> <p>Saved filters are available in both builders, regardless of which experience you used to originally build them. For example, if you created a filter using the standard builder, you can find and modify it in the beta builder interface as well.</p> </li>
<li> <p>The standard and beta builders have a slightly different syntax when building multiple-statement filters that combine the AND and OR operators. As a result, these filters may display differently when you switch from one builder to another. </p>
<div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span>
<p>The following scenario exists: </p>
<ol>
<li value="1"> <p>Use the beta builder to create a filter that has the following syntax:</p> <p><code>(A OR&nbsp;B) AND&nbsp;C</code> </p> </li>
<li value="2"> <p>Switch back to the standard builder and edit the filter using the syntax of the standard builder as described in the <a href="#create-or-edit-a-filter-in-the-standard-builder" class="MCXref xref">Create or edit a filter in the standard builder</a> section in this article. The syntax for the standard builder displays the filter statements as follows:</p>
<div>
<pre>A AND C</pre>
<pre>OR</pre>
<pre>B AND C</pre>
</div> </li>
<li value="3"> <p>Make a change to the filter in the standard interface. </p> </li>
<li value="4"> <p>Switch back to the beta builder. The filter statement displays according to the logic supported in the standard builder, as described in Step b. <!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: ensures this stays correct over time)
</MadCap:conditionalText>
--></p> <p>The filter displays in the beta builder interface as follows: </p>
<div>
<pre>A AND C</pre>
<pre>OR</pre>
<pre>B AND C</pre>
</div> <p>This happens because the filter was modified in the standard interface. </p> </li>
</ol>
</div> </li>
</ul>
</div>
<ol>
<p>Create a filter using the beta builder interface: </p>
<li value="1">Go to a project, task, or issue list where you want to create a filter or that contains the filter that you want to customize.</li>
<li value="2"> <p>Click the <strong>Filter</strong> icon <img src="assets/filter-nwepng.png">, then enable the <strong>Beta setting</strong> <img src="assets/beta-toggle-white-on-existing-filters.png"> to access the beta builder. It is disabled by default. </p> <p>This opens the beta filter builder interface. </p> <note type="tip">
The header of the filter builder interface changes to blue when you enable the beta builder. After you enabled the beta builder interface, Workfront keeps it enabled for all areas where it is available.
</note> <p> <img src="assets/new-filters-my-filters-suggested-shared-filter-lists-nwe-350x234.png" style="width: 350;height: 234;"> </p> </li>
<li value="3"> <p>Review the following lists of filters:</p>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">My filters</td>
<td>Filters that you build and saved yourself.</td>
</tr>
<tr>
<td role="rowheader">Suggested</td>
<td>Filters that the Workfront administrator adds to your list of filters, either at the system level, or in your Layout Template. </td>
</tr>
<tr>
<td role="rowheader">Shared with me</td>
<td>Filters that others create and share with you or that are shared system-wide.</td>
</tr>
</tbody>
</table> </li>
<li value="4"> <p>Do one of the following:</p>
<ul>
<li> <p>Click <strong>New filter</strong> to create a filter from scratch</p> </li>
</ul>
<ul>
<li> <p>Hover over an existing filter that you have permissions to manage and click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> to edit an existing filter. </p> <p>Or</p> <p>Hover over an existing filter that you have permissions to manage and click&nbsp;<strong>Duplicate</strong> to copy the existing filter and edit a copy. </p> </li>
</ul> <p> <img src="assets/new-filters-more-menu-options-wb-nwe.png"> </p> </li>
<li value="5"> <p>(Conditional) Depending on whether you want to find objects that match all or any of the statements in a filter group select from the following options: </p>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Include if all are true</td>
<td>The objects found by the filter must match all filter criteria in a filter group. In this case, the filter statements are connected by the AND&nbsp;operator. This is the default selection. </td>
</tr>
<tr>
<td role="rowheader">Include if any are true</td>
<td>The objects found by the filter must match any filter criteria in a filter group. In this case, the filter statements are connected by the OR&nbsp;operator.</td>
</tr>
</tbody>
</table> <p> <img src="assets/new-filters-all-or-any-are-true-drop-down-menu-nwe-350x190.png" style="width: 350;height: 190;"> </p> <p>For more information about filter operators, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>. </p> </li>
<li value="6"> <p>Start typing the name of a field, then select it when it displays in the list. You can also select <strong>Search all fields</strong> to view a list of all fields to filter by. The fields in the advanced search are grouped by object category.</p> </li>
<li value="7"> <p>Click the modifier drop-down menu to select a modifier. The default modifier is "Equals." </p> <p>For more information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>. </p> <note type="tip">
As you build the filter, the results appear immediately in the list.
</note> </li>
<li value="8"> <p>Start typing the value of a field you want to filter by. For example, start typing the name of an issue, if you want to filter by<code> Issue:Name</code>. Select the value when it displays in the list. </p> <note type="tip">
Depending on what modifier you selected, you can select multiple values.
</note> </li>
<li value="9"> <p>Click&nbsp;<strong>Add filter</strong> to select another field and add a new filtering criteria to the filter statement. </p> </li>
<li value="10"> <p>(Optional)&nbsp;Click the <strong>Delete</strong> icon <img src="assets/delete.png"> to remove existing filter statements.</p> <p>Or</p> <p>Click <strong>Clear all</strong> to clear all filtering criteria. </p> </li>
<li value="11"> <p>(Optional)&nbsp;Click <strong>Add filter group</strong> to add another set of filtering criteria.</p> <note type="tip">  
<p>You might want to user another filter group when you want the groups to be connected by a different operator than the operator in a filter statement. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">  
<p>When you filter for project that contain "marketing" in the name that are either not complete and are not On Hold, you can use the following multiple filter groups: </p>
<p><code>(Project: Name Contains Marketing AND&nbsp;Project:&nbsp;Percent Complete Does not equal 100) </code> </p>
<p><code>OR&nbsp;</code> </p>
<p><code>(Project: Name Contains Marketing AND&nbsp;Project: Status Does not equal On&nbsp;Hold)</code> </p>
<p>In this case, each filter statement is connected by an AND and the filter groups are connected by an OR. </p>
</div>
</note> </li>
<li value="12"> <p>(Optional)&nbsp;Click <strong>Text mode</strong> to continue building the filter using text mode. </p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: update shot below!)</p>
--> <p> <img src="assets/text-mode-option-create-filter-nwe-350x253.png" style="width: 350;height: 253;"> </p> <p>The text mode interface opens. </p> <p> <img src="assets/text-mode-interface-for-beta-filters-nwe-350x324.png" style="width: 350;height: 324;"> </p> <note type="tip">
We recommend building as much of the filter as possible using the beta builder interface and only using text mode when you must make modifications to the filter that are only supported in text mode.
</note> <p>For more information about creating a filter using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Edit a filter using text mode</a>. </p> </li>
<li value="13"> <p>(Optional) Click <strong>Exit text mode</strong> to return to the beta builder interface. </p> <note type="warning">
Some text mode statements are not supported in the beta builder or the standard interface. Exiting text mode when you have created these types of statements might generate a warning message.
</note> </li>
<li value="14"> <p>(Optional)&nbsp;Click <strong>Apply</strong> to apply the filter to the list and see the results.</p> <p>The number of filter statements including filter groups that you selected displays next to the filter icon at the top of the list.</p> <p> <img src="assets/new-filters-number-of-filters-selected-wb-nwe.png"> </p> </li>
<li value="15"> <p>Click&nbsp;<strong>Save as new</strong> to save the filter for future use. </p> <p> <img src="assets/save-as-untitled-filter-ui-nwe-350x348.png" style="width: 350;height: 348;"> </p> </li>
<li value="16"> <p>Select <strong>Untitled Filter</strong> and enter the name of the new filter instead. </p> </li>
<li value="17"> <p>Select an icon for the new filter from the <strong>Icon</strong> drop-down menu. </p> <p> <img src="assets/new-filters-select-icon-expanded-drop-down-wb.png"> </img> </p> </li>
<li value="18"> <p>(Optional) Add a description for the filter to indicate what is unique about it. The description displays under the filter name in the list of filters. </p> <note type="tip">
Clicking
<strong>Cancel</strong> at any time takes you back to the filter building area.
</note> </li>
<li value="19"> <p>Click&nbsp;<strong>Save</strong>. The filter is saved in the My filters list and is applied to the list of items.</p> </li>
<li value="20"> <p> (Optional) Select another filter to apply it in addition to the new filter you just created. </p> <note type="tip">  
<ul>
<li> <p>There is no limit to the number of filters you can select.</p> </li>
<li> <p>When you select multiple filters all their conditions must be met simultaneously to display matching results.</p> </li>
</ul>
</note> <p> <img src="assets/new-filters-apply-multiple-filters-350x335.png" style="width: 350;height: 335;"> </p> <p>The number of filters you selected displays next to the filter icon at the top of the list of items.</p> <p> <img src="assets/new-filters-number-of-filters-selected-wb-nwe.png"> </img> </p> </li>
<li value="21"> <p>(Optional) Do one of the following:</p>
<ul>
<li> <p>Share the filter with others, or make it available system-wide. For more information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md" class="MCXref xref">Share a filter, view, or grouping </a>.</p> </li>
<li> <p>Delete the filter if it is no longer valid or a duplicate.&nbsp;For information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/delete-filters.md" class="MCXref xref">Delete filters</a>. </p> </li>
</ul> </li>
</ol>
</div>
</div>
-->

&nbsp;
