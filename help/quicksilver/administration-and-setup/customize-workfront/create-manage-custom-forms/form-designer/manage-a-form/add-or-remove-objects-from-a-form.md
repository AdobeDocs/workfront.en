---
title: Add or Delete Object Types from an Existing Custom Form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can add or remove object types from custom forms with the form designer.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
TQID: https://experienceleague.adobe.com/2nu2y2zDxTQkLnch-M8Z5jcWXw32O0crTbhmt3VjSGg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Add or delete object types from an existing custom form

You can add or delete object types from an existing custom form with the form designer.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>Administrative access to custom forms</p> </td> 
  </tr>  
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

1. Select the custom form you want to add additional object types to, then click ![Edit icon](assets/edit-icon2.png).

1. At the top of the form, click **Object Types**, then select the type you want to add in the menu that displays. You can repeat this to add as many object types as you want. 

   ![Add new object](assets/add-new-object-to-custom-form-041026.png)

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
1. Select the custom form you want to edit, then click ![Edit icon](assets/edit-icon2.png).
1. At the top of the form, click **Object Types**, then clear the check boxes for the objects you want to delete from the form.
1. Click **Apply**, then click **Save and Close**.
