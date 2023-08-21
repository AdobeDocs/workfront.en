---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configure sharing for custom fields and widgets with the legacy form builder
description: By default, when you add a new custom field or widget to a custom form, anyone in the system with access to custom forms can edit the properties for that item, such as its label and name. You can change this by controlling who it can be shared with.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
---
# Configure sharing for custom fields and widgets with the legacy form builder

By default, when you add a new custom field or widget to a custom form, anyone in the system with access to custom forms can edit the properties for that item, such as its label and name. You can change this by controlling who it can be shared with.

For information about custom fields and widgets in custom forms, see [Add a custom field to a custom form with the legacy form builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) and [Add or edit an asset widget in a custom form with the legacy form builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Configure sharing for a custom field or widget

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Custom Forms**.
1. If you are configuring sharing for a custom field or widget in your organization's Workfront instance, do the following:

   1. Click the **Fields** tab.
   1. Select the item you want to configure sharing for, then click **Share**.

   Or, if you are configuring sharing for a custom field or widget in an existing custom form, do the following:

   1. Select the custom form, then click **Edit**.
   1. In the form editing area on the right, select the item you want to configure sharing for.
   1. In the left panel, click **Share field**.

1. In the **Custom Field Access** box that displays, specify who you want to share the item with and how you want to share it:

   1. Near the lower-left corner of the **Custom Field Access** box, under **Give custom field access to**, start typing the name of a user, team, job role, group, or company you want to share the item with, then click the name when it appears.

      ![](assets/share-field-give-access-to.jpg)

   1. If you want to be more specific about how you want to share the item, click the drop-down list to the right of the name, then use any of the following options:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">View it</td> 
         <td> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to add the item to a custom form or share it with other users.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Manage it</td> 
         <td> <p>Allows access to edit the custom field and to see it in the Field Library and on the page where you build custom forms.</p> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to delete the item from the system or share it with other users.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Optional) Repeat the previous step to add other names to the list and configure their options.
1. (Optional) Click the gear icon ![](assets/gear-icon-settings.png) in the top-right corner if you want to choose a system-wide sharing option for the field.

   Not all of the following options display in this drop-down menu at the same time. For example, the second one displays only when one of the other two are selected.

   * **Make this editable system-wide so that everyone in Workfront can edit it** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.
   
   * **Remove system-wide edit access**

     Limits access to only those whom you added to the list. 
   
   * **Make this visible system-wide so that everyone in Workfront can see it**

1. Click **Save** or **Save + Close**.

## Inherited access to custom fields and widgets when a custom form is shared

When someone shares a custom form with a group, job role, team, or company, the recipients inherit View access to any custom fields and widgets that are on the form. This level of access to those items on the form is always retained so that the form can function for the recipients as intended by the person who created it. This is true even for recipients who have Edit access to the form.

You can find out who has inherited access to a custom field or widget and you can remove access to it.

>[!NOTE]
>
>If a recipient has Manage access to a custom field or widget on the shared custom form, that access is retained for the recipient.

* [Find out who has inherited access to a custom field or widget](#find-out-who-has-inherited-access-to-a-custom-field-or-widget) 
* [Remove access to a custom field or widget in a custom form that was shared](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Find out who has inherited access to a custom field or widget {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Custom Forms**.
1. Click the **Fields** tab, then select the field, image, or access widget.
1. In the box that displays, click **Inherited Permissions** and view the names that display.
1. Click **Cancel**.

### Remove access to a custom field or widget in a custom form that was shared {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

If you need to remove access to a custom field or widget in a custom form that was shared, you need to unshare the form. For instructions, see in the section [Remove access to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) in the article [Share a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
