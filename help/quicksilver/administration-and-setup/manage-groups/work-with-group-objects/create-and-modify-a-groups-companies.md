---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Create and modify a group's companies
description: When you are viewing a group that you manage in the Groups area, you can view and work with companies associated with the group and any of its subgroups.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
---
# Create and modify a group's companies

When you are viewing a group that you manage in the Groups area, you can view and work with companies associated with the group and any of its subgroups.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## View, work with, and create companies for your group from the Groups area

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Click the name of the group for which you want to create or modify companies.
1. In the left panel, click **Companies** to list the companies associated with the group and any subgroups it may have.
1. (Optional) To add a company, click **Add Company**, then configure the company using the options listed below. When you are finished, click **Create Company**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Basic Info section</td> 
      <td> 
       <ul> 
        <li> <p><b>Company Name</b>: Type a name for the company.</p> </li> 
        <li> <p><b>Is Active</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>This is the Primary Company</b>: Assigns the company as your organization's primary company. The primary company typically represents your Workfront account where most of your users work.</p> <p>By modifying their access levels, you can restrict users to see other users:</p> 
         <ul> 
          <li>Only in their primary company</li> 
          <li> <p>In their associated company and the primary company</p> <p>For information about the primary company functionality within users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> <p>You can have only one or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Group</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">The system fills in the <strong>Group</strong> field for the new company with the group you are viewing.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">If you have administrative access to companies in your access level, you can remove the group from the company and assign a different one, or leave the company without a group.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">If you don't have administrative access to companies, the <strong>Group</strong> field is required and you can select only the groups you manage or any subgroups under those groups.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">For information about administrative access to companies, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p> </li> 
        <li> <p><b>Company Members</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Custom Forms section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in Workfront, you can build a custom form and associate it with your company. You can attach this form to your company by selecting it from the drop-down menu. Only active companies are listed in the drop-down menu. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Design a form with the form designer</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >If you have administrative access to companies in your access level, you can also click Add More Companies at the bottom of the list. This adds a row where you can quickly configure the new company.

1. (Optional) To edit or delete companies, select at least one company, then use the toolbar buttons to edit ![](assets/edit-icon.png) or delete ![](assets/delete.png) it.

   For information about editing a company, see the section [Create or edit a company in Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) in the article [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Optional) To export the list of companies, click the Export icon ![](assets/export.png), then select the file format you want for the exported list.
