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
     <li> <p>Issues</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, issues</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Overview of filters in the Workload Balancer

Consider the following when working with filters in the Workload Balancer:

* Depending on where you access the Workload Balancer from, Workfront might already be filtering the information for you.&nbsp;For information about pre-applied filters, see the section [Pre-applied filters in the Workload Balancer](#pre-appl) in this article. 
* You can create and apply a filter without saving it, or you can save a filter to reuse at a later time. 
* When you apply a filter without saving it, you can revert to the original lists by refreshing your page. 
* You can only view and apply filters you created. Filters created by other users display only for those users. 
* When you save and apply a new filter then navigate away from the Workload Balancer, the filter is preserved even after you log off and log back on. 
* When you create filters in the Workload Balancer in one area, they are not available in other areas. 

  ``` ```**Example: **`````` Filters created in the People area are not available in the Workload Balancer of a project or a team.

  For information about where to locate the Workload Balancer, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* You can view only the items that match the selected filters that also match the dates within the timeline displayed on the screen of the Workload Balancer.

## Pre-applied filters in the Workload Balancer

The Workload Balancer displays information in two separate areas:

* **The Unassigned Work area**: work items that are not yet assigned to users. 
* **The Assigned Work area**: work items that are assigned to users.

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
   <td role="rowheader">The People area</td> 
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
```<li value="1"> <p>Go to the Workload Balancer.</p> <p>For information about accessing the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li>``` ```<li value="2"> <p>Click the <strong>Filter</strong> icon <img src="assets/filter-icon.png"> in the upper-right corner of either the <strong>Unassigned Work</strong> or the <strong>Assigned Work</strong> areas.</p> <p>The list of filters and filter builder box displays on the right. </p> <p>The filter builder box displays on the right. The name of the area you create the filter for displays in the header of the box.</p> <p> <img src="assets/filter-list-empty-state-wb-classic-350x240.png" style="width: 350;height: 240;"> </p> </li>``` ```<li value="3"> <p>(Optional and conditional) If you access the Workload Balancer in the People area, the predefined Default filter might already be applied to the Assigned Work area. You can edit and save a copy of this filter. </p> <note type="tip">  The Default filter displays users that belong to any of your teams and their work items. You can edit a copy of this filter.  </note> <p>If you access the Workload Balancer from a project, select one of the following predefined filters in the Assigned Work area:</p>  <ul>   <li> <p><strong>All work items</strong>: Displays work items assigned to users in this project and their work items in other projects. This is the filter selected by default. You cannot edit this filter.</p> </li>   <li> <p><strong>This project's work items</strong>: Displays only work items assigned to users in this project. You can edit and save a copy of this filter. </p> </li>  </ul> </li>``` ```<li value="4"> <p>Click <strong>New Filter</strong> to create a new filter. </p> <p>The filter builder replaces the list of filters on the right. </p> </li>``` ```<li value="5"> <p>Select a field, then a value that matches what information you want to filter by. </p> <note type="important">  When referencing custom fields, you must type the field name and not the field label. The field label displays on a custom form attached to an object. For information about the difference between the label and the name of a custom field, see   <span href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a></span>  <span>.</span> </note>  <div>   <p>When you select more than one field, the filter assumes that all conditions must apply simultaneously. </p>   <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If you want to filter for items that belong to the Marketing portfolio and are assigned to the Job Role of Designer, the work items must be on projects associated with the Marketing portfolio as well as be assigned to Designers at the same time to display in the Workload Balancer.</p>  </div> </li>``` ```<li value="6"> <p>(Optional) Click <strong>Reset</strong> to clear all the fields you have selected and start building the filter from scratch. </p> </li>``` ```<li value="7"> <p>(Optional) Click <strong>Apply</strong> to apply the filter without saving. </p> <p>The filter displays in the <strong>Unsaved</strong> area of the filter builder as <strong>New Filter</strong>. </p>  <div class="tips" data-mc-autonum="<b>Tips: </b>">  <span class="autonumber"><span><b>Tips: </b></span></span>   <ul>    <li> <p>You cannot rename an unsaved filter. </p> </li>    <li> <p>Unsaved filters are removed from the Workload Balancer next time you log out of Workfront and log back in.</p> </li>    <li> <p>You can have only one unsaved filter at one time. </p> </li>   </ul>  </div> </li>``` ```<li value="8"> <p>Click <strong>Save</strong> to save the filter to use it later, then add a name for the filter in the <strong>Add filter name</strong> field and click <strong>Done</strong>. </p> <p>This saves the filter in the <strong>Saved</strong> section of the filter builder. You can use this filter in the future. </p> <p>The last saved and applied filter displays by default next time you log back in to Workfront.</p> <note type="note">  You can view filters only in the areas of Workfront where you build them.&nbsp;For example, if you save a filter in the People area, it is not available when you access the Workload Balancer of a project or of a team. The filters you create are only visible you and cannot be shared with other users.  </note> </li>``` ```<li value="9"> <p>(Optional) Click the <strong>left-pointing arrow</strong> next to <strong>New Filter</strong> to exit the filter builder and return to the list of filters. </p> </li>``` ```<li value="10"> <p>Click the <strong>X icon</strong> in the upper-right corner of the filter builder to close the filter builder.</p> </li>``` ```<li value="11"> <p>(Conditional) Hover over the <strong>Filter icon</strong> <img src="assets/filter-icon.png"> in the upper-right corner of the <strong>Unassigned Work</strong> or the <strong>Assigned Work</strong> areas to display the name of the filter that is currently applied. A blue dot indicator appears when a filter has already been applied to the list. </p> <p> <img src="assets/wb-filter-with-blue-dot-and-filter-name-350x57.png" style="width: 350;height: 57;"> </img> </p> </li>```  

##

## Edit an existing filter in the Workload Balancer

You can edit a saved filter in the Workload Balancer. 
```<li value="1"> <p>Go to the Workload Balancer.</p> <p>For information about accessing the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li>``` ```<li value="2">Click the <strong>Filter icon</strong> <img src="assets/filter-icon.png"> in the upper-right corner of the <strong>Unassigned</strong> or <strong>Assigned Work</strong> areas. <br>The filter builder displays on the right. </li>``` ```<li value="3"> <p>Expand the <strong>Saved</strong> area in the filter builder, then mouse over the filter you want to edit.</p> <p>Or</p> <p>Expand the <strong>Unsaved</strong> area in the filter builder, then mouse over <strong>New Filter</strong>, then click the <strong>Edit icon</strong> <img src="assets/wb-edit-filter-icon.png">. </p> </li>``` ```<li value="4"> <p>(Conditional) If you selected to edit a saved filter, edit the name of the filter. </p> <p> <img src="assets/wb-editing-filter-name-inline-350x251.png" style="width: 350;height: 251;"> </img> </p> <p>Unsaved filters cannot be renamed. An asterisk displays next to the name of a saved filter when you edited the filter but you have not saved the changes. </p> <p> <img src="assets/edited-filter-with-asterisk.png"> </img> </p> </li>``` ```<li value="5">Update the filter criteria to edit the existing filter and create a new one. For information about creating a filter, see the <a href="#create" class="MCXref xref">Manage filters in the Workload Balancer</a> section in this article. </li>``` ```<li value="6"> <p>(Optional and conditional) Click <strong>Apply</strong> to apply your changes temporarily without saving them. </p> <note type="important">  Unsaved changes to a previously saved filter are deleted when you navigate away from the Workload Balancer.  </note> </li>``` ```<li value="7">Click <strong>Save</strong> to save the changes you made to the existing filter. </li>``` ```<li value="8">(Optional) Click the <strong>left-pointing arrow</strong> next to the name of the filter to exit the filter builder and return to the list of filters. </li>``` ```<li value="9">Click the <strong>X icon</strong> in the upper-right corner of the filter builder to close the filter builder.</li>``` 

##

## Delete a saved filter in the Workload Balancer

Consider the following before deleting a filter:

* You cannot recover deleted filters.
* You cannot delete predefined filters. 
* You cannot delete an unsaved filter. They are removed automatically after logging out and logging back in to Workfront. 
* After you delete all saved filters, the Workload Balancer displays according to the original defaults.&nbsp;

To delete a saved filter:

1. Go to the Workload Balancer
1. Click the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned** or **Assigned Work** areas.   
   The filter builder displays on the right. 

1. Expand the **Saved** area in the filter builder, mouse over the name of a filter, click the **More menu** ![](assets/more-menu.png), then **Delete**.

   ![](assets/wb-more-and-delete-on-saved-filter-350x285.png)

1. Click **Delete** to confirm that you want to remove the filter. 
1. Click the **X icon** in the upper-right corner of the filter builder to close the filter builder.

