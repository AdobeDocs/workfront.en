---
filename: delete-a-custom-field
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Delete a custom field
description: To improve system performance and to make forms easier to use for users, you might want to remove fields from a custom form when the fields are no longer being used.
---

# Delete a custom field

To improve system performance and to make forms easier to use for users, you might want to remove fields from a custom form when the fields are no longer being used.

>[!IMPORTANT]
>
>Deleting a field also deletes all custom data on the objects associated with the field. The deleted data cannot be recovered.
>
>You can view all custom forms and reports that use a custom field you want to delete in order to assess what the repercussions might be. For more information, see [View all custom forms that use a particular custom field](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) and [View all reports that use a particular custom field](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> Adobe Workfront plan* Any 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> Access level configurations* Administrative access to custom forms For information about how Workfront administrators grants this access, see Grant users administrative access to certain areas. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Delete a custom field

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Custom Forms.</span></li> 
 <li value="3">Click the <span class="bold">Fields</span> tab.</li> 
 <li value="4">Select the custom field, then click <span class="bold">Delete</span>.</li> 
 <li value="5"> <p>If you are sure you want to permanently delete the custom field and all associated data on objects where it was attached, click <span class="bold">Yes, Delete It</span>. </p> </li> 
</ol>

## Remove fields without losing data

` `**Warning: **`` Removing fields from a form that has over 500 fields cannot be undone. Avoid this unless you are certain that you won't need to re-add fields to the custom form in the future. Each time you remove a field, another field cannot be added to the custom form until the custom form has fewer than 500 fields.

1. Determine which fields you want to remove from the original custom form.

   Do not remove any fields from the original custom form at this time.

1. Create a new custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

  1. Add the fields to the new form that you want to remove from the original custom form.
  1. Save the new custom form that includes all of the fields that you are going to remove from the original custom form.

1. Limit access to the custom form to only users with&nbsp;administrative access.&nbsp;
1. Apply the new custom form to the object where the original custom form is already applied, as described in [Add a custom form to an object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Applying the new custom form to the object ensures that historical reporting data is not affected.

1. Modify the original custom form and remove any fields.

   Remove only the fields that you previously&nbsp;added to the new form (in Step 2).

   For information about removing fields from a custom form without losing data that users have entered in those fields, see the section [Remove fields without losing data](#remove)a in the article [Delete a custom field](#).

   The fields that you removed from the original custom form are now available only on the new custom form that you created. Users are able to see the custom form on the object, but users without administrative access are not able to modify the custom form.

