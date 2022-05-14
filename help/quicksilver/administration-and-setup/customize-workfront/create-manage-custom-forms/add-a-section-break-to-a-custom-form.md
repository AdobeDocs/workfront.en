---
filename: add-a-section-break-to-a-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Add a section break to a custom form
description: You can group the custom fields and widgets in a custom form into sections with headings. This is useful for presenting an organized experience to users who will fill out the form. Also, if you need to limit access to certain custom fields and widgets to certain users, you can place them in a section and then grant access to the section to only those users.
---

# Add a section break to a custom form

You can group the custom fields and widgets in a custom form into sections with headings. This is useful for presenting an organized experience to users who will fill out the form. Also, if you need to limit access to certain custom fields and widgets to certain users, you can place them in a section and then grant access to the section to only those users.

For example, if you need to track sensitive information that only system administrators should be able to view or edit, you can create a section break with Admin Only permissions and place the sensitive fields in that section.

The access settings you select for a section are directly tied to the permissions users have on the Workfront object where the custom form is attached. You can hide or show a section based on whether the user has access to view, contribute to, or manage that object. Or you can set a section to Admin Only so that only users with a system administrator access level can access it.

For information about permissions on objects, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

For information about custom fields and widgets in custom forms, see [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) and [Add or edit an asset widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## Access requirements

You must have the following to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Create and configure access for a section in a custom form

1. Begin creating or editing a custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Add custom fields and widgets to the form, as described in [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) and [Add or edit an asset widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. While still creating or editing the custom form, on the **Add a field** tab, click **Section Break**.

   ![](assets/click-section-break-350x200.jpg)

1. On the **Field Settings** tab, configure the options you want for the section:

   <table> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the section. You can change the label at any time.</p> <p>Important: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type text if you want to explain to users what the section is for. This displays below the section's label on the custom form.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Grant access</p> </td> 
      <td> <p> Select the permissions that users need on an object where the custom form is attached in order to view this section and edit its field values. For information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <p>Note:  
        <ul> 
         <li> <p>Users without the permissions you specify here can't see the custom fields and widgets in the section. </p> <p>This is also true if you display the fields' values in reports or use them in calculated fields in text mode reporting.</p> </li> 
         <li> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li> 
        </ul> </p> 
       <ul> 
        <li> <p role="rowheader"><b>Users with this access to the object can view field values</b> </p> 
         <ul>  
          <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p> 
           <ul> 
            <li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li> 
            <li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li> 
           </ul> </li> 
          <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><b>Edit</b>: Manage permissions to the object </li> 
          <li><b>Admin only</b>: System Administrator access level</li> 
         </ul> </li> 
        <li> <p><b><span>Users with this access to the object can edit field values</span></b> </p> 
         <ul> 
          <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p> 
           <ul> 
            <li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li> 
            <li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li> 
           </ul> </li> 
          <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><b>Edit</b>: Manage permissions to the object </li> 
          <li><b>Admin only</b>: System Administrator access level</li> 
         </ul> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Drag or add at least one custom field or widget to the new section.

   This is required before you save the section.

1. Click **Done**.

   >[!TIP]
   >
   >You can click **Apply** at any point while you are creating a custom form to save your changes and keep the form open.

1. If you want to continue building your custom form in other ways, continue on to one of the following articles:

   * [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2) 
   * [Add or edit an asset widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md) 
   * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) 
   * [Position custom fields and widgets in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md) 
   * [Add display logic and skip logic to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md) 
   * [Preview and complete a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
<div style= data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure access for fields without section breaks</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields
<MadCap:conditionalText class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
and widgets
</MadCap:conditionalText>
to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table>
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## How multiple object types can affect section break permissions {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

The Limited Edit permission for custom form section breaks is available for only the Project, Task, Issue, and User object types.

In a custom form with a section break configured with the Limited Edit permission, if you add one of the other object types to the form (Portfolio, Program, Document, Company, Billing Record, Iteration, Expense, or Group), you will be prompted to switch to the Edit permission, which is compatible with both that object type and the existing object types on the form. 

>[!INFO]
>
>**Example:** In a custom form associated with the Project object type, a section break is configured with the Limited Edit permission.
>
>You add the Portfolio object type to the form, which means that the Limited Edit permission option is no longer available for the section break in the form.
>
>An on-screen message prompts you to switch to the Edit permission, which is the most similar option to Limited Edit, and compatible with both the Project object type and the Portfolio object type. 
