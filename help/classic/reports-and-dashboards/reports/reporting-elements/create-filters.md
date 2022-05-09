---
filename: create-filters
product-area: reporting
navigation-topic: reporting-elements
title: Create or edit filters in Adobe Workfront
description: "(NOTE: ***IMPORTANT: this DIV will need to be drafted/ hidden when the following DIV (that includes new filters) will be live)"
---

# Create or edit filters in Adobe Workfront

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

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

[ ![](assets/video-create-filters-350x198.png)](https://workfront-video.wistia.com/medias/5iz0l6s4o0)

## How-to steps

1. Go to a list or a report that contains the filter that you want to customize.
1. Click the **Filter** drop-down list.

   ![](assets/screen-shot-2013-09-05-at-9.55.17-am-350x481.png)

1. 
   Click **New Filter** at the bottom of the list of filters

   Or

   Select the filter that you want to customize, then click on the drop-down list again and click **Customize Filter**.
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

   ![](assets/filter-remove.png)

   The My Filters dialog box is displayed.

   All filters that you have rights to remove are available to remove. Other filters are displayed as dimmed.

1. Click the (**x**) next to any filters you want to remove, then click **Done**.

## Additional information

See also:

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Classic,QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> (link is not working anymore - drafted)</li>
  -->

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
<h2><a name="Create"></a>Create or edit a filter </h2> <!--
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
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Classic">Click the <strong>Filter</strong> drop-down list.</p> <note type="tip">
The report creator must allow for filters to be edited in order to view the&nbsp;Filter drop-down list on a report. The Report Default filter is applied to a report by default. The Report Default filter can be customized only when you edit the report.
</note> <p> <img src="assets/screen-shot-2013-09-05-at-9.55.17-am-350x481.png" alt="" style="width: 350;height: 481;" data-mc-conditions="QuicksilverOrClassic.Classic"> </p> </li>
<li value="3">
<div data-mc-conditions="QuicksilverOrClassic.Classic">
<p>Click <strong>New Filter</strong> at the bottom of the list of filters</p>
<p>Or</p>
<p>Select the filter that you want to customize, then click on the drop-down list again and click <strong>Customize Filter</strong>.</p>
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
</div>
-->

&nbsp;
