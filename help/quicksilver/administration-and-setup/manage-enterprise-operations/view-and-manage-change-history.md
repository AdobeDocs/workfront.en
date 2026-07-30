---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Change history
description: Change history allows you to view a log of changes to Workfront objects
author: Lisa
feature: System Setup and Administration
role: Admin
---
# View and manage change history

{{preview-fast-release-general}}

You can view change history, including audit logs, in the Change Tracking area of Setup.

* **Audit Logs** are changes triggered by users. 
   For more information on Audit Logs and the Audit Logs area, see [Audit Logs overview](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md) and [View and export audit logs](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).
* **Configuration** displays which field are being tracked for the Change History List. 
   <span class="preview">As a Workfront administrator, you can configure which object fields and actions Workfront tracks. For example, you could have Workfront track all changes users make to the names of issues throughout the system. Any issue name change then appears as an entry on the change history log.</span>

* **Change History List** allows you to view a log of changes to Workfront objects, including attributes such as:

   * Object
   * Object type
   * Type of change (operation)
   * Source of the change, such as specific users, APIs, Workfront Fusion, AI LLMs, or the Workfront system

   <span class="preview">Unified review and approval workflow activity is tracked in Change History, including participants and decisions.</span>

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
   <td><p>System administrator</p>
       <p><span class="preview">To view change history: Administrative access to change history</span></p>
       <p><span class="preview">To configure tracked fields: System administrator</span></p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Add fields you want to track

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
1. On the Configuration screen, click **Add field**.
1. In the **Add fields** box, select an object. You can begin typing the object name, then select it when it appears in the list.
1. Next, select the field names that you want to track for that object. You can being typing the field name, then select it when it appears in the list.

   Both custom fields and native fields are available for the object.
   Fields already being tracked are shown as selected in the list.
   
   ![Add fields for change tracking](assets/change-history-config-add-fields.png)

1. After selecting all of the fields you want to track, click **Add**.
   
   The fields are added to the Tracked Fields list.

## Remove fields you no longer want tracked

You can remove fields you don't want the system to track for a particular type of object throughout the Workfront interface.

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
1. On the Configuration screen, select the field or fields you want to stop tracking.

   You might see the same field name more than once. The fields are grouped by object so you can locate the correct field. You can also use the search box at the top of the screen.

1. Select **Delete** in the action bar at the bottom of the screen.
1. Click **Remove** on the confirmation message.

   The fields are removed from the Tracked Fields list.

</div>

## View the Configuration area for change tracking

>[!NOTE]
>
>In the Production environment, Configuration is currently available only as information and cannot be changed. The ability to change which fields are tracked will be available in the near future.

To view the types of changes that are tracked: 

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > **Configuration**.
   
   Fields are displayed grouped by object type.

1. To display fields under a specific object, click the dropdown arrow next to the object type.

## View the Change History List

Workfront Administrators can view change history in the Setup area.

The Change History List is an enhanced list, and features filters, columns, row height, a date picker, and a search bar.

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Change History List**.

   The Change History List opens.

1. To adjust the dates for which changes display, click the date picker and select the new dates. 

   Changes are available for the last 90 days.

1. To search for a specific term, click the search bar and enter the term. The results are highlighted in the list as you type.
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



