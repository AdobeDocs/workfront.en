---
filename: filters-overview
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Filters overview in Adobe Workfront
description: 
---

# Filters overview in `Adobe Workfront`

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can use filters in  `Adobe Workfront` to reduce the amount of information you display on the screen in lists, reports, or other areas.&nbsp;

>[!NOTE]
>
>This article describes all areas where you can apply filters in  `Workfront`, as well as general information about filters in lists and reports. Refer to the articles linked below to find out information about filters in specific areas other than lists and reports.

## Types of `Workfront` filters

There are several types of filters in `Workfront`. All filters fulfill the same purpose of limiting the amount of information you display on the screen.

The following are types of filters that you can use in  `Workfront`:

<table cellspacing="3"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Temporary filters</td> 
   <td> <p>A one-time quick filter based on a keyword search to quickly find an item in a list. </p> </td> 
  </tr> 
  <tr> 
   <td>Permanent filters for lists and reports</td> 
   <td>Built by <span>Workfront</span> or customized by you or other users. You can use them more than one time. If you have the correct access and permissions, you can name, save, and reuse them in several areas. You can also share these filters with other users. They are available in lists or reports of objects. </td> 
  </tr> 
  <tr> 
   <td>Temporary or permanent filters for special areas</td> 
   <td>Built by <span>Workfront</span> or customized by you or other users. You can save permanent filters and use more than one time, or you can apply them temporarily to serve your immediate needs, without saving them. Unsaved filters cannot be shared or deleted. They are available in special areas, as described in the section <a href="#filters" class="MCXref xref">Workfront filters for special areas</a> in this article. </td> 
  </tr> 
 </tbody> 
</table>

## `Workfront` temporary filters

Quick filters allow you to search for an item on the screen by using a keyword. After you refresh the page, the temporary quick filter is cleared. You cannot save temporary filters to reuse.

For information about quick filters, see [Apply the quick filter to a list](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## `Workfront` permanent filters for lists and reports

You can use permanent filters that you, others, or `Workfront` created in lists or reports of objects.

For information about objects in `Workfront` and which ones you can build reports for, see [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

For more information about filters in lists and reports, see the following articles:

* [Create or edit filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
* [Remove filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md) 
* [Share a filter, view, or grouping in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md) 
* Delete filters

## `Workfront` filters for special areas

You can use either built-in filters or build custom filters in the following areas of `Workfront`:

* Home   
  For information, see the [Filter the Work List](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md#filtering-by-item-type) section in the article [Display items in the Work List in the Home area](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
* Requests area. You cannot customize filters in the Requests area.

  For information, see [Locate submitted requests](../../../manage-work/requests/create-requests/locate-submitted-requests.md). 

* Timesheets. You can use built-in filtering criteria but you cannot build custom filters to reuse for the Timesheets area.

  For information, see [Timesheets overview](../../../timesheets/timesheets/timesheets-overview.md). 

* Resource Planner  
  For information, see the article [Filter information in the Resource Planner](../../../resource-mgmt/resource-planning/filter-resource-planner.md).

* Utilization report

  For information, see the section [Filter utilization information](../../../resource-mgmt/resource-utilization/view-utilization-information.md#filtering-utilization-information) in the article [View resource utilization information](../../../resource-mgmt/resource-utilization/view-utilization-information.md). 

* Resource Scheduling areas  
  For information, see the article [Filter information in the Scheduling area](../../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* `Workload Balancer`

  For information, see [Manage filters in the Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Overview of filters in lists and reports

When working with lists and reports, you can filter information on the screen by using the following types of filters:

* built-in filters

* new filters you or others create from scratch
* customized existing filters that others created and shared with you
* copied and edited filters based on existing filters

>[!IMPORTANT]
>
>When creating or editing filters in reports, you must edit the report in order for the new filter to become the default filter for the report. When you edit just the filter, outside the report builder, the default filter of the report is not updated.  
>For information about editing a report, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

For information about `Workfront` Lists, see the article [Get started with lists in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).  
For information about `Workfront` reports, see the article [Get started with reports in Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md).

Consider the following when working with filters in lists or reports:

* You can customize existing filters in lists and reports. All users who have permissions to the filters can also see your changes.

* Your `Workfront administrator` must grant you access to Edit Filters, Views, and Groupings to create permanent filters.

  For information about granting access to Filters, Views, and Groupings, see [Grant access to filters, views, and groupings](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

<ul> 
 <li> <p>Your level of permissions to a filter determines how filters are saved. If you created the filter originally, you can save the changes, otherwise you are prompted to save a version of the filter that you are modifying.</p> <note type="tip">
   Keep in mind if you make changes to a filter you have shared with others the changes impact them as well.
  </note> </li> 
 <li>You can customize a filter that was shared with you only if the user who shared it granted you Manage access. For information about sharing a filter, see <a href="../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md" class="MCXref xref">Share a filter, view, or grouping in Adobe Workfront</a>.</li> 
</ul>

## Elements of a filter

When you build a filter, you connect multiple elements together that make up filter statements. You can have multiple filter statements that define the criteria for your filter.

A filter contains the following elements:

<table cellspacing="3"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Object</td> 
   <td> <p>The <span>Workfront</span> database object of the filter. For information about what objects are reportable in <span>Workfront</span>, see <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. </p> <p>For example, projects, tasks, issues, users, documents can be the object of a filter. </p> </td> 
  </tr> 
  <tr> 
   <td>Field</td> 
   <td> <p>The attribute of the object that you are filtering by. </p> <p>For example, you can filter by Portfolio Name, or Project Owner. In these case, Name and Owner are fields of the Portfolio and Project objects. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Value</p> </td> 
   <td>The actual name of the field in <span>Workfront</span>.&nbsp;For example, Complete can be the value of a Project&nbsp;Status field. </td> 
  </tr> 
  <tr> 
   <td>Operator</td> 
   <td>Connects multiple filter statements. For information, see the section <a href="#filter" class="MCXref xref">Filter operators</a> in this article. </td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Indicates what kind of information you want your data to match. For information, see the section <a href="#filter2" class="MCXref xref">Filter modifiers</a> in this article. </td> 
  </tr> 
 </tbody> 
</table>

## Filter operators

`Workfront` has 2 filter operators that connect each filter statement:

<ul> 
 <li> <p><span class="bold">AND</span>: When you join 2 filter statement by the AND&nbsp;operator you indicate that you want both filter statements to be met at the same time.</p> 
  <div> 
   <p>By default, the statements in a filter are joined by the AND&nbsp;operator.</p> 
  </div> </li> 
 <li> <p><span class="bold">OR</span>: When you join 2 filter statements by the OR operator you indicate that you want either statement to be met.</p> 
  <div> <note type="tip">
    When changing your AND statements to OR statements, the number of the items in your report should increase.
   </note> 
  </div> </li> 
</ul>

## Filter modifiers

You can use filter modifiers to indicate what kind of information you want your data to match. 

` `**Example: **`` You can filter for projects that have a Percent Complete of 100%. In this case, you can use the "equal" modifier in the following filter statement:

```
Project: Percent Complete Equal(Case Sensitive) 100
```

For more information about filter modifiers, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

## `Create filters in the builder interface`

You can create a filter using the standard builder interface in the following ways:

* From scratch
* Modify an existing filter
* Copy an existing filter

For information about creating a filter using the standard interface, see [Create or edit filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

## Create filters using the text mode interface

You can build filters using the text mode interface. We recommend to build most of the filter statements using the standard interface, and to edit the code of the filter only as a final step. Building a filter from scratch using the text mode interface alone is not recommended.&nbsp;

For more information about creating a filter using the text mode interface, see [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

## `Create filters for complex fields`

* [Create filters for fields whose values contain commas](#filter-for-fields-with-commas) 
* [Create filters for whose values are a multi-select custom field](#filter-for-multi-select)

### `Create filters for fields whose values contain commas`

When building a filter in text mode and filtering for field values that contain commas, you must add a slash ("/") before the commas separating the&nbsp;values, to ensure that the value is read as one filter option. This only applies for the following field types:

* Dropdowns
* Radio Buttons
* Checkboxes

For example, you have a radio button field on a project called "Color" and the options for it are:

* Red
* Blue
* Red, blue

If you want to build a filter that would find only projects where the third option is selected, the filter statement in the text mode interface should be:
<pre>DE:check=red/, blue<br>DE:check_Mod=in</pre>This syntax ensures that the values are read together, as one option. If you omit the slash, `Workfront` reads the comma as an 'OR', in which case only the projects that have either the first or the second option would be selected.&nbsp;

This syntax also applies when building prompts. For more information about using prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

### `Create filters for whose values are a multi-select custom field`

You can report on multi-select custom fields.&nbsp;For example, you can report on fields that are checkboxes.

However, when you want to exclude results that have only one of the options selected, the report will display any objects that have that option and any other option selected.

For example, if you have a field with 3 options (A, B, and C), and select 2 of the 3 options (A and B, but not C) on an object, you can create a report with a filter with a qualifier of Not Equal for options A and B, and it will only filter out projects that have both A and B, but not only A, and not only B selected. If you create a filter with a qualifier for Not Equal for option A, it will only filter out objects with only A selected, but if A and B are selected, those objects still display in the report.

## `Limitations about joining multiple filter rules`

You can reference only five objects, excluding the object of the report, when you build a filter in `Workfront`.&nbsp;

When you reach this limit within the builder, you can select fields that belong only to these six objects. You receive a warning when you have reached this limit.&nbsp;

You cannot overcome this limitation when you build your filter in text mode.&nbsp;

<!--
Filters overview in Adobe Workfront You can use filters in Adobe Workfront to reduce the amount of information you display on the screen. Note: This article describes all areas where you can apply filters in Workfront, as well as general information about filters in lists and reports. Refer to the articles linked below to find out information about filters in specific areas other than lists and reports. Workfront filters There are several types of filters in Workfront. All filters fulfill the same purpose of limiting the amount of information you display on the screen. The following are types of filters that you can use in Workfront: Temporary filters A one-time quick filter based on a keyword search to quickly find an item in a list. Permanent filters Built by Workfront or customized by you or other users that you can use more than one time. If you have the correct access and permissions, you can name, save, and reuse them in several areas. You can also share these filters with other users. Permanent filters You can build filters one time and reuse them in several lists and reports. These are permanent filters. You can create and save permanent filters in the following Workfront areas: Lists Reports Resource Planner For information about filtering in the Resource Planner, see the article Filter information in the Resource Planner. Resource Scheduling areas For information about filtering in the scheduling areas, see the article Filter information in the Scheduling area. Home For information about filtering items in the Home area, see the Filter the Work List section in the article Display items in the Work List in the Home area. Scenario Planner This is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see The Adobe Workfront Scenario Planner overview. Tip: You cannot customize filters in theScenario Planner. You can apply filters to a list of plans, initiatives, or projects in the Scenario Planner. For information, see the following articles: Create and edit plans in the Adobe Workfront Scenario Planner Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner Import projects to plans in the Adobe Workfront Scenario Planner Goals This requires an additional license. For information about Workfront Goals, see Adobe Workfront Goals overview. For information, see Filter information in Adobe Workfront Goals. For information about removing a permanent filter, see the article Remove filters, views, and groupings. Temporary filters You can use a one-time quick filter to quickly jump to an item in a list. This is a temporary filter and you cannot save it. For information about quick filters, see Apply the quick filter to a list. Overview of filters in lists and reports When working with lists and reports, you can customize existing filters, create filters based on existing filters, or create filters from scratch. For information about Workfront Lists, see the article Get started with lists in Adobe Workfront. For information about Workfront reports, see the article Get started with reports in Adobe Workfront. Consider the following when working with filters: You can customize existing filters. All users who can view the filters can also see your changes. Your Workfront administrator must grant you access to Edit Filters, Views, and Groupings to create permanent filters. For information about granting access to Filters, Views, and Groupings, see Grant access to filters, views, and groupings. Your level of permissions to a filter determines how filters are saved. If you created the filter originally, you can save the changes, otherwise you are prompted to save a version of the filter that you are modifying. Keep in mind if you make changes to a filter you have shared with others the changes impact them as well. You can customize a filter that was shared with you only if the user who shared it granted you Manage access. For information about sharing a filter, see Share a filter, view, or grouping in Adobe Workfront. Important: When creating or editing filters in reports, you must edit the report in order for the new filter to become the default filter for the report. When you edit just the filter, outside the report builder, the default filter of the report is not updated. For information about editing a report, see the article Create a custom report. Filter operators Workfront has 2 filter operators that connect each filter statement: AND: When you join 2 filter statement by the AND operator you indicate that you want both filter statements to be met at the same time. By default, the statements in a filter are joined by the AND operator. OR: When you join 2 filter statements by the OR operator you indicate that you want either statement to be met. Tip: When changing your AND statements to OR statements, the number of the items in your report should increase. Filter modifiers You can use filter modifiers to indicate what kind of information you want your data to match. Example: You can filter for projects that have a Percent Complete of 100%. In this case, you can use the "equal" modifier in the following filter statement: Project: Percent Complete Equal(Case Sensitive) 100 For more information about filter modifiers, see Filter and condition modifiers. Create or edit filters in the builder interface You can create a filter using the standard builder interface in the following ways: From scratch Modifying an existing filter Copying an existing filter For information about creating or editing a filter using the standard interface, see the article Create or edit filters in Adobe Workfront. Customize an existing filter Go to the report or list that contains the Filter that you want to customize. Click the Filter drop-down list. Select the Filter that you want to customize, then click Customize Filter. The interface builder for customizing the Filter is launched. Do any of the following: Modify existing filter rules by clicking the existing rule and selecting a new option. Add a filter rule by clicking Add another Filter Rule, begin typing the name of the option for which you want to add a rule, then click it when it appears in the drop-down list. Click AND or OR when adding a new filter rule. When adding filter rules, use the filter modifiers to establish the condition of your filter. For more information about filter modifiers, see the article Filter and condition modifiers. Delete an existing filter rule by clicking the 'X' icon. Click Save Filter to replace the current Filter with your changes. Create a Filter based on an existing Filter Go to the report that contains the Filter that you want to use as the basis for your new Filter. Click the Filter drop-down list. Select the Filter that you want to use as the basis for your new Filter. Click the Filter drop-down list, then click Customize Filter. The interface builder for customizing the Filter is launched. Do any of the following: Modify existing filter rules by clicking the existing rule and selecting a new option. Add a filter rule by clicking Add another Filter Rule, begin typing the name of the option for which you want to add a rule, then click it when it appears in the drop-down list. Click AND or OR when adding a new filter rule. Delete an existing filter rule by clicking the X icon. Click Save as New Filter to save your changes as a new Filter. Create a Filter from scratch Go to the report where you want to create your new report. Click the Filter drop-down list. Click New Filter. The interface builder for customizing the Filter is launched. Do either of the following: Modify existing filter rules by clicking the existing rule and selecting a new option. Add a filter rule by clicking Add another Filter Rule, begin typing the name of the option for which you want to add a rule, then click it when it appears in the drop-down list. Click AND or OR when adding a new filter rule. Delete an existing filter rule by clicking the (x) icon. Click Save Filter. Create filters using the Text Mode interface You can build filters using the text mode interface. We recommend to build most of the filter statements using the standard interface, and to edit the code of the filter only as a final step. Building a filter from scratch using the text mode interface alone is not recommended. For more information about creating a filter using the text mode interface, see Edit a filter using text mode. Create filters for complex fields Create filters for fields whose values contain commas Create filters for whose values are a multi-select custom field Create a filter for fields that contain commas When building a filter in text mode and filtering for field values that contain commas, you must add a slash ("/") before the commas separating the values, to ensure that the value is read as one filter option. This only applies for the following field types: Drop-downs Radio buttons Checkboxes For example, you have a radio button field on a project called "Color" and the options for it are: Red Blue Red, blue If you want to build a filter that would find only projects where the third option is selected, the filter statement in the text mode interface should be: DE:Color=red/, blue DE:Color_Mod=in This syntax ensures that the values are read together, as one option. If you omit the slash, Workfront reads the comma as an 'OR', in which case only the projects that have either the first or the second option would be selected. This syntax also applies when building prompts. For more information about using prompts, see the article Add a prompt to a report. Create a filter for multi-select custom fields You can report on multi-select custom fields. For example, Checkboxes. However, when you want to exclude results that have only one of the options selected, the report will display any objects that have that option and any other option selected. For example, if you have a field with 3 options (A, B, and C), and select 2 of the 3 options (A and B, but not C) on an object, you can create a report with a filter with a qualifier of Not Equal for options A and B, and it will only filter out projects that have both A and B, but not only A, and not only B selected. If you create a filter with a qualifier for Not Equal for option A, it will only filter out objects with only A selected, but if A and B are selected, those objects still display in the report. Limitations about joining multiple filter rules You can reference only five objects, excluding the object of the report, when you build a filter in Workfront. When you reach this limit within the builder, you can select fields that belong only to these six objects. You receive a warning when you have reached this limit. You cannot overcome this limitation when you build your filter in text mode. Removing a Filter from a list You can remove a filter from a list of filters that appears in the Filter drop-down menu in a list. Removing a filter from a list functions differently depending on whether you initially created the filter, or the filter was shared with you. You cannot remove a default filter. If you created the filter and you remove it, the filter is removed from the Workfront system. The filter is no longer available to any users who you previously shared it with. If the filter was shared with you and you remove it, the filter is removed only for you. The user who originally created it and any other users it has been shared with still have access to the filter. To remove a filter: In the Filter drop-down menu, click Remove Filter. The My Filters dialog box is displayed. All filters that you have rights to remove are available to remove. Other filters are displayed as dimmed. Click the (x) next to any filters you want to remove, then click Done.
-->

