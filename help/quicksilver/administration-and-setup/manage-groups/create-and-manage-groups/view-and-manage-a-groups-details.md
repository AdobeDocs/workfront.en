---
title: View and Manage a Group's Details
description: You can view and edit the Group Details page for a group or subgroup that you manage.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
---
# View and manage a group's details

You can view and edit the Group Details page for a group or subgroup that you manage. This page includes:

* A description of the group
* The names of the Business Leader and group administrators
* An option that allows you to make the group and its subgroups public or private

  <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

For information about other ways you can manage a group, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

For information about how you can deactivate or reactivate a group, see [Deactivate or reactivate a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md). 

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

+++

## View and manage a group's details

{{step-1-to-setup}}

1. Click **Groups**.

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the top-level group that you want to edit.
1. If you want to deactivate or reactivate the group, 
1. In the left menu, click **Group Details**, then do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>You can type up to 512 characters.</p> <p>If the field is blank, click <strong>Add</strong> to type a description.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Is Active</td> 
      <td> <p>(Enabled by default) Makes the group active in your Workfront instance.</p> <p>In type-ahead fields like the one shown below, when regular users search for a group to attach it to an object or to share an object with it, only active groups display in the list.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>To streamline this for your users, you can disable the Is Active option for groups that are not currently in use.</p> <p>You can easily view, filter and group the Groups list based on active or inactive status using this field. For information about using views, filters, and groupings in lists, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> <p>For information about inactive groups, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Considerations for inactive groups</a> in the article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Delete or deactivate a custom form</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group accessibility</td> 
      <td> <p>(Available only if you are viewing Details for a group, not a subgroup.) Enable or disable the option <strong>Make this group and subgroups private</strong>.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group stakeholders</td> 
      <td> 
       <ul> 
        <li><strong>Group Administrators</strong>: Add or remove users with a Planner license as group administrators for the group. Begin typing the name of a user, then click the name when it appears in the drop-down menu.</li> 
        <li><strong>Business Leader</strong>: Do one of the following:
         <ul>
          <li>If you have not yet assigned a Business Leader for the group, click <strong>Add</strong>, start typing the name of the user you want to assign, then click the person's name when it appears.</li>
          <li>If the group already has a Business Leader and you want to change it, double-click the name of the existing Business Leader. Delete the name, start typing the name of the user you want to assign, then click the person's name when it appears.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add custom form</td> 
      <td>If your access level allows you to manage custom forms, add a custom form to the group. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Custom forms</a>.</td> 
     </tr> 
    </tbody> 
   </table>
