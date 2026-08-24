---
user-type: administrator
product-area: system-administration;setup
title: View and Manage Change History
description: Change history allows you to view a log of changes to Workfront objects and fields.
author: Lisa
feature: System Setup and Administration
role: Admin
---
# View and manage change history

{{preview-fast-release-general}}

Change history allows you to configure and track changes to objects and specific fields in Adobe Workfront. The flexible configuration lets you set up which exactly which objects and fields you want to track.

Change history can track the following types of data that you define:

* Activity in the Setup area such as creating or deleting an access level or a job role
* Field-level updates such as editing a project description or changing a user's layout template
* Object updates such as updating a project status or attaching a custom form to a task
* <span class="preview">Unified review and approval workflow activity, including participants and decisions</span>

For information about defining which objects and fields are tracked, see [Configure fields to track in change history](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

On the Change History List, you can view the log of changes to Workfront objects, including attributes such as:

   * Object name
   * Object type
   * Type of change (operation)
   * Date and time of the change
   * Source of the change, such as specific users, APIs, Workfront Fusion, AI LLMs, or the Workfront system

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td><span class="preview">Administrative access to change history</span></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
## View the Configuration area for change tracking

>[!NOTE]
>
>In the Production environment, Configuration is currently available only as information and cannot be changed. The ability to change which fields are tracked will be available in the near future.

To view the types of changes that are tracked: 

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
   
   Fields are displayed grouped by object type.

1. To display fields under a specific object, click the dropdown arrow next to the object type.
-->


## View the Change History List

You can view the change history logs in the Setup area.

The Change History List is an enhanced list, and features filters, columns, row height, a date picker, and a search bar.

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Change History List**.

   The Change History List opens.

1. To adjust the dates for which changes display, click the date picker and select the new dates. 

   Changes are available for the last 90 days.

1. To search for a specific term, click in the search box and enter the term. The results are highlighted in the list as you type.
1. (Optional) To filter by a column, see [Filter items in an enhanced list](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) in the article [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional) To hide, display, or reorder columns, see [Customize columns](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) in the article [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional)To add or remove columns, see [Add and remove columns with the Column manager](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) in the article [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional)To adjust row height, see [Change the row height in a view](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) in the article [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Export change history

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Change History List**.
1. Filter the list to display the items you want to export.
1. Click the **Export** icon ![Export icon](assets/export-icon.png) and select whether you want to save to XLSX or CSV format.

   The save file box opens and you can save the exported file on your computer.
   Finish saving the exported file. You can now find it on your computer and share it with others.



