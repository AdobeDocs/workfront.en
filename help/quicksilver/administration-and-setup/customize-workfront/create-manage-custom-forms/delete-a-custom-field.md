---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Delete a Custom Field or Widget from the System
description: To improve system performance and to make forms easier to use for users, you might want to remove custom fields and widgets from your system when they are no longer being used.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
---
# Delete a custom field or widget from the system

To improve system performance and to make forms easier to use for users, you might want to remove custom fields and widgets from your system when they are no longer being used.

>[!CAUTION]
>
>Deleting a custom field also deletes all custom data that users have entered in the field when filling out custom forms attached to objects. That deleted data cannot be recovered.
>
>You can view all custom forms and reports that use a custom field you want to delete in order to assess what the repercussions might be. For more information, see [View all custom forms that use a particular custom field or widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) and [View all reports that use a particular custom field or widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Or, for a workaround you can use to avoid losing data in fields no longer used, see [Remove a custom field without losing data that users have entered](#remove-a-custom-field-without-losing-data-that-users-have-entered) in this article.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Administrative access to custom forms</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Delete a custom field or widget from the system

{{step-1-to-setup}}

1. Click **Custom Forms.**
1. Click **Fields** to open the Fields area.
1. Select the custom field or widget, then click **Delete**.
1. If you are sure you want to permanently delete the item and (in the case of a custom field) all associated data on objects where it was attached, click **Yes, Delete It**.

## Remove a custom field without losing data that users have entered {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Removing a custom field from a custom form that has over 500 fields and widgets cannot be undone. If you remove the field, you can't re-add it until the form has fewer than 500 fields and widgets.

1. Determine which custom fields you want to remove from the original custom form, but do not remove them at this point.
1. Create a new custom form: 

   1. Add the custom fields to the new form that you want to remove from the original custom form. 
   
      For information, see the section [Add new or existing fields to your custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) in [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
   
   1. Save the new custom form.

1. Limit access to the custom form to only users with administrative access, as described in [Share a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md). 
1. Apply the new custom form to the objects where the original custom form is already applied, as described in [Add a custom form to an object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Applying the new custom form to these objects ensures that historical reporting data is not affected.

1. Modify the original custom form and remove the custom fields that you added to the new form (in Step 2).

   The fields that you removed from the original custom form are now available only on the new custom form that you created. Users are able to see the custom form on the object, but users without administrative access are not able to modify the custom form.
