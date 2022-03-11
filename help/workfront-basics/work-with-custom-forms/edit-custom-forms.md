---
filename: edit-custom-forms
product-area: projects;user-management
keywords: edit,forms,rich,text,special,format,fields,custom,information,customize,objects
navigation-topic: work-with-custom-forms
title: Edit information in custom form fields in Adobe Workfront
description: You can edit information on a custom form after the form is attached to an object. For information about adding custom forms to objects, see Add a custom form to an object.
---

# Edit information in custom form fields in `Adobe Workfront`

You can edit information on a custom form after the form is attached to an object. For information about adding custom forms to objects, see [Add a custom form to an object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span>Adobe Workfront</span> plan*</p> </td> 
   <td><span>Team</span> or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span>Adobe Workfront</span> licenses*</p> </td> 
   <td> <p><span>Request</span> or higher</p> </td> 
  </tr> Access level* Edit access to the object for which you want to edit the custom form Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see Create or modify custom access levels. Object permissions Contribute or higher permissions on the object for which you want to edit the custom form View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see Configure sharing for a custom field. Edit permissions for the sections on the form where the fields you want to edit are located For information on requesting additional access for objects, see Request access to objects in Adobe Workfront. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

Before you begin, you must

* Create a custom form. For instructions, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Attach a custom form to an object. For instructions, see [Add a custom form to an object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Edit information on a custom form

Editing information on a custom form attached to an object is identical for all objects. For information about what objects can have a custom form, see [Custom forms overview](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

<ol> 
 <li value="1">Go to an object for which you want to edit information on the custom form.</li> 
 <li value="2"> <p> Click <Object type> Details in the left panel. </p> <p> For example, when editing information on a project custom form, click Project Details. </p> </li> Scroll to the custom form. When there is a custom form attached to the object, the name of the form displays as an area in the Details section. If necessary, click the arrow to the left of the name of the custom form to expand it. 
 <li value="5"> <p> Near the upper-right corner of the page, click the Edit icon.</p> </li> 
 <li value="6"> <p>Start entering information in any field that you have access to edit.</p>  <p>Or</p> <p>If no information has been entered yet on the form, click <span class="bold">Add+</span> for any field you have access to edit and start entering information.</p>  <p>If multiple custom forms are attached to the object, you can do this for every form.</p> <p>Depending on the type of field you are editing consider the following: </p> 
  <ul> 
   <li>You can select only one option for radio-button fields.</li> 
   <li>You can select one or multiple options in a checkbox field, depending on how the form creator configured the field.</li> 
   <li>You can select one or multiple options in a multi-select drop-down field, depending on how the form creator configured the field.</li> 
   <li>You can format text fields (bold, italicize, or underline) only if the user who created the form set them up as a Text Field with Formatting field type. Single Line Text Fields and Paragraph Text Fields cannot be formatted.</li> 
   <li>You can update the time of the day in a Date field type only if the user who created the form has included it when creating the field.</li> 
  </ul> <p>For information about all of the field types, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Save </span>Changes.</p> <note type="important"> 
   <p>You must complete all required fields on the form before you can save the form.&nbsp;The name of a required field is followed by an asterisk. </p>  
  </note> When someone changes data in another object that is referenced by calculated custom fields in your object, the changes are not reflected automatically in your object. For information about manually updating all calculated custom fields in your object, see Recalculate all calculated custom fields for an object in this article. <p>You can also manually update all calculated custom fields for an object when you bulk-edit the object along with other objects in a list. For instructions, see <a href="#recalcul3" class="MCXref xref">Recalculate all calculated custom fields for multiple objects in a list</a> in this article.</p> </li> 
</ol>

Recalculate all calculated custom fields for an object Go to the main page of the object whose custom fields you want to recalculate. Click the More menu to the right of the object's name, then click Recalculate Expressions. This recalculates all custom fields on the object's form.

## Recalculate all calculated custom fields for multiple objects in a list

1. Go to a list of objects that contain custom forms with calculated fields.
1. Select the objects whose calculated custom fields you want to update.
1. Click the Edit icon.
1. Click `Custom Forms` in the left menu, then select `Recalculate Custom Expressions`. 
1. Click `Save` `Changes`.

