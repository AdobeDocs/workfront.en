---
filename: delete-or-deactivate-a-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Delete or deactivate a custom form
description: You can delete or deactivate a custom form from the system.
---

# Delete or deactivate a custom form

You can delete or deactivate a custom form from the system.

` `**Warning: **``Deleting a custom also deletes all custom data on the objects associated with the form. The deleted data cannot be recovered. Consider deactivating a custom form instead—when deactivate a custom form you no longer use, you retain all of the associated historical data.

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

## Delete a custom form

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Custom Forms.`
1. Select the custom form, then click `Delete`.
1. If you are sure you want to permanently delete the custom form and all associated data on objects where it was attached, click `Yes, Delete It`.

## Deactivate a custom form

You can deactivate custom forms you no longer use without losing their associated historical data. Users can't add an inactive custom form to objects, but they can still view and add data to its fields on objects where it was already attached.

Fields on an inactive custom form are also still available to inline-edit in a View. If a user adds a field from an inactive custom form during an inline edit, the form attaches to the object automatically, even though the custom form is deactivated.

If you re-activeate a custom form, it retains the settings it had before and users can interact with it as if it was never deactivated.

To deactivate a custom form:

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click the name of the custom form you want to deactivate.
1. Click the `Form Settings` tab.
1. Disable the `Is Active` option.
1. Click `Save + Close`.

