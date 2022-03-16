---
filename: add-image-or-edit-its-properties-in-a-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Add or edit an image widget in a custom form
description: You can add an image widget to a custom form.
---

# Add or edit an image 

<!--
widget
-->

in a custom form

You can add an image 

<!--
widget
-->

to a custom form.

For example, next to a custom field where users need to type a serial number found on a piece of equipment, you could include a diagram or photo showing where to find the number on the equipment.

You can also edit the properties for an image 

<!--
widget
-->

that is already added to a custom form.

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

## Add an image 

<!--
widget
-->

or edit its properties in a custom form

1. Begin working on a custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. With the **Add a field** tab open, do one of the following:

  * If you are adding a new image widget, select **Embedded image** in the list of field types to add it to the form, or drag it where you want it on the form:

    ![](assets/embedded-image-350x228.jpg)

  * If you are editing an image  
  
    <!--  
    widget  
    -->  
  
    already added to the custom form, select the widget.

1. Type or edit any of the following properties for the image

   <!--
   widget
   -->

   :

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label for the widget. It displays above the widget when users view the field on a custom form added to an object.</p> <p>You can change the label at any time.</p> <p>Important: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Required) This name is how the system identifies the image widget when you add it to various areas throughout Workfront, such as reports, Home, and API interactions.</p> <p>When you are configuring the image widget for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p> <p>Important:  
        <ul> 
         <li> <p><span>Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in Workfront. If you do, the system will no longer recognize the image widget where it might now be referenced in other areas of Workfront.</span> </p> <p><span>For example, if you add the image widget to a report and later change the image widget's name, Workfront doesn't recognize the image widget in the report and the image widget will stop functioning correctly there unless you re-add it to the report using the new name.</span> </p> </li>  
        </ul> </p> <p>Each image widget name must be unique in your organization's Workfront instance. This way, you can reuse a image widget already created for another custom form. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td>(Required) Type or paste the URL of the image <!--
        widget
       -->where it is stored on the internet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Type any additional information about the image widget. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Size</td> 
      <td>Change the size of the image <!--
        widget
       -->as needed.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Done**.
1. (Optional) To position an image 

   <!--
   widget
   -->

   on the same row as another image 

   <!--
   widget
   -->

   or field, drag them next to each other until a line appears between them.

   When you drop the image 

   <!--
   widget
   -->

   where you want it, a gray outline box appears around the image 

   <!--
   widget
   -->

   and the other image 

   <!--
   widget
   -->

   or field, indicating that they share a row. If you drag an image 

   <!--
   widget
   -->

   until the blue line appears above or below another image 

   <!--
   widget
   -->

   or field, the two do not share a row.

   >[!NOTE]
   >
   >
   >  
   >  
   >  * You can use the `Preview` button in the lower-right corner to get an idea of how the image   >  
   >  
   >    <!--   >  
   >    widget   >  
   >    -->   >  
   >  
   >    s and fields will display in the form.
   >  
   >  * When a user is viewing the form, the amount of screen space they are using for the form can affect how image   >  
   >  
   >    <!--   >  
   >    widget   >  
   >    -->   >  
   >  
   >    s and fields display. For example, the third image   >  
   >  
   >    <!--   >  
   >    widgets   >  
   >    -->   >  
   >  
   >    in a row of image   >  
   >  
   >    <!--   >  
   >    widget   >  
   >    -->   >  
   >  
   >    s and fields may wrap to the next row if horizontal space is limited.
   >  
   >  
   >

1. If you want to add custom fields to your custom form, continue on to [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2).

   Or

   If you want to continue building your custom form in other ways, continue on to one of the following articles:

  * [Position fields and widgets in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md) 
  * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) 
  * [Using an existing calculated custom field on a new custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md) 
  * [Display logic and skip logic on a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md) 
  * [Preview and complete a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Reuse an existing image widget

1. Begin creating or editing a custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. With **Add a field** selected, click `Field Library`, then select the image 

   <!--
   widget
   -->

   in the list that appears.

   You cannot use an existing image 

   <!--
   widget
   -->

   more than once on a form.

   >[!IMPORTANT]
   >
   >When you modify an existing image   >
   >
   ><!--   >
   >widget   >
   >-->   >
   >
   >, any changes you make impact that field on all forms where it is used.

1. Click `Apply`.
1. (Optional) Repeat the two previous steps to add any other existing image

   <!--
   widget
   -->

   s.

   >[!NOTE]
   >
   >You can add up to 500 fields and image   >
   >
   ><!--   >
   >widget   >
   >-->   >
   >
   >s on a single custom form. However, performance degradation can occur when more than 100 exist on a form, depending on the complexity of the form. 
   >
   >
   >Examples of complex forms include forms with cascading parameters, calculated custom data fields, and multiple value options in a single field.

1. (Optional) Create and add any new image

   <!--
   widget
   -->

   s you need that have not yet been created for your organization, as explained in [Add or edit an image widget in a custom form](#create) in this article.

1. If you want to add a new custom field to the form, continue on to [Add or edit an image widget in a custom form](#create) in this article.

   Or

   If you want to continue building your custom form in other ways, continue on to one of the following articles:

  * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) 
  * [Using an existing calculated custom field on a new custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md) 
  * [Position fields and widgets in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md) 
  * [Display logic and skip logic on a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md) 
  * [Preview and complete a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

