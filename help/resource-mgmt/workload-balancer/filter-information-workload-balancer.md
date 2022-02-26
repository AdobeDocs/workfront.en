---
filename: filter-information-workload-balancer
product-area: resource-management
navigation-topic: the-workload-balancer
title: Manage filters in the Workload Balancer
description: As a resource manager, you can use the Workload Balancer to view and manage the workload of your users. For more general information about the Workload Balancer, see the following articles:
---

# Manage filters in the *Workload Balancer*

As a resource manager, you can use the *Workload Balancer* to view and manage the workload of your users. For more general information about the *Workload Balancer*, see the following articles:

* [Overview of the Workload Balancer](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) 
* [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

To efficiently find work items and to focus on the users you manage, we strongly recommend that you use filters in the *Workload Balancer*. This allows you to display the correct information before you start managing the assignments of your resources.

This article contains information about filters in the *Workload Balancer*. For information about filters in *Workfront*, see [Filters overview in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> <draft-comment>
      <li xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filters, Views, and Groupings</p> </li>
     </draft-comment>
     <li xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filters, Views, and Groupings</p> </li> 
    </ul> <draft-comment>
     <p xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Edit access to Filters, Views, and Groupings when building or editing filters</span> </p>
    </draft-comment><p xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Edit access to Filters, Views, and Groupings when building or editing filters</span> </p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, issues<draft-comment>
      <span xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">,<span data-mc-edit-date="2021-08-31T17:08:19.1487558-04:00" data-mc-editor="alinaw" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2021-08-31T17:08:16.2246621-04:00">filters</span></span>
     </draft-comment><span xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">,<span data-mc-edit-date="2021-08-31T17:08:19.1487558-04:00" data-mc-editor="alinaw" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2021-08-31T17:08:16.2246621-04:00">filters</span></span></p> <draft-comment>
     <p xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Manage permissions to the filters you want to edit or delete</p>
    </draft-comment><p xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Manage permissions to the filters you want to edit or delete</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Overview of filters in the *Workload Balancer*

Consider the following when working with filters in the *Workload Balancer*:

* Depending on where you access the *Workload Balancer* from, *Workfront* might already be filtering the information for you.&nbsp;For information about pre-applied filters, see the section [Pre-applied filters in the Workload Balancer](#pre-appl) in this article. 
* You can create and apply a filter without saving it, or you can save a filter to reuse at a later time. 
* When you apply a filter without saving it, you can revert to the original lists by refreshing your page.

  <!--
  <li xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>You can view filters you created or filters that other users created and shared with you. </p> </li>
  -->

* You can view filters you created or filters that other users created and shared with you.

  <!--
  <li xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>When you delete or edit a shared filter, the filter is also deleted or edited for everyone with whom it is shared. </p> </li>
  -->

* When you delete or edit a shared filter, the filter is also deleted or edited for everyone with whom it is shared. 
* When you save and apply a new filter then navigate away from the *Workload Balancer*, the filter is preserved even after you log off and log back on. 
* When you create filters in the *Workload Balancer* in one area, they are not available in other areas. 

  ` `**Example: **`` Filters created in the 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  Resourcing
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Resourcing </MadCap:conditionalText>`area are not available in the *Workload Balancer* of a project or a team.

  For information about where to locate the *Workload Balancer*, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* You can view only the items that match the selected filters that also match the dates within the timeline displayed on the screen of the *Workload Balancer*.

## Pre-applied filters in the *Workload Balancer*

The *Workload Balancer* displays information in two separate areas:

* `The Unassigned Work area`: work items that are not yet assigned to users. 
* `The Assigned Work area`: work items that are assigned to users.

  For information about what displays in each of the areas, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Each area of the *Workload Balancer* has its own set of filters which work independently from one another. You must configure both filters to indicate what information you want to see in each area.

Depending on where you access the *Workload Balancer* from, the Unassigned and&nbsp;Assigned areas are already filtered by certain criteria, as described in the following table:

<table cellspacing="0"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Workfront</em> area where you access the <em>Workload Balancer</em> </td> 
   <td><b>Items that display in the Unassigned Work area by default</b> </td> 
   <td><b>Items that display in the Assigned Work area by default</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">The <draft-comment>
     <MadCap:conditionalText xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Resourcing 
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Resourcing 
    </MadCap:conditionalText>area</td> 
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

## Create *Workload Balancer* filters

The process for creating filters for the Unassigned Work and Assigned Work areas in the *Workload Balancer* is identical, regardless of where you access the *Workload Balancer* from. For information about locating the *Workload Balancer*, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

You can create a filter from scratch or edit one of the predefined filters. For information about existing filters that you can edit, see the [Edit an existing filter in the Workload Balancer](#edit2) section in this article.

<!--
<div xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<ol>
<li value="1"> <p>Go to the <em>Workload Balancer</em>.</p> <p>For information about accessing the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li>
<li value="2"> <p>Click the <span class="bold">Filter</span> icon <img src="assets/filter-icon.png"> in the upper-right corner of either the <span class="bold">Unassigned Work</span> or the <span class="bold">Assigned Work</span> areas.</p> <p>The filter builder box displays on the right. The name of the area you create the filter for displays in the header of the box.</p> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/new-filters-empty-panel-workload-balancer-350x371.png" style="width: 350;height: 371;"> </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/new-filters-empty-panel-workload-balancer-350x371.png" style="width: 350;height: 371;"> </p> <p> <img src="assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png" style="width: 350;height: 377;"> </p> </li>
<li value="3"> <p>(Optional and conditional) If you access the <em>Workload Balancer</em> in the Resourcing area, the predefined Default filter might already be applied to the Assigned Work area. You can edit and save a copy of the Default filter. </p> <note type="tip">
The Default filter displays users that belong to any of your teams and their work items. You can edit a copy of this filter.
</note> </li>
<li value="4"> <p>Click <span class="bold">New filter</span>, then do the following: </p>
<ol style="list-style-type: lower-alpha;">
<li value="1"> <p>Select a field name in the first drop-down menu or click <span class="bold">Search All&nbsp;Fields</span> to start typing the name of a field that does not display by default and select it.</p> <note type="important">
When referencing custom fields, you must type the field name and not the field label. The field label displays on a custom form attached to an object. For information about the difference between the label and the name of a custom field, see
<span href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a></span>
<span>.</span>
</note> </li>
<li value="2"> <p>(Conditional) If you clicked <span class="bold">Search All&nbsp;Fields</span>, type the name of a field in the <span class="bold">Search</span> field and select it when it displays in the list. </p> <p> <img src="assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png" style="width: 350;height: 386;"> </img> </p>
<div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
<span class="autonumber"><span><b>Tip: </b></span></span>
<p>You can select a field from the following sections:</p>
<ul>
<li> <p><span class="bold">Suggested fields</span>: the fields most commonly used.</p> </li>
<li> <p><span class="bold">Recent selections</span>: the fields you have recently filtered for. </p> </li>
</ul>
</div> </li>
<li value="3"> <p>Select a modifier from the second drop-down menu.</p> </li>
<li value="4"> <p>Select or type a value for the field you are filtering for. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>When you want to display work objects from a specific portfolio, you can apply the following filter: "Portfolio:&nbsp;name contains marketing." This displays work items that belong to any portfolio that contains "marketing" in the name.</p>
<p> <img src="assets/portfolio-name-filter-statement-wb-350x262.png" style="width: 350;height: 262;"> </img> </p>
</div> </li>
<li value="5"> <p>(Optional)&nbsp;Click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> to remove a filter criteria. </p> </li>
</ol> </li>
<li value="5"> <p>(Optional) Click <span class="bold">Add filter</span> to add another filter criteria, then repeat the actions from step 4. </p> </li>
<li value="6"> <p>Click&nbsp;<span class="bold">Apply</span> to apply the results of the filter to the selected <em>Workload Balancer</em> area without saving it. </p> <p>The list of work items updates on the left. </p> <note type="important">
Results display in the
<em>Workload Balancer</em> when all the filter statements that you added are simultaneously true.
</note> <p>The filter is preserved until you refresh the page. </p> <p>The <span class="bold">Apply</span> button is replaced with a <span class="bold">Save as new</span> button. </p> </li>
<li value="7"> <p>Click&nbsp;<span class="bold">Save as new</span> to save the filter for future use. </p> <p> <img src="assets/new-filters-save-as-box-unassigned-area-wb-350x467.png" style="width: 350;height: 467;"> </img> </p> <note type="tip">
Clicking
<span class="bold">Cancel</span> at any time, takes you back to the filter building area.
</note> </li>
<li value="8"> <p>Select <span class="bold">Untitled Filter</span> and enter the name of the new filter instead. </p> </li>
<li value="9"> <p>Select an icon for the new filter from the <span class="bold">Icon</span> drop-down menu. </p> <p> <img src="assets/new-filters-select-icon-expanded-drop-down-wb.png"> </img> </p> </li>
<li value="10"> <p>(Optional) Add a description for the filter to indicate what is unique about it. The description displays under the filter name in the list of filters. </p> </li>
<li value="11"> <p>Click&nbsp;<span class="bold">Save</span>. </p> <p>Saved filters display in the My filters area of the filter box. </p> <p>For information about applying saved filters, see the section <a href="#apply9" class="MCXref xref">Delete a saved filter in the Workload Balancer</a> in this article. </p> </li>
<li value="12"> <p>(Conditional) Hover over the <span class="bold">Filter icon</span><img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned Work</span> or the <span class="bold">Assigned Work</span> areas to display a tooltip with the name or the number of filters that are currently applied. </p> <p> <img src="assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png" style="width: 350;height: 98;"> </p> </li>
</ol>
<h2>Duplicate a filter</h2>
<p>You can duplicate and edit a filter to create a new one. </p>
<ol>
<li value="1"> <p>Go to the <em>Workload Balancer</em>.</p> <p>For information about accessing the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li>
<li value="2"> <p>Click the <span class="bold">Filter</span> icon <img src="assets/filter-icon.png"> in the upper-right corner of either the <span class="bold">Unassigned Work</span> or the <span class="bold">Assigned Work</span> areas.</p> <p>The filter builder box displays to the right. The name of the area you create the filter for displays in the header of the box.</p> </li>
<li value="3"> <p>Hover over an existing filter, click the <span class="bold">More</span> menu <img src="assets/more-menu.png">, then click&nbsp;<span class="bold">Duplicate</span>. </p> <p> <img src="assets/new-filters-duplicate-option-highlighted-wb-350x125.png" style="width: 350;height: 125;"> </img> </p> </li>
<li value="4"> <p>Edit the following information for the duplicated filter:</p>
<ul>
<li> <p>Name</p> <p>By default, the new filter name is "<Original filter name> Copy."</p> </li>
<li> <p>Icon</p> </li>
<li> <p>Description</p> </li>
<li> <p>Any of the fields, modifiers, or values. </p> </li>
</ul> </li>
<li value="5"> <p>(Optional)&nbsp;Click&nbsp;<span class="bold">Add filter</span> to add more statements to the duplicated filter. </p> </li>
<li value="6"> <p>Click <span class="bold">Save</span> to save the duplicated filter in the <span class="bold">My filters</span> area.</p> <p>The original filter remains unchanged and the duplicated filter is saved as a new filter. </p> </li>
</ol>
</div>
-->

<ol> 
 <li value="1"> <p>Go to the <em>Workload Balancer</em>.</p> <p>For information about accessing the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li> 
 <li value="2"> <p>Click the <span class="bold">Filter</span> icon <img src="assets/filter-icon.png"> in the upper-right corner of either the <span class="bold">Unassigned Work</span> or the <span class="bold">Assigned Work</span> areas.</p> <p>The filter builder box displays on the right. The name of the area you create the filter for displays in the header of the box.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/new-filters-empty-panel-workload-balancer-350x371.png" style="width: 350;height: 371;"> </p> <p> <img src="assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png" style="width: 350;height: 377;"> </p> </li> 
 <li value="3"> <p>(Optional and conditional) If you access the <em>Workload Balancer</em> in the Resourcing area, the predefined Default filter might already be applied to the Assigned Work area. You can edit and save a copy of the Default filter. </p> <note type="tip">
   The Default filter displays users that belong to any of your teams and their work items. You can edit a copy of this filter. 
  </note> </li> 
 <li value="4"> <p>Click <span class="bold">New filter</span>, then do the following: </p> 
  <ol style="list-style-type: lower-alpha;"> 
   <li value="1"> <p>Select a field name in the first drop-down menu or click <span class="bold">Search All&nbsp;Fields</span> to start typing the name of a field that does not display by default and select it.</p> <note type="important">
     When referencing custom fields, you must type the field name and not the field label. The field label displays on a custom form attached to an object. For information about the difference between the label and the name of a custom field, see 
     <span href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a></span>
     <span>.</span>
    </note> </li> 
   <li value="2"> <p>(Conditional) If you clicked <span class="bold">Search All&nbsp;Fields</span>, type the name of a field in the <span class="bold">Search</span> field and select it when it displays in the list. </p> <p> <img src="assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png" style="width: 350;height: 386;"> </img> </p> 
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span> 
     <p>You can select a field from the following sections:</p> 
     <ul> 
      <li> <p><span class="bold">Suggested fields</span>: the fields most commonly used.</p> </li> 
      <li> <p><span class="bold">Recent selections</span>: the fields you have recently filtered for. </p> </li> 
     </ul> 
    </div> </li> 
   <li value="3"> <p>Select a modifier from the second drop-down menu.</p> </li> 
   <li value="4"> <p>Select or type a value for the field you are filtering for. </p> 
    <div class="example" data-mc-autonum="<b>Example: </b>">
     <span class="autonumber"><span><b>Example: </b></span></span> 
     <p>When you want to display work objects from a specific portfolio, you can apply the following filter: "Portfolio:&nbsp;name contains marketing." This displays work items that belong to any portfolio that contains "marketing" in the name.</p> 
     <p> <img src="assets/portfolio-name-filter-statement-wb-350x262.png" style="width: 350;height: 262;"> </img> </p> 
    </div> </li> 
   <li value="5"> <p>(Optional)&nbsp;Click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> to remove a filter criteria. </p> </li> 
  </ol> </li> 
 <li value="5"> <p>(Optional) Click <span class="bold">Add filter</span> to add another filter criteria, then repeat the actions from step 4. </p> </li> 
 <li value="6"> <p>Click&nbsp;<span class="bold">Apply</span> to apply the results of the filter to the selected <em>Workload Balancer</em> area without saving it. </p> <p>The list of work items updates on the left. </p> <note type="important">
   Results display in the 
   <em>Workload Balancer</em> when all the filter statements that you added are simultaneously true. 
  </note> <p>The filter is preserved until you refresh the page. </p> <p>The <span class="bold">Apply</span> button is replaced with a <span class="bold">Save as new</span> button. </p> </li> 
 <li value="7"> <p>Click&nbsp;<span class="bold">Save as new</span> to save the filter for future use. </p> <p> <img src="assets/new-filters-save-as-box-unassigned-area-wb-350x467.png" style="width: 350;height: 467;"> </img> </p> <note type="tip">
   Clicking 
   <span class="bold">Cancel</span> at any time, takes you back to the filter building area. 
  </note> </li> 
 <li value="8"> <p>Select <span class="bold">Untitled Filter</span> and enter the name of the new filter instead. </p> </li> 
 <li value="9"> <p>Select an icon for the new filter from the <span class="bold">Icon</span> drop-down menu. </p> <p> <img src="assets/new-filters-select-icon-expanded-drop-down-wb.png"> </img> </p> </li> 
 <li value="10"> <p>(Optional) Add a description for the filter to indicate what is unique about it. The description displays under the filter name in the list of filters. </p> </li> 
 <li value="11"> <p>Click&nbsp;<span class="bold">Save</span>. </p> <p>Saved filters display in the My filters area of the filter box. </p> <p>For information about applying saved filters, see the section <a href="#apply9" class="MCXref xref">Delete a saved filter in the Workload Balancer</a> in this article. </p> </li> 
 <li value="12"> <p>(Conditional) Hover over the <span class="bold">Filter icon</span><img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned Work</span> or the <span class="bold">Assigned Work</span> areas to display a tooltip with the name or the number of filters that are currently applied. </p> <p> <img src="assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png" style="width: 350;height: 98;"> </p> </li> 
</ol>

## Duplicate a filter

You can duplicate and edit a filter to create a new one.

<ol> 
 <li value="1"> <p>Go to the <em>Workload Balancer</em>.</p> <p>For information about accessing the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li> 
 <li value="2"> <p>Click the <span class="bold">Filter</span> icon <img src="assets/filter-icon.png"> in the upper-right corner of either the <span class="bold">Unassigned Work</span> or the <span class="bold">Assigned Work</span> areas.</p> <p>The filter builder box displays to the right. The name of the area you create the filter for displays in the header of the box.</p> </li> 
 <li value="3"> <p>Hover over an existing filter, click the <span class="bold">More</span> menu <img src="assets/more-menu.png">, then click&nbsp;<span class="bold">Duplicate</span>. </p> <p> <img src="assets/new-filters-duplicate-option-highlighted-wb-350x125.png" style="width: 350;height: 125;"> </img> </p> </li> 
 <li value="4"> <p>Edit the following information for the duplicated filter:</p> 
  <ul> 
   <li> <p>Name</p> <p>By default, the new filter name is "<Original filter name> Copy."</p> </li> 
   <li> <p>Icon</p> </li> 
   <li> <p>Description</p> </li> 
   <li> <p>Any of the fields, modifiers, or values. </p> </li> 
  </ul> </li> 
 <li value="5"> <p>(Optional)&nbsp;Click&nbsp;<span class="bold">Add filter</span> to add more statements to the duplicated filter. </p> </li> 
 <li value="6"> <p>Click <span class="bold">Save</span> to save the duplicated filter in the <span class="bold">My filters</span> area.</p> <p>The original filter remains unchanged and the duplicated filter is saved as a new filter. </p> </li> 
</ol>

##

## Edit an existing filter in the *Workload Balancer*

You can edit a saved filter in the *Workload Balancer*.

<!--
<div xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <note type="tip">
When you edit a filter shared with others, they will also see the changes you make.
</note>
<ol>
<li value="1"> <p>Go to the <em>Workload Balancer</em>. </p> <p>For information about accessing the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li>
<li value="2">Click the <span class="bold">Filter icon</span> <img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned</span> or <span class="bold">Assigned Work</span> areas. <br>The filter builder displays on the right. </li>
<li value="3"> <p>In the <span class="bold">My filters</span> area in the filter builder, hover over the filter you want to edit, then click the <span class="bold">Edit icon</span> <img src="assets/wb-edit-filter-icon.png"> .</p> <p> <img src="assets/new-filters-more-menu-options-wb-nwe.png"> </img> </p> </li>
<li value="4"> <p>Do one of the following:</p>
<ul>
<li> <p>Modify any of the filter statements</p> </li>
<li> <p>Click&nbsp;<span class="bold">Add filter</span> to add new filter statements</p> </li>
<li> <p>Click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> to remove existing filter statements.</p> </li>
</ul> </li>
<li value="5"> <p>(Optional)&nbsp;Click&nbsp;<span class="bold">Apply</span>. </p> <p>The results update in the <em>Workload Balancer</em> on the left to illustrate the changes you made to the filter.</p> </li>
<li value="6"> <p>Click&nbsp;<span class="bold">Save.</span> </p> <p>The results update in the <em>Workload Balancer</em> on the left and the filter is updated with the new information you selected. </p> </li>
</ol>
</div>
-->

>[!TIP]
>
>When you edit a filter shared with others, they will also see the changes you make.

<ol> 
 <li value="1"> <p>Go to the <em>Workload Balancer</em>. </p> <p>For information about accessing the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> </li> 
 <li value="2">Click the <span class="bold">Filter icon</span> <img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned</span> or <span class="bold">Assigned Work</span> areas. <br>The filter builder displays on the right. </li> 
 <li value="3"> <p>In the <span class="bold">My filters</span> area in the filter builder, hover over the filter you want to edit, then click the <span class="bold">Edit icon</span> <img src="assets/wb-edit-filter-icon.png"> .</p> <p> <img src="assets/new-filters-more-menu-options-wb-nwe.png"> </img> </p> </li> 
 <li value="4"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p>Modify any of the filter statements</p> </li> 
   <li> <p>Click&nbsp;<span class="bold">Add filter</span> to add new filter statements</p> </li> 
   <li> <p>Click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> to remove existing filter statements.</p> </li> 
  </ul> </li> 
 <li value="5"> <p>(Optional)&nbsp;Click&nbsp;<span class="bold">Apply</span>. </p> <p>The results update in the <em>Workload Balancer</em> on the left to illustrate the changes you made to the filter.</p> </li> 
 <li value="6"> <p>Click&nbsp;<span class="bold">Save.</span> </p> <p>The results update in the <em>Workload Balancer</em> on the left and the filter is updated with the new information you selected. </p> </li> 
</ol>

##

## Delete a saved filter in the *Workload Balancer*

Consider the following before deleting a filter:

* You cannot recover deleted filters.
* You cannot delete predefined filters. 
* You cannot delete an unsaved filter. They are removed automatically after logging out and logging back in to *Workfront*.

  <!--
  <li xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">When you delete a shared filter, it is also deleted for all users that it is shared with. </li>
  -->

* When you delete a shared filter, it is also deleted for all users that it is shared with. 
* After you delete all saved filters, the *Workload Balancer* displays according to the original defaults.&nbsp;

<!--
<div xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <note type="note">
When you delete a filter shared with others, it will also be deleted for them.
</note>
<ol>
<li value="1">Go to the <em>Workload Balancer</em></li>
<li value="2">Click the <span class="bold">Filter icon</span><img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned Work</span> or <span class="bold">Assigned Work</span> areas. <br>The filter builder box displays on the right. </li>
<li value="3"> <p>Hover over a filter in the My filters area, then click the <span class="bold">More</span> menu <img src="assets/more-menu.png">, then click&nbsp;<span class="bold">Delete</span>. </p> <p> <img src="assets/new-filters-delete-option-highlighted-wb-350x116.png" style="width: 350;height: 116;"> </img> </p> </li>
<li style="color: #000000;" value="4"> <p>(Optional)&nbsp;Click&nbsp;<span class="bold">Cancel</span> to avoid the deletion and return to the list of filters. </p> </li>
<li style="color: #000000;" value="5"> <p><span>Click <span class="bold">Delete</span> to confirm the deletion.</span> </p> <p>The filter is deleted for you and all users who had permissions to it. </p> </li>
</ol>
</div>
-->

>[!NOTE]
>
>When you delete a filter shared with others, it will also be deleted for them.

<ol> 
 <li value="1">Go to the <em>Workload Balancer</em></li> 
 <li value="2">Click the <span class="bold">Filter icon</span><img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned Work</span> or <span class="bold">Assigned Work</span> areas. <br>The filter builder box displays on the right. </li> 
 <li value="3"> <p>Hover over a filter in the My filters area, then click the <span class="bold">More</span> menu <img src="assets/more-menu.png">, then click&nbsp;<span class="bold">Delete</span>. </p> <p> <img src="assets/new-filters-delete-option-highlighted-wb-350x116.png" style="width: 350;height: 116;"> </img> </p> </li> 
 <li style="color: #000000;" value="4"> <p>(Optional)&nbsp;Click&nbsp;<span class="bold">Cancel</span> to avoid the deletion and return to the list of filters. </p> </li> 
 <li style="color: #000000;" value="5"> <p><span>Click <span class="bold">Delete</span> to confirm the deletion.</span> </p> <p>The filter is deleted for you and all users who had permissions to it. </p> </li> 
</ol>

<!--
<div xmlns:MadCap="http://www.madcapsoftware.com/Schemas/MadCap.xsd" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2><a name="share"></a>Share a filter in the <em>Workload Balancer</em></h2>
<p>You can share a filter that you created or that was shared with you by other users.</p>
<p>Consider the following when sharing filters in the <em>Workload Balancer</em>:</p>
<ul>
<li> <p><span>You can share filters with active users, teams, roles, and companies or you can make them visible for everyone in your <em>Workfront</em> instance.</span> </p> </li>
<li> <p>Filters you share in the Resourcing area are not visible in the <em>Workload Balancer</em> of a project or a team. </p> </li>
<li> <p><em>Workload Balancer</em> filters that you share with others are not visible in other areas of <em>Workfront</em>.</p> </li>
</ul>
<p>To share a filter: </p>
<ol>
<li value="1">Go to the <em>Workload Balancer</em></li>
<li value="2">Click the <span class="bold">Filter icon</span><img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned Work</span> or <span class="bold">Assigned Work</span> areas. <br>The filter builder box displays on the right. </li>
<li value="3"> <p>Hover over a filter in the My filters area, then click the <span class="bold">More</span> menu <img src="assets/more-menu.png">, then click&nbsp;<span class="bold">Share.</span></p> <p> <img src="assets/new-filters-share-option-highlighted-wb-350x129.png" style="width: 350;height: 129;"> </img> </p> <p>The Filter sharing box displays. </p> </li>
<li value="4"> <p>Enable the <span class="bold">View system wide</span> setting.&nbsp;This gives anyone in <em>Workfront</em> permission to view the filter. </p> <p>Or</p> <p>Start typing the names of users, teams, roles, groups, or companies that you want to share the filter with in the <span class="bold">Give access to</span> field. </p> <p> <img src="assets/new-filters-sharing-ui-wb-350x422.png" style="width: 350;height: 422;"> </img> </p> </li>
<li value="5"> <p>(Optional)&nbsp;Click the right-pointing arrow next to the name of an entity to edit their permissions to the filter, then enable either the <span class="bold">View</span> or <span class="bold">Manage</span> option.</p> <p> <img src="assets/new-filters-granular-permissions-for-manage-wb-350x107.png" style="width: 350;height: 107;"> </img> </p> </li>
<li value="6"> <p>(Optional) Enable or disable the additional permissions for an entity by doing one of the following:</p>
<ol>
<li value="1">Click <span class="bold">View</span> and disable the <span class="bold">Share</span> option. It is enabled by default.</li>
<li value="2"> <p>Click <span class="bold">Manage</span> and disable either the <span class="bold">Share</span> or the <span class="bold">Delete</span> option. They are enabled by default. </p> </li>
</ol> <note type="tip">
Users cannot receive a higher permission than their access level. If they don't have access to Edit filters in their access level, they cannot receive permissions to manage a filter.
<em>Workfront</em> disables the Manage option for these users and the option is dimmed.
</note> </li>
<li value="7"> <p>Click <span class="bold">Share</span>. The filter is shared with the entities you specified. </p> <p>The filters you shared display in the <span class="bold">Shared with me</span> area of the filter box. </p> <p> <img src="assets/new-filters-shared-with-me-area-wb-350x236.png" style="width: 350;height: 236;"> </p> </li>
</ol>
</div>
-->

## Share a filter in the *Workload Balancer*

You can share a filter that you created or that was shared with you by other users.

Consider the following when sharing filters in the *Workload Balancer*:

* `You can share filters with active users, teams, roles, and companies or you can make them visible for everyone in your *Workfront* instance.` 
* Filters you share in the Resourcing area are not visible in the *Workload Balancer* of a project or a team. 
* *Workload Balancer* filters that you share with others are not visible in other areas of *Workfront*.

To share a filter:

<ol> 
 <li value="1">Go to the <em>Workload Balancer</em></li> 
 <li value="2">Click the <span class="bold">Filter icon</span><img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned Work</span> or <span class="bold">Assigned Work</span> areas. <br>The filter builder box displays on the right. </li> 
 <li value="3"> <p>Hover over a filter in the My filters area, then click the <span class="bold">More</span> menu <img src="assets/more-menu.png">, then click&nbsp;<span class="bold">Share.</span></p> <p> <img src="assets/new-filters-share-option-highlighted-wb-350x129.png" style="width: 350;height: 129;"> </img> </p> <p>The Filter sharing box displays. </p> </li> 
 <li value="4"> <p>Enable the <span class="bold">View system wide</span> setting.&nbsp;This gives anyone in <em>Workfront</em> permission to view the filter. </p> <p>Or</p> <p>Start typing the names of users, teams, roles, groups, or companies that you want to share the filter with in the <span class="bold">Give access to</span> field. </p> <p> <img src="assets/new-filters-sharing-ui-wb-350x422.png" style="width: 350;height: 422;"> </img> </p> </li> 
 <li value="5"> <p>(Optional)&nbsp;Click the right-pointing arrow next to the name of an entity to edit their permissions to the filter, then enable either the <span class="bold">View</span> or <span class="bold">Manage</span> option.</p> <p> <img src="assets/new-filters-granular-permissions-for-manage-wb-350x107.png" style="width: 350;height: 107;"> </img> </p> </li> 
 <li value="6"> <p>(Optional) Enable or disable the additional permissions for an entity by doing one of the following:</p> 
  <ol> 
   <li value="1">Click <span class="bold">View</span> and disable the <span class="bold">Share</span> option. It is enabled by default.</li> 
   <li value="2"> <p>Click <span class="bold">Manage</span> and disable either the <span class="bold">Share</span> or the <span class="bold">Delete</span> option. They are enabled by default. </p> </li> 
  </ol> <note type="tip">
   Users cannot receive a higher permission than their access level. If they don't have access to Edit filters in their access level, they cannot receive permissions to manage a filter. 
   <em>Workfront</em> disables the Manage option for these users and the option is dimmed. 
  </note> </li> 
 <li value="7"> <p>Click <span class="bold">Share</span>. The filter is shared with the entities you specified. </p> <p>The filters you shared display in the <span class="bold">Shared with me</span> area of the filter box. </p> <p> <img src="assets/new-filters-shared-with-me-area-wb-350x236.png" style="width: 350;height: 236;"> </p> </li> 
</ol>

