---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Get started with reports
description: Reports provide visibility into what is happening with users and work. Using reports, you can display information about objects in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
---
# Get started with reports

<!-- Audited: 12/2023 -->

Reports provide visibility into what is happening with users and work. Using reports, you can display information about objects in Adobe Workfront.

For information about understanding objects and how they can be reported on in the Workfront application, see [Adobe Workfront objects overview](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Report elements

Reports are a combination of the following three elements in Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">View</td> 
   <td> <li>Defines the columns in your report and what information you can include in each column.</li> <li>For information about views, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Grouping</td> 
   <td> <li>Categorizes information based on a common piece of information and lists the results of the report under headings.</li> <li>For information about groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <li>Controls the amount of information that appears in a report.</li> <li>For information about filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview</a>.</li> <li>For information about filter modifiers, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</li> <li>You can filter by using wildcards, to make your filters more general and give them more flexibility of usage.</li> <li>For information about using wildcards in filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Wildcard filter variables</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>When you select a new filter, view, or grouping from a list, that selection is retained even if you log out of Workfront or close your browser.

For information about report elements, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

To enhance your reports, you can add the following elements:

* A chart: a visual representation of the results in your report.  
  For information about chart reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* A matrix grouping: summarizes the information of the report in an aggregated table format.  
  For information on matrix reports, see [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* A prompt: an open filter that you can customize and apply differently every time you run the report.  
  For information about prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

When building a report, you can modify any of these elements individually in the report builder.

Another way of enhancing the relevance of the information included in your reports is by applying conditional formatting to your views.  
For information about using conditional formatting, see [Use conditional formatting in views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## System reports

Workfront provides several system reports that come loaded in your system by default.  
After entering information in your system you can use these reports to display the information visually.

For more information about how to access system reports and which system reports are available, see [Use Adobe Workfront built-in reports](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Create reports

In addition to the system reports that Workfront provides, you can create your own customized reports to meet the needs in your organization.

To create a report you can do one of the following:

* Build a report from scratch.
* Copy an existing report.  
  You must have at least View permission to copy a report created by someone else. For more information about copying a report, see [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

For information about creating reports, see [Calendar reports overview](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

### Prerequisites for creating reports {#prerequisites-for-creating-reports}

* You must have a Plan license (current licenses) or Standard license (new licenses) to create your own reports.  
  For information about the Workfront license types, see [Licenses overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) for the current licenses, and [New licenses overview](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) for the new licenses.

* Your Workfront administrator must give you access to Edit Reports in your Access Level.  
  For information about granting access to Edit reports, see [Grant access to reports, dashboards, and calendars](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Your Workfront administrator must give you access to Edit Filters, Views, and Groupings in your Access Level.

  For information abut granting access to Edit filters, views, and groupings, see [Grant access to filters, views, and groupings](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* You must define one object that you want to report on. Reports are object specific in Workfront and you must start with selecting an object type before you can start building the report. You can only report on objects available in the Workfront interface.

### Report ownership {#report-ownership}

When you create a report in Workfront, you become the default owner of the report and it displays in your My&nbsp;Reports section. You cannot change the owner of a report.

When you copy a report, you automatically become the owner of the copied report.
For information on copying reports, see [Create a copy of a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

You can see who owns a report by reviewing the **Entered By** field.

![Entered By field](assets/nwe-entered-by-350x218.png)

### Create reports in the builder interface {#create-reports-in-the-builder-interface}

We recommend that you use the report building interface first to build a new report. The interface offers a streamlined set of tools that walk you through putting elements together to create the report you want. You have objects and fields that you can select from lists and add to all your reporting elements.  
For more information about creating reports in the report building interface, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

For a list of objects that you can report on, see the [Report on objects](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects) section in the article [Adobe Workfront objects overview](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

For more information on the fields that you can display in reports, see [Glossary of Adobe Workfront terminology](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Create reports in Text Mode {#create-reports-in-text-mode}

At times, you might be not able to find certain fields in the builder interface, but they might be available in the API.  
For information about what fields are available in the API, see the article [API Explorer](../../../wf-api/general/api-explorer.md).

For information about how to use the API Explorer, see the article [Using the API Explorer](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>You cannot report in the Workfront interface on objects that are not available in the report builder. However, you can report on fields associated with the objects in the report builder if those fields are available through the API. To do this, you must use the Text Mode interface.

Text Mode enables you to create more complex views, filters, groupings, and prompts by allowing you to use fields that are not available in the standard mode interface.

#### Text Mode terminology {#text-mode-terminology}

You must use a specific syntax to use the Workfront Text Mode interface.

For more details about the Workfront syntax for text mode, see [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Calculated Columns, Conditional Formatting, and other uses of Text Mode {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

Outside of reporting on fields that are not available in the builder interface, you can use Text Mode to display calculations or comparisons between certain fields.

For a list of the most common uses of Text Mode in a report, see [Overview of common uses for Text Mode](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

For information about including calculated custom data in reports, see [Calculated custom data in reports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

For information about comparing fields in conditional formatting, see [Compare fields in conditional formatting](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

You can also refer to collection fields using Text Mode in reports.  
For information about using Text Mode to display collection information in a report, see [Reference collections in a report](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Text Mode samples {#text-mode-samples}

We have a library of samples of the most used views, filters, and groupings you can create with Text Mode.

To browse this library and use some of the samples we offer, see the article [Custom view, filter, and grouping samples: article index](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## The tabs of a report

A report can contain several tabs when you run the report in the interface.

For information about running a report, see the article [Run a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

On each tab, the information you include in the report displays in slightly different formats. Choose the format that best fits the needs of your organization.

You can make any tab the default tab of the report. The default tab is the first tab that displays when you click the name of a report to open it, and it is the tab that displays when you place the report on a dashboard.

### Details tab {#details-tab}

The Details tab of a report displays the object of the reports and the attributes that you choose for that object in a list form. Every report has a Details tab.

>[!IMPORTANT]
>
>Information in the Details tab may display differently from the Chart tab based on your time zone.  
>For example, a user in California completed a task at 9:30 pm PST on February 12. When a user in New York views a report that includes this task completion, the Actual Completion Date displays as February 13 in both the Details tab and the Chart details because it was completed at 12:30 am EST on February 13. However, in the chart, it is included in the February 12 grouping until you expand the chart element.

### Summary tab {#summary-tab}

Reports that include a grouping have a Summary tab.

The same information displayed in list format on the Details tab is summarized and aggregated according to the groupings in the report on the Summary tab.

For information about groupings, see [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Matrix tab {#matrix-tab}

Reports that include a Matrix Grouping have a Matrix tab.

The same information displayed in list format on the Details tab is displayed in a table format, grouped by the groupings in the report on the Matrix tab.

When you add a Matrix grouping to a report, the Summary tab is replaced by the Matrix tab.

For information about building a Matrix Grouping, see the article [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Chart tab {#chart-tab}

Reports that include a chart have a Chart tab.

Consider including a chart in your reports for impactful dashboards for your executives. Charts are a concise way to display the information in a report. You can expand a chart element by clicking it to display the items included in that element.

>[!IMPORTANT]
>
>When you click a chart element, the expanded information may display differently from the chart based on your time zone.  
>For example, a user in California completed a task at 9:30 pm PST on February 12. When a user in New York views a report that includes this task completion, the Actual Completion Date displays as February 13 in both the Details tab and the Chart details because it was completed at 12:30 am EST on February 13. However, in the chart, it is included in the February 12 grouping until you expand the chart element.

For information about building a report with a chart, see the article [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Prompts tab {#prompts-tab}

Reports that include a prompt have a Prompts tab.

A prompt allows you to add a filter to a report every time you run the report. When you add a prompt to the report, the Prompts tab becomes the default tab of the report automatically. This cannot be changed to another tab.

For information about building a prompt for a report, see the article [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Share reports

After you create a report, you can share it with other users.

### Give sharing permissions to a report {#give-sharing-permissions-to-a-report}

You can give sharing permissions to another user to View or Manage a report you create. You can give another user a level of permissions equal or lesser than yours. You can also make a report public using sharing permissions. For information about sharing a report, see [Share a report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Schedule a report delivery {#schedule-a-report-delivery}

You can schedule a report for delivery. The users you are sharing the report with receive an email with an attachment of the report results. The attachment can be in the following formats:

* HTML
* PDF
* Excel
* .TSV

For information about scheduling a report delivery, see [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### Export the results of a report {#export-the-results-of-a-report}

You can export the results of a report to the following file formats:

* PDF
* Excel (.xls and .xlsx formats)
* Tab Delimited

For information about exporting the results of a report, see [Export data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

After the report is exported to one of these formats, you can share it with other users by emailing it as an attachment or printing it.

### Add a report to a dashboard {#add-a-report-to-a-dashboard}

You can add a report to a dashboard and share the dashboard with other users. For information about adding reports to a dashboard, see [Add a report to a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Create calendars

If you want to display your data in a calendar format, you can create calendars instead of reports.

For information about building and using calendars, see [Calendar reports overview](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Report usage

After creating reports and sharing them with other users, you can track how often they use these reports.
For information about report usage, including how often they are viewed, by what user, and what dashboards they display on, see the article [Report usage overview](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## Common terms used in reference to reports

The following terms are used in reference to Workfront reports: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Term or Phrase</strong> </th> 
   <th><strong>Definition</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Advanced Options</td> 
   <td> <p>Refers to the link on the Columns (View) tab of the report builder that provides the ability to do the following:</p> 
    <ul> 
     <li>Set column conditional style formatting of text and images based on criteria you select.</li> 
     <li>Relabel your column.</li> 
     <li>Format the values in your column.</li> 
    </ul> <p>For example, you may want to show all parent tasks in bold, or you may want to display the Planned Completion Date in red if the task is late.</p> </td> 
  </tr> 
  <tr> 
   <td>Attribute</td> 
   <td> The field of an object as defined in the database. It is used in a Text Mode expression. <br>For example, the Status field is displayed as <em>status</em> when used in a Text Mode expression. </td> 
  </tr> 
  <tr> 
   <td>Bean or JavaBean</td> 
   <td>A Bean represents a reusable-programming element. The term Bean identifies relationships between different objects in the Workfront application. It is important to be familiar with these relationships as you attempt to display additional attributes about an object that are not available in the basic reporting tools.</td> 
  </tr> 
  <tr> 
   <td>Builder Interface or Report Builder</td> 
   <td>The Builder Interface is the series of drop-down menus containing fields displayed in the Columns (View), Filter, and Grouping tabs. It provides an intuitive mapping of the Bean relationships to assist in identifying the columns in a view, the criteria of a filter, and the common attributes of a grouping.</td> 
  </tr> 
  <tr> 
   <td>Camel Case</td> 
   <td> <p>Camel Case refers to a specific way to write programming elements to string multi-word attributes together. When spelling an attribute in Camel Case, the first letter of the first word is lower case, there is no space between the words, and the first letter of any subsequent word is uppercase.</p> <p>For example, Home Group would be written as <em>homeGroup</em>, Resource Pool would be <em>resourcePool</em>, and Actual Start Date would be <em>actualStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Chart</td> 
   <td> <p>A tab inside the report builder, a report tab, after you save the report, as well as an optional element of a report which allows you to add a chart to any report. You must define a Grouping in the report before you can create a chart.</p> <p>The following are types of charts that can be added to any report:<br></p> 
    <ul> 
     <li>Column</li> 
     <li>Bar</li> 
     <li>Pie</li> 
     <li>Line</li> 
     <li>Gauge</li> 
     <li>Bubble</li> 
    </ul> <p>For more information about adding charts to reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Details</td> 
   <td>This is one of the tabs of a report, after you save the report. It displays the findings of your report, displayed in the view and grouping of your choice.</td> 
  </tr> 
  <tr> 
   <td>Expression</td> 
   <td>An expression is a written formula in Text Mode to convey information to be searched for or displayed when using the Text Mode interface. It is typically one line in a larger Text Mode statement.</td> 
  </tr> 
  <tr> 
   <td>Fields</td> 
   <td> <p>Refers to the attributes of your objects. For example, "Status" is a field for Projects, Tasks, or Issues. "Portfolio Manager" is a field for the Portfolio object.</p> <p>You can also have custom fields that you create yourself and add to custom forms.<br>For information about creating custom forms, see the article <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Design a form with the form designer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Field Name </td> 
   <td>The value of an attribute that is displayed in a view, or used in the condition of a filter, or as the common element of a grouping. The options for the Field Name are dependent on the Field Source selection.</td> 
  </tr> 
  <tr> 
   <td>Field Source </td> 
   <td>The value of an object that is displayed in a view, or used in the condition of a filter, or as the common element of a grouping. The options in the Field Source are dependent on the object type of the UI element being created. The Field Source allows you to reference attributes from objects other than the object type of the UI element.</td> 
  </tr> 
  <tr> 
   <td>Filter</td> 
   <td>A main report element that determines which results display in the report.</td> 
  </tr> 
  <tr> 
   <td>Form </td> 
   <td>Used interchangeably with "Custom Form." Fields and sections are added to forms, which are then attached to an object to extend the number of fields you can associate with an object.</td> 
  </tr> 
  <tr> 
   <td>Grouping </td> 
   <td>A main report element that identifies how a list of results is organized. The grouping creates horizontal bars throughout the report to group the results by common attributes defined when creating it. Groupings are used in Matrix Reports to aggregate data, as well as in charts, to determine the axes of charts.</td> 
  </tr> 
  <tr> 
   <td>Object or Object Type</td> 
   <td> An object is a Workfront application element (for example, Project, Task, Group, Company, Filter). The Object Type is used when creating a new report, view, filter, or grouping to identify which object is the focus of the report. Reports can have only one object type, which is the main object of the report.<br>Parent objects may be referenced in the same report.<br>For more information about the hierarchy of objects, see the section "Understanding the Interdependency and Hierarchy of Objects" in the article <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront objects overview</a>.</td> 
  </tr> 
  <tr> 
   <td>Prompt</td> 
   <td> <p>An optional report element that can be added to a report when you need to use a different filter every time you run the report.</p> <p>For information about prompts, see <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Qualifier or Condition Modifiers</td> 
   <td> <p>This field appears in the following areas of a report:</p> 
    <ul> 
     <li>On the Filter tab</li> 
     <li>The Advanced Options screen for the column in the Columns (View) tab. By defining a qualifier, you can compare the Field Name to another field or value.</li> 
     <li> In a Custom Prompt<br><p>For information about prompts, see <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p>.</li> 
    </ul> <p>For example, when building a filter for tasks with a Planned Completion Date of Today, you would select <strong>Equal</strong> in your Qualifier field, and today's date in the Date field:</p> <p><em>Task&gt; Planned Completion Date&gt;Equal&gt;(today's date)</em> </p> <p>In this scenario the Qualifier is <strong>Equal</strong>.<br>For more information about qualifiers, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Report </td> 
   <td>The combination of a view, a filter, and (sometimes) a grouping. The purpose of a report is to display data consistently across the interface, to distribute information, and to eliminate the need to run the same search or query on a regular basis.</td> 
  </tr> 
  <tr> 
   <td>Statement</td> 
   <td>Consists of several expressions that are put together to define what information displays in a report when using Text Mode. A statement can be created for a view, filter, grouping, or for a Custom Prompt in a report.</td> 
  </tr> 
  <tr> 
   <td>Summary</td> 
   <td>This is one of the tabs of a report, after you save the report. This tab is created only when you define a grouping for the report. It summarizes information based on the grouping defined during report creation and gives a quick overview of the aggregated objects of the report. It does not display every object in the report, just those that are aggregated.</td> 
  </tr> 
  <tr> 
   <td>Text Mode Interface</td> 
   <td>Provides the ability to create or modify the code of custom views, filters, groupings, and prompts originally created through the Builder Interface. It is suggested that report elements are initially created through the Builder Interface and then converted into the Text Mode after they have been saved to simplify the coding of advanced views, filters, groupings, or prompts.</td> 
  </tr> 
  <tr> 
   <td>User Interface (UI)</td> 
   <td>Refers to the components or building blocks of what displays on the screen of a user at any given time.</td> 
  </tr> 
  <tr> 
   <td>View (or Columns)</td> 
   <td>One of the main elements of a report. It identifies the column headers that will be displayed in the list of a report.</td> 
  </tr> 
 </tbody> 
</table>
