---
title: Reactivate or deactivate a custom form with the form designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can reactivate or deactivate a custom form. We recommend deactivating custom forms rather than deleting forms you no longer use to retain historical data.
author: Courtney
feature: System Setup and Administration
role: Admin
---

# Reactivate or deactivate a custom form

You can reactivate or deactivate a custom form. We recommend deactivating custom forms rather than deleting forms you no longer use to retain historical data. 

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
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Reactivate a custom form

If you reactivate a custom form, it retains the settings it had before and users can interact with it as if it was never deactivated.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click the name of the custom form you want to deactivate.
1. Click the **Form Settings** tab.
1. Enable the **Is Active** option.
1. Click **Save + Close**.

## Deactivate a custom form

You can deactivate custom forms you no longer use without losing their associated historical data. Users can't add an inactive custom form to objects, but they can still view and add data to its fields on objects where it was already attached.

Fields on an inactive custom form are also still available to inline-edit in a View. If a user adds a field from an inactive custom form during an inline edit, the form attaches to the object automatically, even though the custom form is deactivated.

To deactivate a custom form:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click the name of the custom form you want to deactivate.
1. Click the **Form Settings** tab.
1. Disable the **Is Active** option.
1. Click **Save + Close**.