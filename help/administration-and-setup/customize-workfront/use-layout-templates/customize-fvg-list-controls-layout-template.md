---
filename: customize-fvg-list-controls-layout-template
title: Customize Filter, View, and Grouping list controls using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
title: Customize Filters, Views, and Groupings using a layout template
description: As an Adobe Workfront administrator, you can use a layout template to specify which list controls appear in the Filter, View, and Grouping drop-down menus. These menus appear above lists throughout Workfront, such as the list of tasks for a project:
---

# Customize Filters, Views, and Groupings using a layout template

As an `Adobe Workfront administrator`, you can use a layout template to specify which list controls appear in the Filter, View, and Grouping drop-down menus. These menus appear above lists throughout `Workfront`, such as the list of tasks for a project:

![](assets/filter-view-grouping---layout-templates-350x98.png)

For more information about layout templates, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

For information about layout templates for groups, see [Create and modify a group’s layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize Filter, View, and Grouping list controls:

<ol> 
 <li value="1">Begin working on a layout template, as described in <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</li> 
 <li value="2"> <p>Click the down arrow <img src="assets/down-arrow-blue.png"> under <span class="bold">Customize what users see</span>, then click <span class="bold">Lists</span> in the drop-down menu that displays.</p> <p> <img src="assets/customize-what-users-see-dropdown-on-pg-adobe-branding-350x180.png" style="width: 350;height: 180;"> </p> </li> 
 <li value="3"> <p>Click the down arrow <img src="assets/down-arrow-blue.png"> under <span class="bold">Select a list to customize</span>, then select the type of <span>Workfront</span> object for which you want to customize the Filter, View, and Grouping list controls.</p> <p> <img src="assets/select-a-list-to-customize-menu-on-pg-adobe-branding-350x161.png" style="width: 350;height: 161;"> </p> <note type="note">  
   <p>If you select Projects as the list to customize, then disable Projects I'm On or Projects I Own in the Filter section, users will no longer see or be able to use that filter:</p> 
   <ul> 
    <li> <p>In the list of filters that displays when they click the filter icon <img src="assets/filter-nwepng.png"> above a list:</p> <p> <img src="assets/disable-filters-projects-im-on-or-own-350x249.png" style="width: 350;height: 249;"> </p> </li> 
    <li> <p>In the header on the Projects area header:</p> <p> <img src="assets/disable-filter-pills-350x115.png" style="width: 350;height: 115;"> </p> <p>For more information about these filters in the Projects area header, see the section <a href="../../../workfront-basics/the-new-workfront-experience/subtabs-removed.md#project" class="MCXref xref">Project lists under a Portfolio</a> in the article <a href="../../../workfront-basics/the-new-workfront-experience/subtabs-removed.md" class="MCXref xref">Subtabs replaced by new main areas or filters in the new Adobe Workfront experience</a>.</p> </li> 
   </ul> 
  </note> </li> 
 <li value="4"> <p>(Optional) If you want to change the default filter, view, or grouping for the layout template, hover over the filter, view, or grouping, then click <span class="bold">Set as default</span>.</p> <p>The defaults you choose determine which Filter, View, and Grouping users will see in lists throughout <span>Workfront</span> when the layout template is assigned to them. If you don’t change these defaults, users see all lists as follows:</p> 
  <ul> 
   <li><span class="bold">Filters</span>: All</li> 
   <li><span class="bold">View</span>: Standard (where applicable; some lists do not have this view)</li> 
   <li> <p><span class="bold">Grouping</span>: Nothing</p> </li> 
  </ul> <p>You can hide the options All, Standard, and Nothing after selecting different defaults (see Step 5), but they can’t be deleted.</p> <p>You can delete any other option being used as a default, but you have to select a different default first.</p> <p>For information about deleting filters, views, and groupings, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md" class="MCXref xref">Create, edit, and share default filters, views, and groupings</a>.</p> </li> 
 <li value="5"> <p>Hide and add list controls as follows:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Hide a list control</td> 
     <td> <p>Clear or check the box next to the list control you want to hide or show.</p> <p>If a checkbox is dimmed, you cannot hide that list control. The Default <img src="assets/default-pill.png"> setting for each list control is dimmed because you can’t hide the setting that is currently configured as the default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Add a custom list control</td> 
     <td> <p> 
       <ol> 
        <li value="1"> Click <span class="bold">Add Filter</span>, <span class="bold">Add View</span>, or <span class="bold">Add Grouping</span> at the bottom of the Filter, View, or Grouping list. In the box that displays, start typing the name of an existing custom list control previously created for your organization, then click the name when it appears.</li> 
        <li value="2"> If you want the new custom list control set as the default filter, view, or grouping for the layout template, click <span class="bold">Set as Default</span>. </li> 
        <li value="3"> <p>Click <span class="bold">Add</span> when you are finished.</p> <note type="note">  
          <p>Users can add custom list controls to their own lists. If you add custom list controls in a layout template, your list controls are added and theirs move to the bottom of the panel; yours do not replace theirs.</p> 
          <p>This is also true if you assign the user to a new layout template that has custom list controls. </p> 
          <p>For information about customizing list controls, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>, and <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> 
         </note> </li> 
       </ol> </p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Continue customizing the layout template.</p> <p>Or</p> <p>If you are finished customizing, click <span class="bold">Save</span>.</p> <note type="tip">
   You can 
   <span class="bold">Save</span> your progress at any time, then continue to modify the template later.
  </note> </li> 
</ol>

