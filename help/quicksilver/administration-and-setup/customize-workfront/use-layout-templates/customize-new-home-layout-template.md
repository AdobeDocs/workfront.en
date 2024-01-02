---
title: Customize new Home using a layout template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: You can use a Layout Template to configure what users see when they open new Home.
author: Nolan
feature: System Setup and Administration
role: Admin
hide: yes
hidefromtoc: yes
---
# Customize new Home using a layout template

You can use a Layout Template to configure what users see when they open new Home.

You can configure:

* Which widgets display in the workspace by default, and their layout on the page
* Which background is selected
* Specific widget settings, including which filters and groups are available for the My Projects, My Tasks, and My Issues widgets, as well as their defaults

>[!IMPORTANT]
>
>The administrator layout template choices described on this page override individual users' customization choices.
>
>When changes to a layout template are saved, users on that layout template will have their new Home page changed to match the layout template and their existing widget selections will pushed to the bottom of the page. While widgets selected by the administrator may be repositioned and resized by a user, they cannot be removed.

For information about new Home, see [Get started with New Home](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

For information about creating layout templates, see [Create and manage layout templates](../use-layout-templates/create-and-manage-layout-templates.md). 

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

After configuring a layout template, you must assign it to users for changes you made to be visible to others. For information about assigning a layout template to users, see [Assign users to a layout template](../use-layout-templates/assign-users-to-layout-template.md).

## Access requirements

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.
To perform them for a group, you must be a manager of that group.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize new Home using a layout template

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
      <p>This tab essentially functions as a small new Home workspace; as such, it can be customized according to the steps described in <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Add, edit, or remove widgets in new Home</a>. Select widgets and arrange the workspace as you would like it to appear for users.</p>
      <p>To change the background, follow the steps under <b>Background customization</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Get started with New Home</a>.</p>
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
      <p>Once you have selected the widget you would like to edit, available options will display on the right. Currently, these options are <b>Filters</b> and <b>Groups</b>. You can:</p>
      <ul>
        <li><b>Select which Filters or Groups will be available to users:</b><p>Check the box next to all options in the list you would like users to be able to use. Unchecked options will not appear for users.</li></p>
        <li><b>Set a default Filter or Group for the widget:</b><p>Hover your mouse over an option and a button will appear that allows you to set that option as the default for users. The current default will have a blue Default badge to its right.</li></p>
        <li><b>Add an existing Filter or Group to the list of available options:</b><p>Click the plus sign button at the bottom of each list to add an option to that list. Note that only existing Filters or Groups can be added in this way.</li></p>
      </ul>
      </td> 
     </tr>
    </tbody> 
   </table>

1. Continue customizing the layout template.

   Or

   If you are finished customizing, click **Save** in the bottom-left corner.

