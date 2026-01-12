---
title: Grant Administrative Access for a Layout Template
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: As an Adobe Workfront administrator, you can grant administrative access for a layout template to the group administrators of a particular group so that they can edit the template. This does not assign the template to the users in the group.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
---
# Grant administrative access for a layout template

{{preview-fast-release-general}}

As an Adobe Workfront administrator, you can grant administrative access for a layout template to the group administrators of a particular group so that they can edit the template. This does not assign the template to the users in the group.

For information about assigning users to a layout template, see [Assign users to a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

For more information about layout templates, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.</p>
        <p>To perform them for a group, you must be a manager of that group.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Grant administrative access for a layout template

1. Begin working on a layout template, as described in [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Click **Grant access to** in the top section of the page.
1. In the box that appears, click **Add a group**, start typing the name of the group, click the name when it appears, then click **Done**.

   Any users designated as the group administrators for the group you specify can administer the layout template. However, the template is not assigned to the member of the group for their use. For information about assigning a layout template to a group, see [Assign a layout template to users](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) in this article.

   >[!NOTE]
   >
   >* When a group administrator creates a layout template, assigning administrative access is mandatory. The layout template is designated for and visible to only the specified group. For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). For information about group administrators, see [Group administrators](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* If you don't grant administrative access to the group administrators in a particular group, all users who can edit user accounts have administrative access to the layout template. Some Workfront administrators purposefully choose not to grant administrative access for a layout template in order to make it a system-level layout template. 

1. You can click <span class="preview">**Apply**</span> or **Save** at any time to save your progress, then continue to modify the template later.
