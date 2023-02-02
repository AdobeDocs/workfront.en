---
title: Design a form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can design a custom form with the Form Designer.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
---

# Design a form

You can design a custom form with the Form Designer. You can attach custom forms to different Workfornt objects. 

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
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Start designing a custom form

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms** in the left panel.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Click **New Custom Form.**
1. Select which object types you'd like to attach the custom form to, then click **Continue**.

   ![](assets/choose-object-type.jpg)

1. In the **Title is required** area, type the custom form title.
1. (Optional) If you want to add more object types to the form so that it can be attached to more objects, click the **Add** icon ![](assets/add-objects-icon.png) after **Object Types**, then select the type you want in the menu that displays. You can repeat this to add as many object types as you want. 
   
   You can also click the X on an object type to delete it from the form. This should be done with caution when you want to delete an object type from a custom form you have already saved. For more information, see [Delete object types on a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Next, you can start adding fields to your custom form. See the following sections: 
    * Add text fields 
    * Add calculated fields
    * Add radio buttons and checkboxes
    * Add typeahead, drop-down, and date fields
    * Add images, PDFs, and Videos
    * Add Adobe XD files

## Add fields

You can add several different text fields to a custom form. 

+++ **See descriptions of available text fields**

* **Single Line Text Field**: Allows users to type a single line of text in the field.
* **Paragraph Text Field**: Allows users to type multiple lines of text in the field.
* **Text Field with Formatting**: Allows users to type multiple lines of text in the field and format the text with bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. This is available in Home, the Updates area, lists, and the Details area for Workfront objects. A character limit of 15,000 allows for plenty of text and formatting.

    For information about accessing this field through the API, see Rich text field storage in the API.

    >[!NOTE]
    >
    >Text fields with formatting are not available for Workfront mobile apps (available in coming releases).

+++

To add a text field: 

1. On the left side of the screen, find one of the following fields and drag it to a section on the canvas.
    ![](assets/drag-field-to-section.png)

1. On the right side of the screen, configure the options that are available for the type of custom field you are adding:

   <table>
    <tr>
    <td>Input into</td>
    <td>Description</td>
    <td>Available for </td>
    </tr>
    <tr>
    <td>Label</td>
    <td><p>Type a descriptive label to display above the widget. You can change the label at any time.<p>
    <p>IMPORTANT: Avoid using special characters in this label. They don't display correctly in reports.</p></td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    <li>Text with formatting</li>
    </ul></td>
    </tr>
    <tr>
     <td>Name</td>
    <td>(Required) This name is how the system identifies the widget. When you are configuring the widget for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    <li>Text with formatting</li>
    <li>Descriptive text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instructions</td>
    <td>Type any additional information about the widget. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    <li>Text with formatting</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td>Choose formatting for the text box</td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Display Type</td>
    <td>Switch between single line and paragraph text</td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    <li>Text with formatting</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hyperlink</td>
    <td>Add a hyperlink for the text</td>
    <td><ul><li>Descriptive text</li></ul></td>
    </tr>
</table>


 ### Add text fields

 ### Add calculated fields

 ### Add radio buttons and checkboxes

 ### Add typeahead, drop-down, and date fields

 ### Add images, PDFs, and Videos

 ### Add Adobe XD files


 ## Organize your form