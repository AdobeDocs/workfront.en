---
product-area: reporting
navigation-topic: text-mode-reporting
title: Edit a filter using text mode
description: You can edit a filter in a list or report using text mode to access fields that are not available in the standard interface and create more complex filters.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
---
# Edit a filter using text mode

<!-- Audited: 1/2025 -->

You can edit a filter in a list or report using text mode to access fields that are not available in the standard interface and create more complex filters.

For more text-mode examples when creating a filter, also see the section [Samples of custom filters](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) in the article [Custom view, filter, and grouping samples: article index](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
      <p>New:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Current:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Filters, Views, and Groupings</p> <p>Edit access to Reports, Dashboards, and Calendars to edit reporting elements in a report</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to edit filters in a report</p> <p>Manage permissions to a filter to edit it</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before starting to use text mode in a report or list, always ensure that you are familiar with the Workfront text mode syntax.

For more information, see:

* [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md) 
* [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md) 
* [Custom view, filter, and grouping samples: article index](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Edit text mode in a filter

Editing a filter using text mode is identical for reports and lists. Accessing the filter from a report or from a list differs.

>[!TIP]
>
>We recommend that you build as much of the filter as possible in standard mode, then convert the filter to text mode to edit it.

For more information about building filters, see [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

For information about creating a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Do one of the following:

   To access the filter from a list, go to the list and click the **Filter** icon, then hover over the filter in the side **Filters** side panel that you want to modify and click the **Edit** icon ![Edit icon](assets/edit-icon.png). Either the **Filters** side panel displays your selected filter or the legacy filter builder opens.

   OR

   To access the filter from a report, go to the report, then click **Report Actions** > **Edit** > **Filters** tab.

1. Do one of the following:

   If you are using the **Filters** side panel on a list, click **Text mode**.

   OR

   If you are using the legacy filter builder or in a report, click **Add a Filter Rule** to start adding the conditions of your filter. Then, click **Switch to Text Mode** then **Edit Text Mode** on the right side of the builder.

1. Add filter statements using text mode. Each filter statement may contain the following lines and additional information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Filter line/information</b></td> 
      <td><b>Example</b></td> 
     </tr> 
     <tr> 
      <td> <p>Field name and the value that it equals as they appear in the Workfront database.</p> <p>This line is mandatory.</p> <p> For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>To filter for tasks in a status of In Progress, use the following line:</p> <p><code>status=INP</code> </p> <p><b>TIP</b> 
      
      When filtering for statuses, you must use the three-letter code of the status and not the name.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Field name modifier and what the modifier equals. This indicates which conditions the field you are filtering by must fulfill.</p> <p>This line is mandatory.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>To indicate that the status of the tasks you filter for must be equal to In&nbsp;Progress, use the following line in addition to the one above:</p> <p><code>status_Mod=in</code> </p> <p>If the modifier is a range, there are two lines to indicate the modifier.</p> 
       <div> <span class="autonumber"><span><b>EXAMPLE </b></span></span> 
        <p>This is a text mode filter that looks for tasks that are in progress, that have a Planned Completion&nbsp;Date within the current month, and are assigned to a user with a specific GUID:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>For a complete list of filter modifiers in text mode, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Statement operator. By default, each filter statement is connected by the "AND" operator. This does not display in the text mode interface. You can also add an "OR" operator between two statements to indicate that you want to filter for objects that can fulfill one or the other of two conditions.</p> <p>Filter operators are required only for filters that have more than one statement.</p> <p>Tip:   
        <ul> 
         <li> <p>"OR" is case sensitive and must always be capitalized.</p> </li> 
         <li> <p>When you change your operator from&nbsp;AND&nbsp;to OR, the number of list items may increase.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>EXAMPLE </b></span></span> 
        <p>To filter for tasks in a status of In&nbsp;Progress or with a Planned Completion Date of Today, use the following: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>A wildcard, which allows you to generalize the information in a filter and reference the current time or the user who is logged in.</p> <p>Wildcards are optional.</p> <p>Tip:   <p>We recommend using wildcards whenever possible to make your filters more dynamic and not duplicate the same filters for each user or similar time frames.</p> <p>For information about filter wildcards, see <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Wildcard filter variables overview</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>EXAMPLE</b></span></span> 
        <p>To filter for tasks that are assigned to the user that is currently logged in, use the following:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. To add a filter statement connected by the "OR" operator, do the following:

   1. Add a new line of code and type OR:1: followed by the object or attribute you want to filter by and the value you want to compare it with. To reference tasks that are in any status except New, use the following line:

      `OR:1:status=NEW`

   1. Add a second line and type OR:1: followed by the object, the modifier, and the modifier code. To define the modifier for the line of code referencing all task statuses except for New, use the following modifier line:

      `OR:1:status_Mod=notin`

      Each line of the new statement must be preceded by "OR:`<number>`:".

      For information about creating "OR" statements in a filter, see [Create "OR" statements in text mode filters](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >You can have multiple "OR" statements in the same filter. Every time you have a new "OR" statement, the number after "OR:" increases.
      >
      >To filter for tasks that are in a status of In Progress or are assigned to the logged-in user or they have the Planned Completion Date today, use the following:
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Click **Apply** or **Done** to save your text mode changes and continue editing the report or the filter.
1. Click **Save + Close** to save your report or **Save Filter** to save the filter in the list.


