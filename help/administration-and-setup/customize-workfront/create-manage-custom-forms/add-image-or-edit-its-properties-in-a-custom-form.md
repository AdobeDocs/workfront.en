---
filename: add-image-or-edit-its-properties-in-a-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Add an image or edit its properties in a custom form
description: You can add an image widget that displays in a custom form.
---

# Add an image or edit its properties in a custom form

You can add an image widget that displays in a custom form.

For example, could you An image could be helpful, for example, next to a custom field where users need to type a serial number found on a piece of equipment—you could include a diagram or photo showing where to find the number on the equipment.

You add an image to a custom form by specifying the URL of the image where it is stored on the internet.

You can also edit the properties for an image widget that is already added to a custom form.

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

## Add an image or edit its properties in a custom form

<ol> 
 <li value="1">Begin working on a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li> 
 <li value="2"> <p>Select <b>Widget Library</b>.</p> <!--
   SCREENSHOT SHOWING WHERE THIS IS
  --> </li> 
 <li value="3"> <p>If you are adding an image, click <b>Embedded image</b> in the <b>Widget Library</b> list.</p> <p>Or</p> <p>If you are editing the properties for an image already added to the custom form, select the image.</p> </li> 
 <li value="4"> <p>Type or edit any of the following properties for the image widget:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Label</td> 
     <td> <p>(Required) Type a descriptive label for the widget. It displays above the widget when users view the field on a custom form added to an object.</p> <p>You can change the label at any time.</p> <note type="important">
       Avoid using special characters in this label. They don't display correctly in reports.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td> <p>(Required) This name is how the system identifies the widget when you add it to various areas throughout Workfront, such as reports, Home, and API interactions.</p> <p>When you are configuring the widget for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p> <note type="important">  
       <ul> 
        <li> <p><span>Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in Workfront. If you do, the system will no longer recognize the widget where it might now be referenced in other areas of Workfront.</span> </p> <p><span>For example, if you add the widget to a report and later change the widget's name, Workfront doesn't recognize the widget in the report and widget will stop functioning correctly there unless you re-add it to the report using the new name.</span> </p> </li>  
       </ul> 
      </note> <p>Each widget name must be unique in your organization's Workfront instance. This way, you can reuse a widget already created for another custom form. For more information, see <a href="#add" class="MCXref xref" data-mc-variable-override="">Add an image or edit its properties in a custom form</a> in this article.<!--
        [may need to say "existing field or widget" throughout that section; asked gevorg and he says they're still figuring this out]
       --></p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Instructions</td> 
     <td> <p>Type any additional information about the widget. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Image URL</td> 
     <td>(Required) Type or paste the URL of the image where it is stored on the internet.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Size</td> 
     <td>Change the size of the image as needed.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">Click <b>Done</b>.</li> 
 <li value="6"> <p> If you want to add custom fields to your custom form, continue on to <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a>.</p> <p>Or</p> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p> 
  <ul> 
   <li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position fields in a custom form</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md" class="MCXref xref">Using an existing calculated custom field on a new custom form</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Display logic and skip logic on a custom form</a> </li> 
   <li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li> 
  </ul> </li> 
</ol>

