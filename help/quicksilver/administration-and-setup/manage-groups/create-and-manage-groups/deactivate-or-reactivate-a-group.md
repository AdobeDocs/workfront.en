---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Deactivate or Reactivate a Group
description: You can deactivate a group you manage that you no longer use.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
---
# Deactivate or reactivate a group

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

You can deactivate a group you manage that you no longer use.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>Or</p>
       <p>Current: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>You must be a group administrator of the group or a system administrator.</td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Deactivate or reactivate a group

>[!IMPORTANT]
>
>When you deactivate a group, any subgroups below it are also deactivated. 
>
>If you need to reactivate one of them, you can do so after you do one of the following:
>
>* Remove it from its parent group. For more information, see the section [Remove a subgroup from its parent group and make it a top-level group](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in the article [Manage a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Move it under an active group. For more information, see the section [Create, move, view, edit, copy, rename, export, or delete a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) in the article [Manage a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

{{step-1-to-setup}}

1. In the left panel, select **Groups**.

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group to open its page. 

1. Click the More menu ![More icon](assets/more-icon.png) next to the name of the group, then click **Deactivate** or **Reactivate**.    
  
   >[!NOTE]
   >
   >The Is Active option (Reactivate option in Preview) is unavailable if the group is a subgroup of a deactivated group. Before you can reactivate it, you must remove it from its parent group or move it under a group that is active, as described in the Important note above.

1. (Conditional) If you are deactivating the group, click **Deactivate** in the **Deactivate group** box that displays.  

## Considerations for inactive groups

Consider the following about a group that you deactivate by disabling the Is Active option explained in the section [Deactivate or reactivate a group](#View) in this article.

* Deactivating a group also deactivates all subgroups below it. This includes subgroups that you add after you deactivate it.

  For information about re-activating a subgroup in this situation, see [About reactivating a subgroup below an inactive parent group](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in this article.

* When you go to the Groups area in Setup, you can see only active groups in the list because Active is the default filter ![Filter icon](assets/filter-nwepng.png) for it. If you want to see all of the groups you manage, including the inactive ones, you can use the All filter. Or use the Inactive filter to list only the inactive ones.

  For more information about filters in lists, see [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Deactivating a group does not change the following:

   * The group's associations to objects. Associated objects continue to function as they did before, without any changes.

     For example, if a project is associated with a group you deactivate, the project continues to use the group's preferences and statuses without any changes.
   
   * Your ability to create a new object, such as an approval, team, or company, from within the group's page in setup. By default, the new object is associated with the inactive group.
   * Your ability, as an administrator, to find the group in filters and reporting.

     You can also find it in group type-ahead fields where you might want to manage the group's settings in the Setup area. This includes the Preferences, Event Notifications, and System Licenses areas.

     For example, if you go to Setup > Project Preference > Projects and clear the type-ahead field above the options there, you can still find an inactive group and configure its project preferences.

## About reactivating a subgroup below an inactive parent group {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Deactivating a group also deactivates all subgroups below it. If you need to reactivate one of the subgroups under an inactive group, you can do one of two things:

* Move the subgroup under an active group. Then enable the Is Active option for the moved group, as explained in the section [Deactivate or reactivate a group](#View) in this article.

  For instructions on moving a group, see [Move a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Remove the subgroup from its parent group (which makes the subgroup a top-level group). Then enable the Is Active option for the moved group, as explained in the section [Deactivate or reactivate a group](#View) in this article.

  For instructions on removing a subgroup from its parent group, see the section [Remove a subgroup from its parent group and make it a top-level group](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in the article [Manage a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
