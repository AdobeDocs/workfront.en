---
title: Organize and preview a form with the Form Designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can organize a custom form with the Form Designer.
author: Courtney
feature: System Setup and Administration
role: Admin
---

# Organize and preview a form with the form designer

 You can organize a custom form with the form designer.

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>
   <p>Current plan: Standard</p>
   <p>or</p>
   <p>Legacy plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Add a section break

You can group the custom fields and widgets in a custom form into sections with headings. This is useful for presenting an organized experience to users who will fill out the form. Also, if you need to limit access to certain custom fields and widgets to certain users, you can place them in a section and then grant access to the section to only those users.

For example, if you need to track sensitive information that only system administrators should be able to view or edit, you can create a section break with Admin Only permissions and place the sensitive fields in that section.

The access settings you select for a section are directly tied to the permissions users have on the Workfront object where the custom form is attached. You can hide or show a section based on whether the user has access to view, contribute to, or manage that object. Or you can set a section to Admin Only so that only users with a system administrator access level can access it.

For information about permissions on objects, see [Overview of sharing permissions on objects](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

For information about custom fields and widgets in custom forms, see [Design a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Create and configure access for a section in a custom form

1. Begin creating or editing a custom form and adding fields, as described in [Design a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click **Section Break** and drag it into the desired position on the canvas.

1. In the right panel, configure the options you want for the section:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the section. You can change the label at any time.</p> <p><b>IMPORTANT</b>: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type text if you want to explain to users what the section is for. This displays below the section's label on the custom form.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Grant access</p> </td> 
      <td> <p> Select the permissions that users need on an object where the custom form is attached in order to view this section and edit its field values. 
       <p>The following permissions are available under <b>Users with this access to the object can view field values</b>:</p> 
         <ul>  
          <li><p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p> 
          <p>Allows users to contribute to the object if it's a project, task, or issue.</p>
          <p>Allows users  to edit the profile or own the profile permission to the object if it's a user.</p></li> 
          <li><b>Edit</b>: Manage permissions to the object </li> 
          <li><b>Admin only</b>: System Administrator access level</li> 
         </ul> </li> 
        <p>The following permissions are available under <b>Users with this access to the object can edit field values</b>: </p> 
         <ul> 
          <li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p> 
           <p>If the object a project, task, or issue, this permission allows users to contribute to the object</p>
          <p>If the object is a user, this permission allows users to edit the profile or own the profile permission to the object.</p> 
          <li><b>Edit</b>: Manage permissions to the object </li> 
          <li><b>Admin only</b>: System Administrator access level</li> 
         </ul> </li> 
       </ul> 
       <p>For information about permissions on objects, see <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li> <p>Users without the permissions you specify here can't see the custom fields and widgets in the section. </p> <p>This is also true if you display the fields' values in reports or use them in calculated fields in text mode reporting.</p> </li> 
       <li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Drag or add at least one custom field or widget to the new section. This is required before you save the section.

1. Click **Done**.

   >[!TIP]
   >
   >You can click **Apply** at any point while you are creating a custom form to save your changes and keep the form open.

### How multiple object types can affect section break permissions {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

The Limited Edit permission for custom form section breaks is available for only the Project, Task, Issue, and User object types.

In a custom form with a section break configured with the Limited Edit permission, if you add one of the other object types to the form (Portfolio, Program, Document, Company, Billing Record, Iteration, Expense, or Group), you will be prompted to switch to the Edit permission, which is compatible with both that object type and the existing object types on the form. 

>[!INFO]
>
>**Example:** In a custom form associated with the Project object type, a section break is configured with the Limited Edit permission.
>
>You add the Portfolio object type to the form, which means that the Limited Edit permission option is no longer available for the section break in the form.
>
>An on-screen message prompts you to switch to the Edit permission, which is the least level of permissions compatible with both the Project object type and the Portfolio object type.


## Position custom fields and widgets in a custom form

 
1. Begin creating or editing a custom form, as described in [Design a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. To position custom fields and widgets on the same row, drag one next to the other until a line appears between them.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

   >[!NOTE]
   >
   >* You can use the **Preview** button in the upper-right corner to get an idea of how the custom fields and widgets will display in the form.
   >* Custom fields and widgets may not always display the same way in the form, depending on how much screen space is available when a user is viewing it. For example, the third field in a row of fields may wrap to the next row of fields if horizontal space is limited.

1. (Optional)To position a custom field or widget above or below another one, drag it above or below until a horizontal blue line appears between the items.

1. To save your changes, click **Apply** 

    or

    Click **Save and Close**. 

## Preview a custom form

1. Begin creating or editing a custom form and adding fields, as described in [Design a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click **Preview** in the top-left corner to see how the form will look when being used, then click **End Preview** to return to editing the form. 