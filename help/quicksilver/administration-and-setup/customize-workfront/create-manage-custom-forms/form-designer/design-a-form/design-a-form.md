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

## Add fields to your custom form

 ### Add text fields

 You can add several different text fields to a custom form. 

+++ **See descriptions of available text fields**

* **Single Line Text Field**: Allows users to type a single line of text in the field.
* **Paragraph Text Field**: Allows users to type multiple lines of text in the field.
* **Text Field with Formatting**: Allows users to type multiple lines of text in the field and format the text with bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. This is available in Home, the Updates area, lists, and the Details area for Workfront objects. A character limit of 15,000 allows for plenty of text and formatting.

    For information about accessing this field through the API, see Rich text field storage in the API.

    >[!NOTE]
    >
    >Text fields with formatting are not available for Workfront mobile apps (available in coming releases).
* **Descriptive text**: Allows you to include instructions and link to pages outside Workfront.

+++

To add a text field: 

1. On the left side of the screen, find one of the following text fields and drag it to a section on the canvas:

    * Single Line Text:
    * Paragraph Text
    * Text field with formatting
    * Descriptive texts

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
    <td><p>(Required) This name is how the system identifies the widget. When you are configuring the widget for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p>
    <p><b>IMPORTANT</b>:   
      <ul> 
      <li>Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in Workfront. If you do, the system will no longer recognize the custom field where it might now be referenced in other areas of Workfront. <p>For example, if you add the custom field to a report and later change its name, Workfront doesn't recognize it in the report and it will stop functioning correctly there unless you re-add it to the report using the new name.</p> </li>
      <li> <p>We recommend that you do not type a name that is already used for built-in Workfront fields.</p> </li>
      <li><p>We recommend that you do not use the period/dot character in the custom field name, to prevent errors when using the field in different areas of Workfront.</p></li>
    </td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    <li>Text with formatting</li>
    <li>Descriptive text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instructions</td>
    <td>Type any additional information about the widget. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    <li>Text with formatting</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td><p>Select the type of data that will be captured in the custom field.</p> <p><b>NOTE</b>:   
    <ul> 
    <li>This field cannot be edited after the form is saved. If you intend to use your field in mathematical calculations, ensure that you select a Number or Currency format.<br></li> 
    <li>When you select Number or Currency, the system automatically truncates numbers that start with 0.</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Display Type</td>
    <td>Switch the type of option selection you want for the field.</td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    <li>Text with formatting</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hyperlink</td>
    <td> If you want to apply a hyperlink to the Descriptive Text you have typed, add it here.</td>
    <td><ul><li>Descriptive text</li></ul></td>
    </tr>
</table>

 ### Add calculated fields

 ### Add radio buttons and checkboxes

 You can add radio buttons and checkboxes to a custom form. 

+++ **See descriptions of available fields**

* **Radio buttons**: Requires users to select only one choice.
* **Checkbox Group**: Allows users to select multiple choices.

+++

To add radio buttons and checkboxes:

1. On the left side of the screen, find one of the following fields and drag it to a section on the canvas.

    * Radio buttons
    * Checkbox Group

    ![](assets/drag-field-to-section.png)

1. On the right side of the screen, configure the options that are available for the type of custom field you are adding:

    <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Input into</td>
    <td>Description</td>
    <td>Available for </td>
    </tr>
    <tr> 
     <td role="rowheader">Label</td> 
     <td> <p>(Required) Type a descriptive label to display above the custom field. You can change the label at any time.</p> <p><b>IMPORTANT</b>: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     <td><ul>
    <li>Radio buttons</li>
    <li>Checkbox Group</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Name</td> 
     <td> <p>(Required) This name is how the system identifies the custom field when you add it to various areas throughout Workfront, such as reports, Home, and API interactions.</p> <p>When you are configuring the custom field for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p> 
    <p><b>IMPORTANT</b>:   
     <ul> 
    <li>Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in Workfront. If you do, the system will no longer recognize the custom field where it might now be referenced in other areas of Workfront. <p>For example, if you add the custom field to a report and later change its name, Workfront doesn't recognize it in the report and it will stop functioning correctly there unless you re-add it to the report using the new name.</p> </li>
    <li> <p>We recommend that you do not type a name that is already used for built-in Workfront fields.</p> </li>
     <li><p>We recommend that you do not use the period/dot character in the custom field name, to prevent errors when using the field in different areas of Workfront.</p></li>
     </ul> <p>Each custom field name must be unique in your organization's Workfront instance. This way, you can reuse one that was already created for another custom form. For more information, see <a href="#Add" class="MCXref xref">Add a custom field to a custom form</a> in this article.</p> </td>
     <td><ul>
    <li>Radio buttons</li>
    <li>Checkbox Group</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Instructions</td> 
    <td> <p>Type any additional information about the custom field. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Radio buttons</li>
    <li>Checkbox Group</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Format</td> 
    <td> <p>Select the type of data that will be captured in the custom field.</p> <p><b>NOTE</b>:   
     <ul> 
    <li>This field cannot be edited after the form is saved. If you intend to use your field in mathematical calculations, ensure that you select a Number or Currency format.<br></li> 
    <li>When you select Number or Currency, the system automatically truncates numbers that start with 0.</li> 
     </ul></p></td> 
     <td><ul>
    <li>Radio buttons</li>
    <li>Checkbox Group</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Display Type</td> 
    <td>(Dropdown, checkboxes, and radio buttons only) Switch the type of option selection you want for the field.</td> 
    <td><ul>
    <li>Radio buttons</li>
    <li>Checkbox Group</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Make a required field</td> 
    <td>Select this option if you want the field to be required in order for the user to complete the custom form. </td> 
    <td><ul>
    <li>Radio buttons</li>
    <li>Checkbox Group</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Choices </td> 
    <td> 
    <ol> 
    <li> <p>Click <b>Options</b>, then enable any of the following:</p> 
    <ul> 
    <li><strong>Show Values</strong>: Shows the values of each choice in the field. The label of each choice shows by default.</li> 
     <li><strong>Sort Choices A-Z</strong>: Sorts the choices you add alphabetically in the field.</li> 
    </ul> 
    </li> 
    <li> <p>For each choice you add for the user, click the gear icon <img src="assets/gear-icon-settings.png">, then select one of the following options:</p> 
    <ul> 
    <li><strong>Select by Default</strong>: Select the choice by default in the field.</li> 
    <li> <p><strong>Hide Choice</strong>: Hide the choice in the field. Hidden choices remain accessible in reports.</p> </li> 
    <li> <p><strong>Remove Choice</strong>: Remove the choice from the field.</p> <p><b>WARNING</b>:  If you have current objects using this choice, do not remove it from the field. Removing it will cause historic data to be lost. Instead, select the option to hide it, which prevents users from selecting it in the future.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Radio buttons</li>
    <li>Checkbox Group</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

 ### Add typeahead, drop-down, and date fields

 You can add typeahead, drop-down, and date fields to a custom form. 

+++ **See descriptions of available fields**

* **Typeahead**: Allows users to type the name of an object that exists in Workfront. A list of suggestions appears when the user starts typing. This field type supports the following objects:
    * User
    * Group
    * Job Role
    * Portfolio
    * Program
    * Project
    * Team
    * Template
    * Company
* **Dropdown**: Provides a list of drop-down choices.
* **Date Field**: Displays a calendar where users can select a date and time.

+++

To add radio buttons and checkboxes:

1. On the left side of the screen, find one of the following fields and drag it to a section on the canvas.

    * Typeahead
    * Dropdown
    * Date Field

    ![](assets/drag-field-to-section.png)

1. On the right side of the screen, configure the options that are available for the type of custom field you are adding:

 ### Add images, PDFs, and Videos

 ### Add Adobe XD files

 You can add an Adobe XD prototype directly to a custom form. 

 To add an Adobe XD file:

1. On the left side of the screen, find **Adobe XD** and drag it to a section on the canvas. 
1. Type or edit any of the following properties for the widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the widget. You can change the label at any time.</p> <p><b>IMPORTANT</b>: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Required) This name is how the system identifies the widget. When you are configuring the widget for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p>
    <p><b>IMPORTANT</b>:   
      <ul> 
      <li>Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in Workfront. If you do, the system will no longer recognize the custom field where it might now be referenced in other areas of Workfront. <p>For example, if you add the custom field to a report and later change its name, Workfront doesn't recognize it in the report and it will stop functioning correctly there unless you re-add it to the report using the new name.</p> </li>
      <li> <p>We recommend that you do not type a name that is already used for built-in Workfront fields.</p> </li>
      <li><p>We recommend that you do not use the period/dot character in the custom field name, to prevent errors when using the field in different areas of Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Required) Type or paste a valid XD prototype link.</p> 
      <p>Note: The Link Access setting on the Share tab in Adobe XD must be set to Anyone with the link. Otherwise, users will not be able to view the prototype. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Type any additional information about the widget. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Size</td> 
      <td>(Optional) Change the display size of the widget as needed.</td> 
     </tr> 
    </tbody> 
   </table>

 ## Organize your custom form