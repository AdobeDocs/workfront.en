---
title: Design a form from a copy with the form designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can design a custom form from a copy with the form designer.
author: Courtney
feature: System Setup and Administration
role: Admin
---

# Design a form from a copy with the form designer

{{highlighted-preview-article-level}}

You can design a new custom form that is based on an existing one. You can attach custom forms to different Workfront objects to capture data about those objects.

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
   <td>
   <p>Current plan: Standard</p>
   <p>or</p>
   <p>Legacy plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Copy a custom form to create a new one

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms.**
1. Select the custom form that you want to use as the basis for a new custom form, then click **Copy**.
1. In the **Custom Form Copy** box that appears, type the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Form Name</td> 
      <td>Type a name for the copied form.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Form Types </p> </td> 
      <td> <p>In the <b>Form Type</b> box, select the object types that you want the custom form to work with, and click the X next to any types that you want to remove. Types that are already associated with the form are disabled in the list.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>The form must be associated with at least one object type.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Copy Form**.

   In the original form, if calculated fields reference fields that are incompatible with an object type you add to the new form, a message prompts you to change the calculations in those fields.

   Similarly, if an access option for a section break on the original form isn't compatible with an object type you add to the new one, a message prompts you to adjust the option.

1. Select the form that you just copied, then click **Edit**.
1. Make any changes to the form, as explained in the following sections of the [Design a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) article:

* [Reuse an existing field or widget already used in another custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
    * [Add text fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
    * [Add calculated fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
    * [Add radio buttons, checkbox group, and dropdowns](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
    * [Add typeahead and date fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
    * [Add images, PDFs, and Videos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
    * [Add Adobe XD files](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Optional) After you click **Save+Close**, attach the form to the object where you want to use it, as described in [Add a custom form to an object](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).