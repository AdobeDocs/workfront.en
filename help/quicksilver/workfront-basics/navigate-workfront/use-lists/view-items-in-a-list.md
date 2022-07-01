---
navigation-topic: use-lists
title: Get started with lists in Adobe Workfront
description: "Objects can be displayed in lists in Adobe Workfront. A list is a grid that contains a number of objects, information about them, or other objects referenced from them. Suggested edit: You can view lists of objects in Adobe Workfront to get information about them, such as their start and due dates, users assigned to them, and other objects that are associated with them."
feature: Get Started with Workfront
---

# Get started with lists in&nbsp;Adobe Workfront

Objects can be displayed in lists in Adobe Workfront. A list is a grid that contains a number of objects, information about them, or other objects referenced from them. 

<!--
<MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
Suggested edit: You can view lists of objects in Adobe Workfront to get information about them, such as their start and due dates, users assigned to them, and other objects that are associated with them.
</MadCap:conditionalText>
-->

The following are some characteristics of lists in Workfront:

* Lists are object specific: one list can reference only one type of object. Other objects that are directly connected to the object of the list can also be referenced in the same list. 

  <!--
  Suggested edit: I would remove this and the sentence below if you use the alternative first paragrap above.
  -->

  For example, a list of tasks includes task information like Assignments, Start and Due Date, but it can also include project information like Project Name or the name of the Project Owner.

* Lists refresh automatically every 5 minutes to update information that other users in the system are updating elsewhere.
* Some areas in Workfront are preconfigured with default lists of objects.

  You can customize most of these preconfigured lists.

* A Workfront administrator can create custom lists to apply to various areas of Workfront.

  For more information about creating system-level lists, see the article [Create, edit, and share default filters, views, and groupings](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

Below are some types of object lists that you can find in Workfront and some of the areas where they display by default when you have rights to view an object.

>[!NOTE]
>
>This list is not comprehensive. Each of these object lists can also appear on a report or a dashboard.  
>For example, a Project report or a dashboard that contains a Project report also displays a list of projects.

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Might be useful to add a Description column that explains the objects that appear in each list.</p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront list</th> 
   <th>Location of object list</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>List of portfolios</td> 
   <td> 
    <ul> 
     <li> <p>Portfolios</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of programs</td> 
   <td> 
    <ul> 
     <li> <p>Portfolios &gt; select a portfolio &gt; Programs</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Programs</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of projects</td> 
   <td> 
    <ul> 
     <li> <p>Projects</p> </li> 
     <li> <p>Portfolios &gt; select a portfolio &gt; Projects</p> </li> 
     <li> <p>Portfolios &gt; select a portfolio &gt; Programs &gt; select a program &gt; Projects</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of tasks</td> 
   <td> 
    <ul> 
     <li> <p>Projects &gt; select a project &gt;&nbsp;Tasks</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Tasks &gt; select a task &gt; Subtasks</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Tasks &gt; select a task &gt;&nbsp;Predecessors*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of issues</td> 
   <td> 
    <ul> 
     <li> <p>Projects &gt;&nbsp;select a project &gt; Issues</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Tasks &gt; select a task &gt;&nbsp;Issues</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Tasks &gt; select a task &gt; Subtasks &gt; select a task &gt;&nbsp;Issues</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of reports</td> 
   <td> 
    <ul> 
     <li> <p>  Reports  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of dashboards</td> 
   <td> 
    <ul> 
     <li> <p>Dashboards</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of iterations</td> 
   <td> 
    <ul> 
     <li> <p>Teams &gt;&nbsp;Iterations</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of users</td> 
   <td> 
    <ul> 
     <li> <p>Users</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of documents</td> 
   <td> 
    <ul> 
     <li> <p>Documents</p> </li> 
     <li> <p>Portfolios &gt; select a portfolio &gt;&nbsp;Documents</p> </li> 
     <li> <p>Portfolios &gt;&nbsp;select a portfolio &gt; Programs &gt; select a program &gt; Documents</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Documents</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Tasks &gt; select a task &gt;&nbsp;Documents</p> </li> 
     <li> <p>Projects &gt;&nbsp;select a project &gt;&nbsp;Issues &gt; select an issue &gt;&nbsp;Documents</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of timesheets</td> 
   <td> 
    <ul> 
     <li> <p>Timesheet s  &gt;&nbsp;All Timesheets*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of billing rates</td> 
   <td> 
    <ul> 
     <li> <p>Projects &gt; select a project &gt; Billing Rates*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of billing records</td> 
   <td> 
    <ul> 
     <li> <p>Projects &gt;&nbsp;select a project &gt;&nbsp;Billing Records</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of risks</td> 
   <td> 
    <ul> 
     <li> <p>Projects &gt; select a project &gt; Risks</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of expenses</td> 
   <td> 
    <ul> 
     <li> <p>Projects &gt; select a project &gt; Expenses</p> </li> 
     <li> <p>Projects &gt;&nbsp;select a project &gt; Tasks &gt; select a task &gt; Expenses</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List of hour entries</td> 
   <td> 
    <ul> 
     <li> <p>Projects &gt; select a project</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Tasks &gt; select a task &gt; Hours</p> </li> 
     <li> <p>Projects &gt; select a project &gt; Issues &gt; select an issue &gt; Hours</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;You cannot customize the list on the specified area. A Workfront administrator can build a customized list at the system level, or you can build a report for this object if your access level allows you have access to edit reports.

## List elements

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Consider adding Sort to this list.</p>
-->

A list contains certain elements that define its format and the information that displays. You can find several system list elements that are available by default. You can also create custom elements to meet your needs.

>[!NOTE]
>
>When you select a new filter, view or grouping from a list, that selection is retained even if you log out of Workfront or close your browser.

The following are the elements of a list:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Element</th> 
   <th>Explanation</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Filter</strong> </td> 
   <td> <p>Filters keep unnecessary information out of a list, based on the criteria that you specify. </p> <p>For more information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>View</strong> </td> 
   <td> <p>Views define which fields (columns) you display on the screen.</p> <p>For more information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Grouping</strong> </td> 
   <td> <p>Groupings separate the objects on the list in areas based on the criteria that you specify.</p> <p>For example, the issues in a list can display in sections by status or priority.</p> <p>You can have up to 3 layers of groupings in a standard grouping, and you can add a 4th layer if you are configuring a grouping in text mode.</p> <p>For more information about groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> <p>For more information about text mode, see <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Text Mode overview</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

These elements display at the top of every list by default. They are sticky and do not move as you scroll through the list. Mouse over the icon for each element to identify them.

![](assets/nwe-list-elements.png)

You can can customize list elements in the following areas and share them with other users:

* Any system default list found in the section [Get started with lists in Adobe Workfront](#default-workfront-lists) in this article
* Any report that is shared with you

The building elements for lists are the same as the building elements for reports.

For more information about creating and customizing the building elements of lists and reports, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## The difference between the updated and the legacy lists

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider renaming to "The different types of lists"</p>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Maybe break this article up a bit? This section might be good to move out into its own article.</p>
-->

There are two types of lists in Workfront:

* Legacy lists

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Updated lists

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Both types of lists appear in&nbsp;the new Adobe Workfront experience.

All lists and reports in the new Adobe Workfront experience are updated lists, except for the following:

* Lists in the Setup area
* Lists in the Reports area
* Documents lists

The following table shows some of the differences between the legacy and updated lists in Workfront:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Legacy lists</b></td> 
   <td><b>Updated lists</b></td> 
  </tr> 
  <tr> 
   <td> <p>Legacy fonts, column headers, blue grouping color scheme</p> </td> 
   <td> <p>Updated fonts, column headers, gray grouping color scheme</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Slower inline editing</p> </td> 
   <td> <p>Faster inline editing</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Display <strong>100</strong> items by default</p> </td> 
   <td> <p>Display <strong>All</strong> or up to <strong>2000</strong> items by default</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Use CTRL+F to find items in a list</p> </td> 
   <td> <p>Use quick filters to quickly find information in a large list</p> <p>For information about using quick filters in lists, see <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Apply the quick filter to a list</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>You can't inline edit custom fields with rich text formatting.</td> 
   <td> <p>Text in custom fields with formatting can be configured to allow bold, italics, underline, bullets, numbering, hyperlinks, and block quotes.</p> <p>For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Conditional formatting can change the text color of links in a list</td> 
   <td>Cannot apply text color changes to links in a list</td> 
  </tr> 
 </tbody> 
</table>

## The difference between lists and reports

Both lists and reports are grids that contain information about a type of object.

The following table outlines the similarities and differences between lists and reports:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Functionality</strong> </th> 
   <th><strong>List</strong> </th> 
   <th><strong>Report</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Anyone can create them</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Only a Workfront administrator and users with a Plan license can create them</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>A default set is available from Workfront</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Customizable in standard mode</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Customizable in text mode</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>You can share them with other users</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>You can share them system wide</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>You can share them outside of the system</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>You can export to .pdf, Excel, and Tab Delimited formats</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>You can schedule them for delivery in an email</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>You can add to a Layout Template</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>You can add them to custom  sections </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>You can add them to a dashboard</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>You can use prompts to customize what they display</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>You can display them in a chart</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>You can inline edit objects in them</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42; You must have access to Filters, Views, and Groupings to be able to create them. For more information, see [Grant access to filters, views, and groupings](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

&#42;&#42; You must have access to Filters, View, and Groupings as well as Reports, Dashboards, and Calendars to be able to create them. For more information, see [Grant access to reports, dashboards, and calendars](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

&#42;&#42;&#42; You can customize lists for reports that are placed on a dashboard only if the creator of the report has configured the list elements to be visible on the dashboard.

>[!NOTE]
>
>You cannot add a list to a dashboard without creating a report and adding it to the dashboard first.

For more information about building a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). For information about creating custom  sections , see [Create custom tabs or sections](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## List actions

You can complete the following actions in a list:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>Information</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Inline edit</strong> </td> 
   <td> <p>Edit objects and their information directly in the list.</p> <p>For more information, see <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Inline edit items in a list in&nbsp;Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Update with the Summary</strong> </td> 
   <td> <p>Update tasks and issues at the project level using the Summary panel.</p> <p>Tip: The Summary is not available for all objects and it is not available in Task or Issue reports.</p> <p>For more information, see <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Summary overview in the new Adobe Workfront experience</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Customize list display</strong> </td> 
   <td> <p>Customize the look and feel of a list, column arrangement, sorting order of items, or number of items that display.</p> <p>Note: Changes you make to the number of items to display on a page are reverted when you log out of Workfront or close your browser. Changes might also be reverted after a period of 8 hours.</p> <p>For more information, see <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modify how a list displays</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Quick filter</strong> </td> 
   <td> <p>Apply a quick filter to find only items that are important to you so that you can quickly review, update, or share them with others.</p> <p>Important:  You can find items that contain a search word using the quick filter, whether that item is visible on your screen or will display after you scroll to the bottom of the page. When you use your browser's search capabilities, you can find only items that are already visible on the screen. If your list has multiple pages, quick filters find only the items on the current page.</p> <p>For more information, see <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Apply the quick filter to a list</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Export</strong> </td> 
   <td> <p>Export a list of objects from Workfront. When a list contains more than 2000 items, exporting the list is the only way to review all of the items on one page.</p> <p>For more information about exporting a list, see <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Export a list</a>. For more information about export formats and limits, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Export data</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

