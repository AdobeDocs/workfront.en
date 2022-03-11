---
filename: create-and-modify-a-groups-companies
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Create and modify a group’s companies
description: When you are viewing a group that you manage in the Groups area, you can view and work with companies associated with the group and any of its subgroups.
---

# Create and modify a group’s companies

When you are viewing a group that you manage in the Groups area, you can view and work with companies associated with the group and any of its subgroups.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for `Workfront administrators` (for any group).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> <p>You must be a <span>group administrator</span> of the group or a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your `Workfront administrator`.

## View, work with, and create companies for your group from the Groups area

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Groups</span> <img src="assets/groups-icon.png">.</li> 
 <li value="3">Click the name of the group for which you want to create or modify <span>companies</span>.</li> 
 <li value="4">In the left panel, click <span class="bold">Companies <img src="assets/companies-icon-left-panel-group-pg.png"></span> to list the companies associated with the group and any subgroups it may have.</li> 
 <li value="5"> <p>(Optional) To add a company, click <span class="bold">Add Company</span>, then configure the company using the options listed below. When you are finished, click <span class="bold">Create Company</span>.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Basic Info section</td> 
     <td> 
      <ul> 
       <li> <p><b>Company Name</b>: Type a name for the company.</p> </li> 
       <li> <p><b>Is Active</b>: When this option is enabled, users can find the <span>company</span> and attach it to projects that they create and edit. An inactive <span>company</span> cannot be attached to projects. This option is enabled by default.</p> </li> 
       <li> <p><b>This is the Primary Company</b>: Assigns the company as your organization's primary company. The primary company typically represents your <span>Workfront</span> account where most of your users work.</p> <p>By modifying their access levels, you can restrict users to see other users:</p> 
        <ul> 
         <li>Only in their primary company</li> 
         <li> <p>In their associated company and the primary company<br></p> <p>For information about the primary company functionality within users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> <p>You can have only one or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </li> 
        </ul> </li> 
       <li> <p><b>Group</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for <span>group administrators</span> who need to report on and manage all the companies that their groups do business with.</p> The system fills in the Group field for the new company with the group you are viewing. If you have administrative access to companies in your access level, you can remove the group from the company and assign a different one, or leave the company without a group. If you don’t have administrative access to companies, the Group field is required and you can select only the groups you manage or any subgroups under those groups. For information about administrative access to companies, see Grant users administrative access to certain areas. </li> 
       <li> <p><b>Company Members</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Billing Rates section</td> 
     <td> <p>You can override billing rates associated with your job roles at the company level. For information about creating job roles and associating them with billing rates, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">Create and manage job roles</a>.</p> <p>For more information about overriding billing rates at the company level, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">Override job role billing rates at the company level</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Custom Forms section</td> 
     <td> <p>If there are fields that you want to add to your company that are not available in <span>Workfront</span>, you can build a Custom Form and associate it with your company. You can attach this form to your company by selecting it from the drop-down menu. Only active companies are listed in the drop-down menu. For information about creating Custom Forms, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Create or edit a custom form</a>. </p> </td> 
    </tr> 
   </tbody> 
  </table> <note type="tip">
   If you have administrative access to companies in your access level, you can also click Add More Companies at the bottom of the list. This adds a row where you can quickly configure the new company. 
  </note> </li> 
 <li value="6"> <p>(Optional) To edit or delete companies, select at least one company, then use the toolbar buttons to edit <img src="assets/edit-icon.png"> or delete <img src="assets/delete.png"> it.</p> <p>For information about editing a company, see the section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront" class="MCXref xref">Create or edit a company in Workfront</a> in the article <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Create and edit companies</a>.</p> </li> 
 <li value="7">(Optional) To export the list of companies, click <span class="bold">Export</span><!--
  -->, then select the file format you want for the exported list.</li> 
</ol>

