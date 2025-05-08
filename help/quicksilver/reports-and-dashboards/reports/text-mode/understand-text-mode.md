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

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

You can build a report or a list in Adobe Workfront by using either the standard or the text mode interface when creating the elements that make up the report or the list. 

The standard interface allows you to reference fields and their attributes that are readily available in the Workfront interface. 

Using text mode you can reference fields and attributes that might not be available in standard mode, but are available in the Workfront database.

For more information about creating reports using text mode, including classes, videos, and tutorials, see the Learn section on the Adobe Experience League site. 

## Considerations before using text mode

>[!TIP]
>
>You can also expand the capabilities of calculated custom fields by using a version of text mode for custom fields. The syntax and rules for creating a calculated custom field are different than those you use in reports and lists. For information about adding a calculated custom field, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Before you start using text mode in your reports, we strongly recommend that you take our classes on advanced reporting, to gain a deeper understanding of our text mode language.
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

Text mode enables you to create more complex views, filters, groupings, and prompts by allowing you to use fields that are not available in the standard mode interface. In&nbsp;Workfront text mode is a collection of coded statements that indicate what objects you want to display in a report or a list.

For a complete list of all our reportable fields, see the [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Not all the fields available through the API are available through the text mode interface. If you use the correct field in your text mode code and you do not display the results you expect, then the field might only be reportable through the API.

## Access reporting elements and edit text mode {#access-reporting-elements-and-edit-text-mode}

Accessing the text mode interface is similar for views, groupings and filters when accessing them from a report or a list.

For information about using text mode in views, filters, and groupings, see:

* [Edit a view using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md) 
* [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md) 
* [Edit a grouping using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Custom prompts can only be edited in text mode. You can access prompts only from a report.

For information about accessing the text mode interface for custom prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Common reasons to use Text Mode {#common-reasons-to-use-text-mode}

Outside of creating custom prompts which can only be configured using text mode, we recommend that you use the report builder to build your views, filters and groupings. However, there are some instances where you can use text mode to enhance your reports and lists.

For more information about common uses for text mode, see [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
