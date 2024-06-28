---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Manage custom forms attached to objects
description: You can update the order in which the custom forms attached to one object display, remove them, or bulk-edit the way custom forms display on multiple objects.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
---
# Manage custom forms attached to objects

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

You can update the order in which the custom forms attached to one object display, remove them, or bulk-edit the way custom forms display on multiple objects.

## Access requirements

You must have the following access to perform the actions described in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the objects for which you manage custom forms</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

* Your Workfront administrator or a Plan user with administrative access to custom forms must create custom forms in your environment. For more information, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* You must have custom forms attached to an object.

  For information about how to apply custom forms to an object, see [Add a custom form to an object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Reorder multiple custom forms attached to an object {#reorder-multiple-custom-forms-attached-to-an-object}

1. Go to the object where you want to change the order of the added custom forms, ,then start to edit the object.

   **Example:** For example, to manage the custom forms of a project, go to the project,  click the **More** menu ![](assets/more-icon.png), then click **Edit** .

1. In the **Custom Forms** section for projects, tasks, and issues, click the ![](assets/move-icon---dots.png) icon next to the name of a custom form. For all other objects, click **Manage Forms**. This option displays only if at least one custom form is attached to the object.
1. Drag a form ![](assets/move-icon---dots.png) to a new location in the list.
1. For projects, tasks, and issues custom forms, click **Save**.

   For all other objects, click **I'm done managing** >&nbsp;**Save Changes**.

## Remove a custom form from an object {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>When you remove a custom form from an object, all the information captured in the custom fields of the form is lost and cannot be recovered.

1. Go to the object where you want to remove&nbsp;the custom form and start editing the object.

   For example, go to a project,  click the **More** menu ![](assets/more-icon.png), then click **Edit** .

1. Click **Custom Forms**.
1. For projects, tasks, and issues custom forms, click the **X**&nbsp;icon to the right of a form to remove it from the object.

   For all other objects, click **Manage Forms**, then click the **X** icon to the right of a form to remove it from the object.

1. Click **Save** .

## Manage multiple custom forms that contain the same custom fields

You might have the same field appear on multiple custom forms attached to the same object. In this case, consider the following:

* The value of the field is identical in all forms.

  You cannot have different values for the same fields on different forms attached to the same object.

* If you have the same calculated fields on two different objects, their calculations must be identical to avoid errors. For information about adding calculated fields to custom forms including multiple forms, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Manage multiple custom forms when bulk-editing objects

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Managing custom forms to objects is identical for all objects except for projects. 
>
>For information about adding custom forms to projects in bulk, see the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).

When you are bulk editing objects that have multiple custom forms applied, you can edit the way custom forms are displayed on those objects, as well as edit common fields among the custom forms.

Only the custom forms that are attached to all selected objects can be edited in a bulk edit.

To edit multiple custom forms when editing objects in bulk:

1. In a list objects, select the objects where the custom forms are attached, then click  the **Edit** icon ![](assets/edit-icon.png).
1. Click **Custom Forms**.

   You can edit only the custom forms attached to all of the selected objects.

   Custom forms attached only to some of the objects do not display.

1. Start editing fields on the custom forms.

   When fields are edited, a visual indicator is shown on the field, showing that the field has been edited.

   If a field is included on more than one custom form, all values of those fields are updated on each form when you update the field on one of the forms.

1. Click the **Make a selection** drop-down menu and select additional forms to add to all the selected objects.

   Consider the following when applying additional forms:

   * Objects can have up to 10 custom forms.
   * You can apply forms only when the form is not already applied to any of the objects that you are editing. A form that is already attached to one of the objects does not appear in the drop-down menu.
   * After you apply an additional form, any fields that form has in common with other forms are displayed in the **Common Fields** section, and they can be edited.

1. (Optional) If you added custom forms to all the objects, but you have not saved the objects yet, you can change the order in which the custom forms appear on the objects.

   For more information about changing the order of the forms, see [Reorder multiple custom forms attached to an object](#reorder-multiple-custom-forms-attached-to-an-object) in this article.

1. Click **Remove Form** to remove a custom form from the objects.

   For more information about removing custom forms from objects, see [Remove a custom form from an object](#remove-a-custom-form-from-an-object).

   Consider the following when removing forms in bulk from several objects:

   * If you have made changes to the form, removing it results in your changes being lost and they cannot be recovered.
   * After you remove a form, any fields from that form that were in the **Common Fields** section are removed from this section and can no longer be edited here.

1. Click&nbsp;**Restore Form** to restore the form to the state it was in before you edited the objects.
1. (Optional) Click the collapse arrow next to the name of the form to collapse one form at a time.

   Or

   Click **Collapse Forms** to collapse all forms at the same time.

1. (Optional) Click the expand arrow next to the name of the form to expand one form at a time.

   Or

   Click **Expand Forms** to expand all forms at the same time.&nbsp;

1. Click **Save Changes**.
