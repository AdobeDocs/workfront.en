---
title: Configure Sharing for Custom Fields and Widgets
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: By default, when you add a new custom field or widget to a custom form, anyone in the system with access to custom forms can edit the properties for that item, such as its label and API name. You can change this by controlling who it can be shared with.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
TQID: 'https://experienceleague.adobe.com/KyrIWEpIQQb-f8YODUPz3-RbP5wFww8Vu7Ffy33wUog'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
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
# Configure sharing for custom fields and widgets

By default, when you add a new custom field or widget to a custom form, anyone in the system with access to custom forms can edit the properties for that item, such as its label and API name. You can change this by controlling who it can be shared with.

For information about custom fields and widgets in custom forms, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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

## Configure sharing a custom field or widget

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. To share from the list of forms and fields:
   
   1. Click **Fields** to open the Fields area.
   1. Select the field you want to share, then click ![Share icon](assets/share-icon.png).

1. To share from the form designer:
   1. Open a custom form or create a new custom form.
   1. In the form designer, select the field you want to share, then click **Share** in the field editing area on the right.

1. In the sharing box, under **Grant field access to**, start typing the name of the user, team, job role, group, company, or business profile you want to share the item with, then press **Enter** when the name displays.
1. If you want to be more specific about how you share the item, click the drop-down menu to the right of the name, then use any of the following options:

   * **View**: Click the **Advanced Settings** icon ![Advanced Settings icon](assets/configure-options-icon.png) to specify whether you want the users to be able to add the item to a custom form or share it with other users.
   * **Manage**: Allows access to edit the custom field and see it both in the Field library and in the form designer. Click the **Advanced Settings** icon ![Advanced Settings icon](assets/configure-options-icon.png) to specify whether you want the users to be able to delete the item from the system or share it with other users.

1. (Optional) Repeat Steps 5-6 to add other names to the list and configure their options.
1. (Optional) Choose a system-wide sharing option for the field:

   * **Everyone in the system can edit** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.

   * **Everyone in the system can view**

      Everyone in the system who has access to custom forms can view the field but not edit it.

   * **Only invited people can access**

     Limits access to only those you added to the list.

   ![Sharing options](assets/share-field-in-designer.png)

1. Click **Save**.

## Inherited access to custom fields and widgets when a custom form is shared

When someone shares a custom form with a group, job role, team, company, or business profile, the recipients inherit View access to any custom fields and widgets that are on the form. This level of access to those items on the form is always retained so that the form can function for the recipients as intended by the person who created it. This is true even for recipients who have Edit access to the form.

You can find out who has inherited access to a custom field or widget and you can remove access to it.

>[!NOTE]
>
>If a recipient has Manage access to a custom field or widget on the shared custom form, that access is retained for the recipient.

### Find out who has inherited access to a custom field or widget {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Click **Fields**, then select the field, image, or access widget.
1. In the box that displays, click **Inherited Permissions** and view the names that display.
1. Click **Cancel**.

### Remove access to a custom field or widget in a custom form that was shared {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

If you need to remove access to a custom field or widget in a custom form that was shared, you need to unshare the form. For instructions, see the section [Remove access to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form) in the article [Share a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).


