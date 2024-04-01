---
title: Add or delete object types from an existing custom form with the form designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can add or remove object types from custom forms with the form designer.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
---
# Add or delete object types from an existing custom form with the form designer

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

You can add or delete object types from an existing custom form with the form designer. 

## Access requirements

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
   <td role="rowheader">Access level configurations*</td> 
   <td><p>Administrative access to custom forms</p></td> 
  </tr>  
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Add object types to an existing custom form 

You can add additional object types to the form so that it can be attached to multiple objects. 

>[!NOTE]
>
>Section break permissions can be impacted by the object type. The Limited Edit permission for custom form section breaks is available for only the Project, Task, Issue, and User object types.
>
>For more information, see [How multiple object types can affect section break permissions](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Click **Custom Forms** in the left panel.

   In the view that appears, you can review all custom forms that have been created for your organization. You can also see who created each form, which object type it works with, and whether it is active.

1. Select the custom form you want to add additional object types to, then click **Edit** <span class="preview">or ![Edit icon](assets/edit-icon.png).</span>

1. At the top of the form, click the plus sign + after **Object Types**, then select the type you want in the menu that displays. You can repeat this to add as many object types as you want. 

   ![](assets/add-new-object.png)

1. Click **Save and Close**.

   >[!TIP]
   >
   >You can click **Apply** at any point while you are creating a custom form to save your changes and keep the form open.

## Delete object types on a custom form

You can delete object types from an existing custom form. A custom form must have at least one object type.

>[!CAUTION]
>
>If people have already attached the custom form to objects of the type you want to delete and added data to it, that data is permanently deleted when you delete that object type on the form. It might include historical information that users will need later.
>
>In general, we recommend minimizing the number of times you edit a custom form that is already in use. There is no notification system to alert people who use the custom form about your changes.

To delete an object type: 

{{step-1-to-setup}}

1. Click **Custom Forms** in the left panel.
1. Select the custom form you want to edit, then click **Edit** <span class="preview">or ![Edit icon](assets/edit-icon.png).</span>
1. Click the X on any of the **Object Types** that you want to delete from the form.

   ![](assets/delete-object-types.png)

1. (Optional) Repeat the previous step for any other object type you want to remove from the form.
1. Click **Done**, then click **Save and Close**.
