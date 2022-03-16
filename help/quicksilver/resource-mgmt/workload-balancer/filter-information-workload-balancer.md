---
filename: filter-information-workload-balancer
product-area: resource-management
navigation-topic: the-workload-balancer
title: Manage filters in the Workload Balancer
description: As a resource manager, you can use the Workload Balancer to view and manage the workload of your users. For more general information about the Workload Balancer, see the following articles:
---

# Manage filters in the Workload Balancer

As a resource manager, you can use the Workload Balancer to view and manage the workload of your users. For more general information about the Workload Balancer, see the following articles:

* [Overview of the Workload Balancer](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) 
* [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

To efficiently find work items and to focus on the users you manage, we strongly recommend that you use filters in the Workload Balancer. This allows you to display the correct information before you start managing the assignments of your resources.

This article contains information about filters in the Workload Balancer. For information about filters in Workfront, see [Filters overview in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
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
   <td> <p>Plan or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> Filters, Views, and Groupings 
    </ul> Edit access to Filters, Views, and Groupings when building or editing filters <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, issues,filters</p> Manage permissions to the filters you want to edit or delete <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Overview of filters in the Workload Balancer

Consider the following when working with filters in the Workload Balancer:

* Depending on where you access the Workload Balancer from, Workfront might already be filtering the information for you.&nbsp;For information about pre-applied filters, see the section [Pre-applied filters in the Workload Balancer](#pre-appl) in this article. 
* You can create and apply a filter without saving it, or you can save a filter to reuse at a later time. 
* When you apply a filter without saving it, you can revert to the original lists by refreshing your page. 
* When you save and apply a new filter then navigate away from the Workload Balancer, the filter is preserved even after you log off and log back on. 
* When you create filters in the Workload Balancer in one area, they are not available in other areas. 

  ` `**Example: **`` Filters created in the Resourcingarea are not available in the Workload Balancer of a project or a team.

  For information about where to locate the Workload Balancer, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* You can view only the items that match the selected filters that also match the dates within the timeline displayed on the screen of the Workload Balancer.

## Pre-applied filters in the Workload Balancer

The Workload Balancer displays information in two separate areas:

* `The Unassigned Work area`: work items that are not yet assigned to users. 
* `The Assigned Work area`: work items that are assigned to users.

  For information about what displays in each of the areas, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Each area of the Workload Balancer has its own set of filters which work independently from one another. You must configure both filters to indicate what information you want to see in each area.

Depending on where you access the Workload Balancer from, the Unassigned and&nbsp;Assigned areas are already filtered by certain criteria, as described in the following table:

<table cellspacing="0"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront area where you access the Workload Balancer </td> 
   <td><b>Items that display in the Unassigned Work area by default</b> </td> 
   <td><b>Items that display in the Assigned Work area by default</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">The Resourcingarea</td> 
   <td>No items display here by default. You must customize filters to view work items in this area.</td> 
   <td>Users who are members of any of your teams and their work items.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A team</td> 
   <td>Work items that are assigned to the team or the team and a job role. </td> 
   <td> <p>Users who are members of the selected team and their work items that match the timeline selected on the screen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A project</td> 
   <td> <p>Unassigned work items or items assigned to teams or job roles in the selected project display in this area.</p> </td> 
   <td> <p>Users that are assigned to at least one work item on the selected project and their work items on the selected project or on other projects that match the timeline selected on the screen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

## Create Workload Balancer filters

The process for creating filters for the Unassigned Work and Assigned Work areas in the Workload Balancer is identical, regardless of where you access the Workload Balancer from. For information about locating the Workload Balancer, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

You can create a filter from scratch or edit one of the predefined filters. For information about existing filters that you can edit, see the [Edit an existing filter in the Workload Balancer](#edit2) section in this article. 
Go to the Workload Balancer. For information about accessing the Workload Balancer, see Navigate the Workload Balancer. Click the Filter icon in the upper-right corner of either the Unassigned Work or the Assigned Work areas. The filter builder box displays on the right. The name of the area you create the filter for displays in the header of the box. (Optional and conditional) If you access the Workload Balancer in the Resourcing area, the predefined Default filter might already be applied to the Assigned Work area. You can edit and save a copy of the Default filter. Tip: The Default filter displays users that belong to any of your teams and their work items. You can edit a copy of this filter. Click New filter, then do the following: Select a field name in the first drop-down menu or click Search All Fields to start typing the name of a field that does not display by default and select it. Important: When referencing custom fields, you must type the field name and not the field label. The field label displays on a custom form attached to an object. For information about the difference between the label and the name of a custom field, see Create or edit a custom form. (Conditional) If you clicked Search All Fields, type the name of a field in the Search field and select it when it displays in the list. Tip: You can select a field from the following sections: Suggested fields: the fields most commonly used. Recent selections: the fields you have recently filtered for. Select a modifier from the second drop-down menu. Select or type a value for the field you are filtering for. Example: When you want to display work objects from a specific portfolio, you can apply the following filter: "Portfolio: name contains marketing." This displays work items that belong to any portfolio that contains "marketing" in the name. (Optional) Click the Delete icon to remove a filter criteria. (Optional) Click Add filter to add another filter criteria, then repeat the actions from step 4. Click Apply to apply the results of the filter to the selected Workload Balancer area without saving it. The list of work items updates on the left. Important: Results display in the Workload Balancer when all the filter statements that you added are simultaneously true. The filter is preserved until you refresh the page. The Apply button is replaced with a Save as new button. Click Save as new to save the filter for future use. Tip: Clicking Cancel at any time, takes you back to the filter building area. Select Untitled Filter and enter the name of the new filter instead. Select an icon for the new filter from the Icon drop-down menu. (Optional) Add a description for the filter to indicate what is unique about it. The description displays under the filter name in the list of filters. Click Save. Saved filters display in the My filters area of the filter box. For information about applying saved filters, see the section Delete a saved filter in the Workload Balancer in this article. (Conditional) Hover over the Filter icon in the upper-right corner of the Unassigned Work or the Assigned Work areas to display a tooltip with the name or the number of filters that are currently applied. Duplicate a filter You can duplicate and edit a filter to create a new one. Go to the Workload Balancer. For information about accessing the Workload Balancer, see Navigate the Workload Balancer. Click the Filter icon in the upper-right corner of either the Unassigned Work or the Assigned Work areas. The filter builder box displays to the right. The name of the area you create the filter for displays in the header of the box. Hover over an existing filter, click the More menu , then click Duplicate. Edit the following information for the duplicated filter: Name By default, the new filter name is "<Original filter name> Copy." Icon Description Any of the fields, modifiers, or values. (Optional) Click Add filter to add more statements to the duplicated filter. Click Save to save the duplicated filter in the My filters area. The original filter remains unchanged and the duplicated filter is saved as a new filter. 

##

## Edit an existing filter in the Workload Balancer

You can edit a saved filter in the Workload Balancer. 
Tip: When you edit a filter shared with others, they will also see the changes you make. Go to the Workload Balancer. For information about accessing the Workload Balancer, see Navigate the Workload Balancer. Click the Filter icon in the upper-right corner of the Unassigned or Assigned Work areas. The filter builder displays on the right. In the My filters area in the filter builder, hover over the filter you want to edit, then click the Edit icon . Do one of the following: Modify any of the filter statements Click Add filter to add new filter statements Click the Delete icon to remove existing filter statements. (Optional) Click Apply. The results update in the Workload Balancer on the left to illustrate the changes you made to the filter. Click Save. The results update in the Workload Balancer on the left and the filter is updated with the new information you selected.  

##

## Delete a saved filter in the Workload Balancer

Consider the following before deleting a filter:

* You cannot recover deleted filters.
* You cannot delete predefined filters. 
* You cannot delete an unsaved filter. They are removed automatically after logging out and logging back in to Workfront. 
* After you delete all saved filters, the Workload Balancer displays according to the original defaults.&nbsp;

Note: When you delete a filter shared with others, it will also be deleted for them. Go to the Workload Balancer Click the Filter icon in the upper-right corner of the Unassigned Work or Assigned Work areas. The filter builder box displays on the right. Hover over a filter in the My filters area, then click the More menu , then click Delete. (Optional) Click Cancel to avoid the deletion and return to the list of filters. Click Delete to confirm the deletion. The filter is deleted for you and all users who had permissions to it. Share a filter in the Workload Balancer You can share a filter that you created or that was shared with you by other users. Consider the following when sharing filters in the Workload Balancer: You can share filters with active users, teams, roles, and companies or you can make them visible for everyone in your Workfront instance. Filters you share in the Resourcing area are not visible in the Workload Balancer of a project or a team. Workload Balancer filters that you share with others are not visible in other areas of Workfront. To share a filter: Go to the Workload Balancer Click the Filter icon in the upper-right corner of the Unassigned Work or Assigned Work areas. The filter builder box displays on the right. Hover over a filter in the My filters area, then click the More menu , then click Share. The Filter sharing box displays. Enable the View system wide setting. This gives anyone in Workfront permission to view the filter. Or Start typing the names of users, teams, roles, groups, or companies that you want to share the filter with in the Give access to field. (Optional) Click the right-pointing arrow next to the name of an entity to edit their permissions to the filter, then enable either the View or Manage option. (Optional) Enable or disable the additional permissions for an entity by doing one of the following: Click View and disable the Share option. It is enabled by default. Click Manage and disable either the Share or the Delete option. They are enabled by default. Tip: Users cannot receive a higher permission than their access level. If they don't have access to Edit filters in their access level, they cannot receive permissions to manage a filter. Workfront disables the Manage option for these users and the option is dimmed. Click Share. The filter is shared with the entities you specified. The filters you shared display in the Shared with me area of the filter box. 