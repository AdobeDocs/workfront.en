---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filter information in the Workload Balancer
description: To efficiently find work items and to focus on the users or items you manage, we strongly recommend that you use filters in the Workload Balancer.
author: Lisa
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
---
# Filter information in the Workload Balancer

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

As a resource manager, you can use the Workload Balancer to view and manage the workload of your users. For more general information about the Workload Balancer, see the following articles:

* [Workload Balancer overview](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) 
* [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>To efficiently find work items and to focus on the users or items you manage, we strongly recommend that you use filters in the Workload Balancer. This allows you to display the correct information before you start managing the assignments of your resources.
>
>When you save and apply a new filter, then navigate away from the Workload Balancer, the filter is preserved even after you log off and log back on.

This article contains information about filters in the Workload Balancer. For information about filters in Workfront, see [Filters overview](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, when using the Workload Balancer in the Resourcing area</p>
   <p>Work, when using the Workload Balancer of a team or project</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filters, Views, and Groupings</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Edit access to Filters, Views, and Groupings when building or editing filters</span> </p> <p><b>NOTE</b> 
    
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, issues</p>
   <p>Manage permissions to the filters you want to edit or delete</p>
     </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Overview of filters in the Workload Balancer

Consider the following when working with filters in the Workload Balancer:

* Depending on where you access the Workload Balancer from, Workfront might already be filtering the information for you. For information about pre-applied filters, see the section [Pre-applied filters in the Workload Balancer](#pre-applied-filters-in-the-workload-balancer) in this article. 
* You can create and apply a filter without saving it, or you can save a filter to reuse at a later time. 
* When you apply a filter without saving it, you can revert to the original lists by refreshing your page. 
* You can view filters you created or filters that other users created and shared with you. 
* When you delete or edit a shared filter, the filter is also deleted or edited for everyone with whom it is shared. 
* When you create filters in the Workload Balancer in one area, they are not available in other areas. 

  For example, filters created in the Resourcing area are not available in the Workload Balancer of a project or a team.

  For information about where to locate the Workload Balancer, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* You can view only the items that match the selected filters that also match the dates within the timeline displayed on the screen of the Workload Balancer.

## Pre-applied filters in the Workload Balancer {#pre-applied-filters-in-the-workload-balancer}

The Workload Balancer displays information in two separate areas:

* **The Unassigned Work area**: work items that are not yet assigned to users. 
* **The Assigned Work area**: work items that are assigned to users.

  For information about what displays in each of the areas, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Each area of the Workload Balancer has its own set of filters which work independently from one another. You must configure both filters to indicate what information you want to see in each area.

The Workload Balancer displays users and their work items. 
The work items assigned to the users only display when the dates of the items match the time frame displayed on the screen. 

Depending on where you access the Workload Balancer from, the Unassigned and Assigned areas are already filtered by certain criteria, as described in the following table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Workfront area where you access the Workload Balancer</strong></td> 
   <td><b>Items that display in the Unassigned Work area by default</b> </td> 
   <td><b>Items that display in the Assigned Work area by default</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">The Resourcing area</td> 
   <td>No items display here by default. You must customize filters to view work items in this area.</td> 
   <td>Users who are members of any of your teams and their work items. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A team</td> 
   <td>Work items that are assigned to the team or the team and a job role. </td> 
   <td> <p>Users who are members of the selected team and their work items.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A project</td> 
   <td> <p>Unassigned work items or items assigned to teams or job roles in the selected project display in this area.</p> </td> 
   <td> <p>Users that are assigned to at least one work item on the selected project and their work items on the project when the system default filter <b>This project's work items</b> is selected. </p> 
   
   <p>When the system default filter <b>This project's work items</b> is deselected, the Assigned Work area of a project displays all the work items of the users assigned to at least one item on the selected project.  </p> This filter is deselected by default.
   
   <b>NOTE</b>
   <p>You can enable the Show all users option in the Workload Balancer of a project to display all users in the system. For more information, see <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a></p> 
   
   </td> 
  </tr> 
 </tbody> 
</table>

## Create Workload Balancer filters

The process for creating filters for the Unassigned Work and Assigned Work areas in the Workload Balancer is identical, regardless of where you access the Workload Balancer from. For information about locating the Workload Balancer, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

You can create a filter from scratch or edit one of the predefined filters. For information about existing filters that you can edit, see the [Edit an existing filter in the Workload Balancer](#edit-an-existing-filter-in-the-workload-balancer) section in this article.

1. Go to the Workload Balancer.

   For information about accessing the Workload Balancer, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of either the **Unassigned Work** or the **Assigned Work** areas.

   The filter builder box displays on the right. The name of the area you create the filter for displays in the header of the box.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Optional and conditional) If you access the Workload Balancer in the Resourcing area, the predefined Default filter might already be applied to the Assigned Work area. You can edit and save a copy of the Default filter.

   >[!TIP]
   >
   >The Default filter displays users that belong to any of your teams and their work items. You can edit a copy of this filter.

   If you access the [!UICONTROL Workload Balancer] from a project, the "[!UICONTROL This project's work items]" filter might already be applied. This displays only work items assigned to users in this project. You can duplicate and save a copy of this filter. 
   
   By default, the [!UICONTROL Workload Balancer] of a project displays all work items assigned to all users on the project.


1. Click **New filter.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. To create a filter, do the following:

   1. Select a field name in the first drop-down menu or click **Browse fields** to start typing the name of a field that does not display by default.

      >[!IMPORTANT]
      >
      >When referencing custom fields, you must type the field name and not the field label. The field label displays on a custom form attached to an object. For information about the difference between the label and the name of a custom field, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Conditional) If you clicked **Browse fields**, type the name of a field in the **Search** field and select it when it displays in the list.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >You can select a field from the following sections:
      >
      >* **Recent selections**: the fields you have recently filtered for.
      >* **Suggested fields**: the fields most commonly used.
      

   1. Select a modifier from the second drop-down menu. For information about Workfront filter modifiers, see [Filters and condition modifiers](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md). 
   1. Select or type a value for the field you are filtering for. 
   
      >[!NOTE]
      >
      > When you want to display work objects from a specific portfolio, you can apply the following filter: "Portfolio name contains marketing." This displays work items that belong to any portfolio that contains "marketing" in the name.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

      >[!NOTE]
      >
      >To exclude projects in a status of On Hold, you must apply the following filter: "Project: Status does not equal On Hold." This prevents work items from On Hold projects from displaying in the Workload Balancer.

   1. (Optional) Click the **Delete** icon ![](assets/delete.png) to remove a filter criteria.

1. (Optional) Click **Add filter** to add another filter criteria, then repeat the actions from step 4. 

   <!--(NOTE: ensure this stays correct)-->

1. Click **Apply** to apply the results of the filter to the selected Workload Balancer area without saving it.

   The list of work items updates on the left.

   >[!IMPORTANT]
   >
   >Results display in the Workload Balancer when all the filter statements that you added are simultaneously true.

   The filter is preserved until you refresh the page.

   The **Apply** button is replaced with a **Save as new** button. 

1. Click **Save as new** to save the filter for future use.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Clicking **Cancel** at any time, takes you back to the filter building area.

1. Select **Untitled Filter** and enter the name of the new filter instead. 
1. Select an icon for the new filter from the **Icon** drop-down menu.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Optional) Add a description for the filter to indicate what is unique about it. The description displays under the filter name in the list of filters. 
1. Click **Save**.

   Saved filters display in the My filters area of the filter box.

   For information about applying saved filters, see the section [Delete a saved filter in the Workload Balancer](#delete-a-saved-filter-in-the-workload-balancer) in this article. 

1. (Conditional) Mouse over the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or the **Assigned Work** areas to display a tooltip with the name or the number of filters that are currently applied.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Duplicate a filter

You can duplicate and edit a filter to create a new one.

1. Go to the Workload Balancer.

   For information about accessing the Workload Balancer, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of either the **Unassigned Work** or the **Assigned Work** areas.

   The filter builder box displays to the right. The name of the area you create the filter for displays in the header of the box.

1. Mouse over an existing filter, click the **More** menu ![](assets/more-menu.png), then click **Duplicate**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > While editing a filter, you may click the **More** menu in the lower-left corner of the Edit Filter box then click **Duplicate**.

1. Edit the following information for the duplicated filter:

   * Name

     By default, the new filter name is "(Original filter name) Copy."
   
   * Icon
   * Description
   * Any of the fields, modifiers, or values.

1. (Optional) Click **Add filter** to add more statements to the duplicated filter. 
1. Click **Save** to save the duplicated filter in the **My filters** area.

   The original filter remains unchanged and the duplicated filter is saved as a new filter.

## Edit an existing filter in the Workload Balancer {#edit-an-existing-filter-in-the-workload-balancer}

You can edit a saved filter in the Workload Balancer.

>[!TIP]
>
>When you edit a filter shared with others, they will also see the changes you make.

1. Go to the Workload Balancer.

   For information about accessing the Workload Balancer, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Click the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned** or **Assigned Work** areas.   
   The filter builder displays on the right. 

1. Mouse over the filter you want to edit, then click the **Edit** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Do one of the following:

   * Modify any of the filter statements
   * Click **Add filter** to add new filter statements
   * Click the **Delete** icon ![](assets/delete.png) to remove existing filter statements.

1. (Optional) Click **Apply**.

   The results update in the Workload Balancer on the left to illustrate the changes you made to the filter.

1. Click **Save.**

   The results update in the Workload Balancer on the left and the filter is updated with the new information you selected.

## Delete a saved filter in the Workload Balancer {#delete-a-saved-filter-in-the-workload-balancer}

Consider the following before deleting a filter:

* You cannot recover deleted filters.
* You cannot delete predefined filters. 
* You cannot delete an unsaved filter. They are removed automatically after logging out and logging back in to Workfront. 
* When you delete a shared filter, it is also deleted for all users that it is shared with. 
* After you delete all saved filters, the Workload Balancer displays according to the original defaults.

>[!NOTE]
>
>When you delete a filter shared with others, it will also be deleted for them.

1. Go to the Workload Balancer
1. Click the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas.   
   The filter builder box displays on the right. 

1. Mouse over a filter, then click the **More** menu ![](assets/more-menu.png), then click **Delete**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >While editing a filter, you may click the **More** menu in the lower-left corner of the Edit Filter box then click **Delete**.

1. (Optional) Click **Cancel** to avoid the deletion and return to the list of filters. 
1. Click **Delete** to confirm the deletion.

   The filter is deleted for you and all users who had permissions to it.

## Share a filter in the Workload Balancer

You can share a filter that you created or that was shared with you by other users.

Consider the following when sharing filters in the Workload Balancer:

* You can share filters with active users, teams, roles, and companies or you can make them visible for everyone in your Workfront instance. 
* Filters you share in the Resourcing area are not visible in the Workload Balancer of a project or a team. 
* Workload Balancer filters that you share with others are not visible in other areas of Workfront.

To share a filter:

1. Go to the Workload Balancer
1. Click the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas.   
   The filter builder box displays on the right. 

1. Mouse over a filter, then click the **More** menu ![](assets/more-menu.png), then click **Share.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > While editing a filter, you may click the **More** menu in the lower-left corner of the Edit Filter box then click **Share**.

   The Filter sharing box displays. 

1. Enable the **View system-wide** setting. This gives anyone in Workfront permission to view the filter.

   Or

   Start typing the names of users, teams, roles, groups, or companies that you want to share the filter with in the **Give access to** field.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Optional) Click the right-pointing arrow next to the name of an entity to edit their permissions to the filter, then enable either the **View** or **Manage** option.

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Optional) Enable or disable the additional permissions for an entity by doing one of the following:

   1. Click **View** and disable the **Share** option. It is enabled by default.
   
   1. Click **Manage** and disable either the **Share** or the **Delete** option. They are enabled by default.

   >[!TIP]
   >
   >Users cannot receive a higher permission than their access level. If they don't have access to Edit filters in their access level, they cannot receive permissions to manage a filter. Workfront disables the Manage option for these users and the option is dimmed.

1. Click **Share**. The filter is shared with the entities you specified.

   The filters you shared display in the **Shared with me** area of the filter box.

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
