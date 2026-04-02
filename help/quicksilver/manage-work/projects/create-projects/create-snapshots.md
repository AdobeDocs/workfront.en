---
product-area: projects
navigation-topic: create-projects
title: Create and View Project Snapshots
description: Snapshots in Adobe Workfront give you a way to see differences between snapshots (taken on a specific date and time) and the project's current data.
author: Lisa
feature: Work Management
hidefromtoc: yes
hide: yes
---
# Create and view project snapshots

{{highlighted-preview-article-level}}

Project managers often need to compare the past data of a project with the current status to make informed decisions and see how their projects have changed over time.

Snapshots in Adobe Workfront give you a way to see these differences between snapshots (taken on a specific date and time) and the project's current data quickly and accurately, helping you to manage projects more effectively and make better decisions. Snapshot comparisons show side-by-side how the project has evolved.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Workflow Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
    <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Access level configuration</td> 
   <td>Edit access to Projects</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>When viewing a snapshot, you can view all fields you have permission to view on the original project </td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a snapshot

1. Go to a project.
1. In the left panel, click **Snapshots**.

   ![Snapshots for a project](assets/snapshot-list.png)

1. Click **New snapshot**.
1. Type a name for the snapshot on the **New snapshot** dialog, and click **Save**.
   
   The snapshot name appears in the list.

   >[!NOTE]
   >
   >When you create a snapshot, it is not available for viewing right away. Based on data running in the background, it could take up to 4 hours to be ready. The Creation Status is **Pending** when the snapshot is not available yet, and **Ready** when you can view it.

## View a single snapshot

1. Go to a project and click **Snapshots** in the left panel.
1. Click a snapshot name in the list to open it. The status must be **Ready** before you can open it.

   >[!TIP]
   >
   >The breadcrumbs at the top of the screen link back to the project and help you identify that you are viewing a snapshot.

   The snapshot displays the following items as they existed at the time the snapshot was created:

   * The hierarchy of tasks and subtasks in the project
   * Project details and any custom forms attached to the details
   * Associated projects and their hierarchy
   * Issues
   * Rates
   * Billing records
   * Expenses <!--* Bookings (on its own line of course when they get released)-->
   * Project team (People tab)

   You can customize any lists in the snapshot by filtering, sorting, adding and removing columns, or applying a view. Time-phased KPIs are available to add to the snapshot view. For more information, see [Customize snapshot lists](#customize-snapshot-lists) in this article.

## Compare snapshots

1. Go to a project and click **Snapshots** in the left panel.
1. Select an option for comparing snapshots:

   * To compare two or more snapshots to each other, select the check boxes next to the snapshots in the list, and click **Compare** in the action bar at the bottom of the screen.
   * To compare snapshots to the current project, select the check boxes next to the snapshots in the list, and click **Compare with current** in the action bar at the bottom of the screen.

      >[!NOTE]
      >
      >The status of each snapshot you want to compare must be **Ready**.

1. On the Comparison screen, expand each snapshot and the current project to see the hierarchy underneath.

   ![Snapshot Comparison screen](assets/snapshot-comparison.png)

1. You can customize the comparison by sorting, adding and removing columns, or applying a view. For more information, see [Customize snapshot lists](#customize-snapshot-lists) in this article.

## Export snapshots

You can export the list of all snapshots or a snapshot comparison in .xlsx or .csv format. All displayed columns are included in the exported file.

1. Click the **Export** icon ![Export icon](assets/export-icon.png) on the snapshot list or snapshot comparison.
1. Select the format for the export file.

   The file is saved to your computer. You may be prompted to choose the location.

1. (Optional) Open the exported list using the appropriate application.

## Customize snapshot lists

You can customize the list of all snapshots, as well as any lists within a snapshot or comparison, by filtering, sorting, adding and removing columns, or applying a view.

For more information about list customizations, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Filter items in a list

Filters help you reduce the amount of information you display in the list.

1. Click **Filter** above the list.
1. In the Filter box, click **Add condition**.
1. Select a field to filter by.
1. Select a filter modifier, such as "Has any of," "Has none of," "Is before," or "Is after." The modifier options are different depending on the type of field you are filtering by.
1. Select the field value or values. Depending on the field type you are filtering by, you might be prompted to select the item from a list, search for it, or use a calendar to select a date range.

   ![Filter the snapshot list](assets/filter-snapshot-list.png)

   The filter is applied to the list automatically.

1. Click **Add condition** to add another condition to the filter.

   You can join multiple filters by an AND or an OR connector.

1. When the filter is applied, you can open the **Filter** options again to change the filter options or clear all of the filters.

   An indicator appears on the **Filter** button when a filter is applied to the list.

   ![Filter applied indicator](assets/glist-filter-applied-indicator.png)

### Sort in a list

To sort individual columns:

1. Hover over the column, then click the down arrow and select **Sort**.

   An icon next to a column name indicates that the list is sorted by the values in that column, and the direction of the sort.
   
   ![Sort the snapshot list](assets/sort-snapshot-list.png)

### Customize columns in a list

You can hide, display, and reorder columns in a list.

1. Click **Columns** above the list.

   ![Columns for snapshot list](assets/hide-display-columns-on-snapshot.png)

1. Use the toggles to display or hide columns in the list.
1. To reorder the columns, click the **Drag** icon ![Drag icon](assets/drag-icon.png) and move a column to your desired location. Moving columns changes the list automatically.

   >[!NOTE]
   >
   >The primary field is the first column in the list. It is fixed in the first position, and you cannot change its column. If the number of columns is large, then the primary field is frozen to the left, and when you scroll horizontally you will always see it.
   >
   >The icon next to a field name shows the field type, such as text or date field.

   An indicator appears on the **Columns** button when columns are hidden. The indicator does not appear when you reorder columns.
   
   ![Indicator for hidden columns](assets/glist-columns-hidden-indicator.png)

### Add and remove columns with the Column manager

You can use the Column manager in some enhanced lists to easily add and remove columns on the list. You can add or remove both system and custom fields that already exist in Workfront as columns.

1. Click the **+** icon on the upper-right corner of the table to open the **Column manager** box.

   ![Column manager for snapshots](assets/column-manager-on-snapshot-no-kpi-tab.png)

1. Search for an existing object field in the **Available** column, then click **+** to the right of the field name it to add it to the **Selected** column.
1. Click **-** to the right of a field in the **Selected** column to remove it from the list.
1. Click **Save**.

   The list updates the columns according to the choices you made.

### Apply a view to a list

To apply or create a view:

1. Click the **Views** dropdown and select an existing view to apply it to the list

   OR

   Click **New view** to create one.

   ![Views menu on a snapshot](assets/views-on-snapshot-list.png)

1. (Conditional) For adding a new view, enter a name for the view, then click **Create**.
1. (Optional) Hide, show, or rearrange the columns. For more information, see [Customize columns in a list](#customize-columns-in-a-list).
1. (Optional) Filter the list. For more information, see [Filter items in a list](#filter-items-in-a-list).

Changes to views are saved automatically. The next time you apply this view, the column and filter settings remain the way you set them. For more information about views, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

