---
product-area: reporting
navigation-topic: text-mode-reporting
title: Overview of common uses for Text Mode
description: Overview of common uses for Text Mode
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
---
# Overview of common uses for Text Mode

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

You can expand your reporting capabilities by using text mode in reports and report elements. You can also use a version of text mode to build more complex calculated custom fields. For more information about text mode, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

This article outlines just a few common examples of where you would most likely need to use text mode to expand reporting or calculated custom fields capabilities in Adobe Workfront. For a more expansive list of examples, see:

* [Custom view, filter, and grouping samples: article index](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md) 
* [Calculated custom data in reports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

For more information about creating reports using text mode, including classes, videos, and tutorials, see the Learn section on the Adobe Experience League site. 

## Instances where you might use text mode in lists and reports

We recommend that you use the report and list builder to build your views, filters and groupings. However, there are some instances where you can use text mode to enhance your reports and lists.

You can use text mode when you want to achieve the following in Workfront:

* Build custom calculated custom fields in a custom form.  
  For more information about calculated custom fields, see the [Use Text Mode in calculated custom fields](#use-text-mode-in-calculated-custom-fields) section in this article.
* Enhance filters, views, and groupings beyond what is possible in the report builder. For information about using text mode for filters, views, and groupings, see the following sections in this article:

   * [Use Text Mode in views](#use-text-mode-in-views) 
   * [Use Text Mode in filters](#use-text-mode-in-filters) 
   * [Use Text Mode in groupings](#use-text-mode-in-groupings)

* Create custom prompts. You can only create custom prompts using Text Mode.

  For information about building custom prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Use Text Mode in calculated custom fields {#use-text-mode-in-calculated-custom-fields}

You can use text mode to add a calculated custom field to a Custom Form.

For more information about adding a calculated custom field to a Custom Form, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

For more information about creating a calculated custom field in text mode, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

For example, you can add a calculated custom field that shows a time and date stamp of the moment when an item was marked as In Progress. You can use this calculation for other statuses.

For information, see [Calculated custom field example: display a Status timestamp in a Custom Form](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md).

## Use Text Mode in views {#use-text-mode-in-views}

You can use text mode in views to expand on the fields and objects you can display in the view.

For examples of the most common reasons for using text mode in a view, see the following articles:

* [View: display objects that are not included in the standard interface](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md) 
* [View: display the result of a calculation between two fields in a column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md) 
* [View: permanently edit the width of a column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md) 
* [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md) 
* [View: remove link to an object in a column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md) 
* [Reference collections in a report](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md) 
* [View: hide the content of a column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md) 
* [View: display an image instead of a string in a column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md) 
* [View: display task indentations in a task list](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md) 
* [View: calculate time and date differences](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## Use Text Mode in filters {#use-text-mode-in-filters}

You can use text mode when building filters to expand on the fields and objects you can filter by.

For examples of the most common reasons for using text mode in a filter, see the following articles:

* [Filter: create multiple filter rules that reference the same field ("AND" statements)](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md) 
* [Filter: display only items in an approval status](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md) 
* [Filter: display items by same-name statuses when the statuses are associated with different groups](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md) 
* [Filter: eliminate items in a list by comparing two fields](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md) 
* The section [Examples of text mode filters that span multiple levels in the object hierarchy](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples) in the article [Create complex Text Mode filters using EXISTS statements](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)
* The section [Create complex text mode filters for missing objects](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters) in the article [Create complex Text Mode filters using EXISTS statements](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)

## Use Text Mode in groupings {#use-text-mode-in-groupings}

You can use text mode when building groupings to expand on the fields and objects you can group by in lists and reports.

For examples of the most common reasons for using text mode in a grouping, see the following articles:

* [Grouping: organize list results by a calculated value common to all objects in the grouping](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md) 
* [Grouping: add a fourth grouping to a list](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md) 
* [Grouping: edit the display name in a grouping](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md) 
* [Grouping: indicate whether the results of a grouping should be collapsed or expanded using text mode](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
