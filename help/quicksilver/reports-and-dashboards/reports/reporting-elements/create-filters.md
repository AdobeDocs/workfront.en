---
filename: create-filters
product-area: reporting
navigation-topic: reporting-elements
title: Create or edit filters in Adobe Workfront
description: You can use filters to reduce the amount of information you display on the screen.
---

# Create or edit filters in Adobe Workfront

You can use filters to reduce the amount of information you display on the screen.

You can apply the following types of filters in&nbsp;Adobe Workfront:

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
   <td> <p>Manage permissions to a report to create or edit a filter in a report</p> <p>Manage permissions to a filter to edit it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
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
1. Click the Filter icon . 
1. Click New Filter at the top of the list of filters Or Hover over the filter you want to modify and click the Edit icon . The interface builder for customizing the Filter launches.
1. Do any of the following:

  * Modify existing filter rules by clicking the existing rule and selecting a new option.
  * Add a filter rule by clicking `Add another Filter Rule`, begin typing the name of the option for which you want to add a rule in the `Start typing field name` box, then click it when it appears in the drop-down list.

    Fields associated with the object of your filter are listed in the `Start typing field name` box. 
  
  * Click `AND` or `OR` when adding a new filter rule.  
    When adding filter rules, use the filter modifiers to establish the condition of your filter. For more information about filter modifiers, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

    >[!NOTE]
    >
    >When you connect a group of AND&nbsp;statements by multiple OR statements, you must repeat the fields that are not changing between the OR statements for each group of statements. 
    >
    >
    >![](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-350x163.png)    >
    >

    >
    >When you build a filter for tasks that contain the word "marketing" and are in projects with a status of Current or Planning, you must have the following filter rules:
    ><pre>Task: Name Contains Marketing</pre><pre>AND</pre><pre>Project: Status Equals Current</pre><pre>OR</pre><pre>Task: Name Contains Marketing</pre><pre>AND</pre><pre>Project:&nbsp;Status Equal Planning</pre>Although Task: Name Contains "marketing" does not change between the two AND filter groups, it must be repeated in the second group.

  * Delete an existing filter rule by clicking the 'X' icon.

1. (Optional) Click `Switch to Text Mode` to add a filter using the Text Mode interface.

   For more information about creating a filter using the text mode interface, see [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md). 

1. Click `Save Filter` to replace the current Filter with your changes.
1. (Optional) If you no longer want to display a filter in the `Filter` drop-down menu, click `Remove Filter`.

   The My Filters dialog box is displayed.

   All filters that you have rights to remove are available to remove. Other filters are displayed as dimmed.

1. Click the ( `x`) next to any filters you want to remove, then click `Done`.

## Additional information

See also:

* [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md) 
* [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md) 
* [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md) 
* [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md) 
* [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)

&nbsp;

<!--
You can limit the amount of information you display on the screen in a list of items with a filter. You can define certain criteria based on particular pieces of information about an object and only display those objects that meet those criteria. You can apply the following types of filters in Adobe Workfront: Quick filters in a list of objects to find an item using a keyword. These are temporary filters that you cannot save for future use. For information about quick filters, see Apply the quick filter to a list. Permanent filters that you can save and use numerous time on multiple lists and reports. This article describes how to create a permanent filter or edit an existing one in a list or report. Filters in other areas of Workfront, outside of lists and reports. For a list of all filters in Workfront and the areas where you can apply them, see Filters overview in Adobe Workfront. Access requirements You must have the following access to perform the steps in this article: Adobe Workfront plan* Any Adobe Workfront license* Request or higher Access level configurations* Edit access to Filters, Views, and Groupings Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see Create or modify custom access levels. Object permissions Manage permissions to a filter For information on requesting additional access, see Request access to objects in Adobe Workfront. *To find out what plan, license type, or access you have, contact your Workfront administrator. Types of filter-building interfaces You can create filters using the types of filter builders described in the table below: Builder type Filter object Where available Standard builder All objects Lists and reports Beta builder Projects Tasks Issues Lists The Projects list in the Scenario Planner This is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see The Adobe Workfront Scenario Planner overview. Requests area Note: Beta builders for filters are not available in reports. For information about Workfront objects, see Understand objects in Adobe Workfront. Create or edit a filter in the standard builder You can create filters in lists and reports in the following ways: From scratch Edit an existing filter and save it as a new filter Regardless of the method you use to create filters, creating a filter from scratch or from an existing filter is similar. Go to a list or a report where you want to create a filter or that contains the filter that you want to customize. Click the Filter icon . Tip: The report creator must allow for filters to be edited in order to view the Filter drop-down list on a report. The Report Default filter is applied to a report by default. The Report Default filter can be customized only when you edit the report. Click New Filter at the top of the list of filters Or Hover over the filter you want to modify and click the Edit icon . The builder for customizing the filter opens. Do any of the following: Modify existing filter rules by clicking the existing rule and selecting a new option. Add a filter rule by clicking Add another Filter Rule, begin typing the name of the option for which you want to add a rule in the Start typing field name box, then click it when it appears in the drop-down list. Fields associated with the object of your filter are listed in the Start typing field name box. Click AND or OR when adding a new filter rule. When adding filter rules, use the filter modifiers to establish the condition of your filter. For more information about filter modifiers, see Filter and condition modifiers. Note: When you connect a group of AND statements by multiple OR statements, you must repeat the fields that are not changing between the OR statements for each group of statements. Example: When you build a filter for tasks that contain the word "marketing" and are in projects with a status of Current or Planning, you must have the following filter rules: Task: Name Contains Marketing AND Project: Status Equals Current OR Task: Name Contains Marketing AND Project:&nbsp;Status Equal Planning Although Task: Name Contains "marketing" does not change between the two AND filter groups, it must be repeated in the second group. Delete an existing filter rule by clicking the 'X' icon. (Optional) Click Switch to Text Mode to add a filter using the Text Mode interface. For more information about creating a filter using the text mode interface, see Edit a filter using text mode. Click Save Filter to create a new filter or replace the selected one with your changes. Or Click Save as New Filter to create a new filter from the selected one. The new filter displays in the list of filters and it is automatically applied to the list or report you selected. (Optional) Do one of the following: Share filters you create with other users, or make them available system-wide. For information, see Share a filter, view, or grouping in Adobe Workfront. Remove filters you no longer want to display in the list. For information, see Remove filters, views, and groupings. Create or edit a filter in the beta builder Consider the following when creating filters using the different interfaces: You can find the beta builder in the same places you find the standard filter interface for the areas listed in the table above. You can switch back and forth between the standard and the beta builder interface, where the beta option is available. After you have enabled the beta builder in one area, it is the default experience for all areas where it is available. For example, if you enable the beta builder in a project list, it is the default experience for building task and issue filters in lists as well. You can create filters using the beta builder interface in project, task, and issue lists in the following ways: From scratch Edit an existing filter Duplicate an existing filter Duplicate an existing filter, edit it, and save it as a new filter Saved filters are available in both builders, regardless of which experience you used to originally build them. For example, if you created a filter using the standard builder, you can find and modify it in the beta builder interface as well. The standard and beta builders have a slightly different syntax when building multiple-statement filters that combine the AND and OR operators. As a result, these filters may display differently when you switch from one builder to another. Example: The following scenario exists: Use the beta builder to create a filter that has the following syntax: (A OR B) AND C Switch back to the standard builder and edit the filter using the syntax of the standard builder as described in the Create or edit a filter in the standard builder section in this article. The syntax for the standard builder displays the filter statements as follows: A AND C OR B AND C Make a change to the filter in the standard interface. Switch back to the beta builder. The filter statement displays according to the logic supported in the standard builder, as described in Step b. The filter displays in the beta builder interface as follows: A AND C OR B AND C This happens because the filter was modified in the standard interface. Create a filter using the beta builder interface: Go to a project, task, or issue list where you want to create a filter or that contains the filter that you want to customize. Click the Filter icon , then enable the Beta setting to access the beta builder. It is disabled by default. This opens the beta filter builder interface. Tip: The header of the filter builder interface changes to blue when you enable the beta builder. After you enabled the beta builder interface, Workfront keeps it enabled for all areas where it is available. Review the following lists of filters: My filters Filters that you build and saved yourself. Suggested Filters that the Workfront administrator adds to your list of filters, either at the system level, or in your Layout Template. Shared with me Filters that others create and share with you or that are shared system-wide. Do one of the following: Click New filter to create a filter from scratch Hover over an existing filter that you have permissions to manage and click the Edit icon to edit an existing filter. Or Hover over an existing filter that you have permissions to manage and click Duplicate to copy the existing filter and edit a copy. (Conditional) Depending on whether you want to find objects that match all or any of the statements in a filter group select from the following options: Include if all are true The objects found by the filter must match all filter criteria in a filter group. In this case, the filter statements are connected by the AND operator. This is the default selection. Include if any are true The objects found by the filter must match any filter criteria in a filter group. In this case, the filter statements are connected by the OR operator. For more information about filter operators, see Filters overview in Adobe Workfront. Start typing the name of a field, then select it when it displays in the list. You can also select Search all fields to view a list of all fields to filter by. The fields in the advanced search are grouped by object category. Click the modifier drop-down menu to select a modifier. The default modifier is "Equals." For more information, see Filter and condition modifiers. Tip: As you build the filter, the results appear immediately in the list. Start typing the value of a field you want to filter by. For example, start typing the name of an issue, if you want to filter by Issue:Name. Select the value when it displays in the list. Tip: Depending on what modifier you selected, you can select multiple values. Click Add filter to select another field and add a new filtering criteria to the filter statement. (Optional) Click the Delete icon to remove existing filter statements. Or Click Clear all to clear all filtering criteria. (Optional) Click Add filter group to add another set of filtering criteria. Tip: You might want to user another filter group when you want the groups to be connected by a different operator than the operator in a filter statement. Example: When you filter for project that contain "marketing" in the name that are either not complete and are not On Hold, you can use the following multiple filter groups: (Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100) OR (Project: Name Contains Marketing AND Project: Status Does not equal On Hold) In this case, each filter statement is connected by an AND and the filter groups are connected by an OR. (Optional) Click Text mode to continue building the filter using text mode. The text mode interface opens. Tip: We recommend building as much of the filter as possible using the beta builder interface and only using text mode when you must make modifications to the filter that are only supported in text mode. For more information about creating a filter using the text mode interface, see Edit a filter using text mode. (Optional) Click Exit text mode to return to the beta builder interface. Warning: Some text mode statements are not supported in the beta builder or the standard interface. Exiting text mode when you have created these types of statements might generate a warning message. (Optional) Click Apply to apply the filter to the list and see the results. The number of filter statements including filter groups that you selected displays next to the filter icon at the top of the list. Click Save as new to save the filter for future use. Select Untitled Filter and enter the name of the new filter instead. Select an icon for the new filter from the Icon drop-down menu. (Optional) Add a description for the filter to indicate what is unique about it. The description displays under the filter name in the list of filters. Tip: Clicking Cancel at any time takes you back to the filter building area. Click Save. The filter is saved in the My filters list and is applied to the list of items. (Optional) Select another filter to apply it in addition to the new filter you just created. Tips: There is no limit to the number of filters you can select. When you select multiple filters all their conditions must be met simultaneously to display matching results. The number of filters you selected displays next to the filter icon at the top of the list of items. (Optional) Do one of the following: Share the filter with others, or make it available system-wide. For more information, see Share a filter, view, or grouping in Adobe Workfront. Delete the filter if it is no longer valid or a duplicate. For information, see Delete filters.
-->

&nbsp;
