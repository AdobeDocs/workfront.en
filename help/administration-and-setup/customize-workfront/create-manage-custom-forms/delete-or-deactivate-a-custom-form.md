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
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> Access level configurations* Administrative access to custom forms For information about how Workfront administrators grants this access, see Grant users administrative access to certain areas.  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your `Workfront administrator`.

## Delete a custom form

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Custom Forms.</span></li> 
 <li value="3">Select the custom form, then click <span class="bold">Delete</span>.</li> 
 <li value="4"> <p>If you are sure you want to permanently delete the custom form and all associated data on objects where it was attached, click <span class="bold">Yes, Delete It</span>. </p> </li> 
</ol>

## Deactivate a custom form

You can deactivate custom forms you no longer use without losing their associated historical data. Users can't add an inactive custom form to objects, but they can still view and add data to its fields on objects where it was already attached.

Fields on an inactive custom form are also still available to inline-edit in a View. If a user adds a field from an inactive custom form during an inline edit, the form attaches to the object automatically, even though the custom form is deactivated.

If you re-activeate a custom form, it retains the settings it had before and users can interact with it as if it was never deactivated.

To deactivate a custom form:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click the name of the custom form you want to deactivate.</li> 
 <li value="3">Click the <span class="bold">Form Settings</span> tab.</li> 
 <li value="4">Disable the <span class="bold">Is Active</span> option.</li> 
 <li value="5">Click <span class="bold">Save + Close</span>.</li> 
</ol>

