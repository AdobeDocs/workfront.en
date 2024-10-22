---
title: Customize New Home Using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: You can use a Layout Template to configure what users see when they open Home.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
---
# Customize Home using a Layout Template

You can use a Layout Template to configure what users see when they first open Home.

You can configure:

* Which widgets display in the workspace by default
* Which background is selected
* Specific widget settings, including which filters and groups are available for the My Projects, My Tasks, and My Issues widgets, as well as their defaults

>[!IMPORTANT]
>
>End users are able to change their background and reorder widgets on the page after the Layout Template is applied. They are not able to remove widgets included by a Workfront Administrator. 
> <br>
>Administrators have the ability to add new widgets for users. However, if an end user has already customized their widget order or background selection, those specific customizations are not altered.



For information about home, see [Get started with Home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

For information about creating layout templates, see [Create and manage layout templates](../use-layout-templates/create-and-manage-layout-templates.md). 

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

After configuring a layout template, you must assign it to users for changes you made to be visible to others. For information about assigning a layout template to users, see [Assign users to a layout template](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p>
  <p> Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.
To perform them for a group, you must be a manager of that group.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Customize Home using a layout template

To customize Home using a layout template:

1. Begin working on a layout template, as described in [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Click the down arrow ![](assets/dropdown-arrow.png) under **Customize what users see**, then click **Home Workspace**.

1. In the tabs that appear to the right, click either **Design & layout** to choose and arrange widgets and the background, or **Widget settings** to manage settings for individual widgets such as available filters and groups.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design & layout</td> 
      <td>
      <p>Select which widgets will be present in users' workspaces, their position, and choose a background. Note that while users cannot remove the selected widgets, they can move and resize them freely as well as add additional widgets.</p>
      <p>This tab essentially functions as a small Home workspace; as such, it can be customized according to the steps described in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Add, edit, or remove widgets in Home</a>. Select widgets and arrange the workspace as you would like it to appear for users.</p>
      <p>To change the background, follow the steps under <b>Background customization</b> in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Get started with Home</a>.</p>
      <p>

  >[!NOTE]
  >
  >Only moving or resizing widgets in the Layout Template will not trigger users' Home pages to update their layout. However, adding or removing a widget will trigger an update to users' pages.

  </p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Widget settings</td> 
      <td>
      <p>Change settings for individual widgets. Currently, only three widgets are supported:</p>
      <ul>
        <li>My projects</li>
        <li>My tasks</li>
        <li>My issues</li>
      </ul>
      <p>Once you have selected the widget you would like to edit, available options will display on the right. These options include <b>Filters</b>, <b>Columns</b>, and <b>Groups</b>. You can:</p>
      <ul>
      <li><p><b>Select and order Filters, Columns, or Groups available to users:</b></p>
      <p>Check the box next to all options in the list you would like users to be able to use. These options do not extend to the Summary panel. You must configure that area in the Summary tab in the Layout Template. Unchecked options will not appear for users. Drag and drop options in the list to set an order.</li></p>
      <p>

  >[!IMPORTANT]
  >
  >* The Filter, Columns, and Group options are linked to the list customization options in the Layout Template. Changes made here will apply to those settings as well.
  >* Users must have at least Create access to Views in order for administrator column configuration to properly apply to their Home pages.

  </p>
      <li><p><b>Set a default Filter or Group for the widget:</b></p>
      <p>Hover your mouse over an option and a button will appear that allows you to set that option as the default for users. The current default will have a blue Default badge to its right.</li></p>
      <li><p><b>Add an existing Filter, Column, or Group to the list of available options:</b></p>
      <p>Click the plus sign button at the bottom of each list to add an option to that list. Note that only existing Filters, Fields (for Columns), or Groups can be added in this way.</p></li>
      </ul>
      <p>

  >[!NOTE]
  >
  >If you set a default filter or grouping for a specific widget using a layout template, it may not take effect immediately due to existing user preferences. To apply the new filter or grouping immediately, either you or the user may need to reset their user preferences by appending "/resetUser" to the end of their URL.

  </p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. Continue customizing the layout template.

   Or

   If you are finished customizing, click **Save** in the bottom-left corner.

>[!IMPORTANT]
>
>You must refresh the Home page to see customizations from the Layout Template. 
