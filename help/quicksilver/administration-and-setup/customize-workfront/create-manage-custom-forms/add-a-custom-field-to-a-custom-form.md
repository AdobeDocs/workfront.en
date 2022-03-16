---
filename: add-a-custom-field-to-a-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Add a custom field to a custom form
description: The highlighted information on this page refers to functionality available only in the new Workfront experience beta.
---

# Add a custom field to a custom form

The highlighted information on this page refers to functionality available only in the new Workfront experience beta.

When you are working on a custom form, you can create a new custom field and add it to a custom form.

You can also add a custom form that is already created in your system. For instructions, see [Reuse an existing custom field](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
For information about adding an image to a custom form, which is a process similar to adding a custom field, see Add or edit an image widget in a custom form. 

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

## Add a custom field to a custom form

1. Begin creating or editing a custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Open the **Add a field** tab.

   ![](assets/add-a-field-350x175.jpg)

1. With `New Field` selected, select one of the field types listed below:

   <table cellspacing="0"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Single Line Text Field</td> 
      <td>Allows users to type a single line of text in the field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Paragraph Text Field</td> 
      <td>Allows users to type multiple lines of text in the field.</td> 
     </tr> Text Field with Formatting Allows users to type multiple lines of text in the field and format the text with bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. This is available in Home, the Updates area, lists, and the Details area for Workfront objects. A character limit of 15,000 allows for plenty of text and formatting. For information about accessing this field through the API, see Rich text field storage in the API. Note: Text fields with formatting are not available for Workfront mobile apps (available in coming releases). 
     <tr> 
      <td role="rowheader">Dropdown</td> 
      <td>Provides a list of drop-down choices.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typeahead </td> 
      <td> <p>Allows users to type the name of an object that exists in Workfront. A list of suggestions appears when the user starts typing. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calculated</td> 
      <td>Allows you to define an expression and display the result on the custom form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date</td> 
      <td>Displays a calendar where users can select a date and time.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Checkboxes</td> 
      <td>Allows users to select multiple choices.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Radio Buttons</td> 
      <td>Requires users to select only one choice.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descriptive Text</td> 
      <td>Allows you to include instructions and link to pages outside Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Section Break</td> 
      <td> <p>You can use a section break to organize your fieldsand image widgets into sections and, if necessary, configure different viewing and editing permissions for each section. For information about adding and configuring section breaks, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Add a section break to a custom form</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. On the `Field Settings` tab, configure the options that are available for the type of field you are adding:

   <table cellspacing="0"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label for the custom field. It displays above the custom field when users view the field on a custom form added to an object.</p> <p>You can change the label at any time.</p> <p>Important: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Required) This name is how the system identifies the custom field when you add it to various areas throughout Workfront, such as reports, Home, and API interactions.</p> <p>When you are configuring the custom field for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p> <p>Important:   
        <ul> 
         <li> <p><span>Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in Workfront. If you do, the system will no longer recognize the custom field where it might now be referenced in other areas of Workfront.</span> </p> <p><span>For example, if you add the custom field to a report and later change the custom field's name, Workfront doesn't recognize the custom field in the report and the custom field will stop functioning correctly there unless you re-add it to the report using the new name.</span> </p> </li>  
        </ul> </p> <p>Each custom field name must be unique in your organization's Workfront instance. This way, you can reuse a custom field already created for another custom form. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Type any additional information about the custom field. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p> <p> <img src="assets/custom-field-tooltip-350x83.png" alt="custom_field_tooltip.png" style="width: 350;height: 83;"> </img> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Select the type of data that will be captured in the field</p> <p>Note:   
        <ul> 
         <li>This field cannot be edited after the form is saved. If you intend to use your field in mathematical calculations, ensure that you select a Number or Currency format.<br></li> 
         <li>When you select Number or Currency, the system automatically truncates numbers that start with 0.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Size</td> 
      <td>(Text fields only) Select a width for the field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Display Time of Day</td> 
      <td>(Date fields only) Select this option if you want to show the time of day along with the date in the field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Referenced Object Type</td> 
      <td> <p>(Typeahead fields only) Select the object type that you want to associate with the field.</p> <p>Once you have clicked Apply or Save+Close, you cannot change the object type for the field.</p> <p>Note:   
        <ul> 
         <li>If your Workfront administrator customized the name for Portfolios, Programs, or Projects in the Workfront user interface, the default Workfront name for the object appears in this drop-down list, not the customized name. See your Workfront administrator if you need help with this.<br></li> 
         <li>The following object types are supported in the iOS and Android Workfront Mobile Apps: User, Company, Group, Job Role, Portfolio, Program, Project, and Template.</li> 
        </ul> </p> </td> 
     </tr> Add Filter (Typeahead fields only) Add a filter for an object type to limit the objects users can choose when they are using the field. For example, you could limit a field so that user names can be selected only if they meet the following criteria: They belong to a group or groups that you specify They are associated with a role or job title you specify They belong to the same group as the person using the field You must define the filter for the object type you selected using Text Mode syntax. For instructions on creating a filter, see Add a custom field to a custom form in the article Add a custom field to a custom form. For information about creating a filter using Text Mode, see the section Edit text mode in a filter in the article Text Mode overview. Note: If you are editing an existing custom form, adding a filter to a Typeahead field does not remove any objects (outside the scope of the filter) that users have already added using the field. This filter is not available on mobile devices. If you use the filter for a Typeahead field, the field will appear on users' mobile devices unaffected by the filter. 
     <tr> 
      <td role="rowheader">Descriptive Text</td> 
      <td>(Descriptive Text fields only) Type the text that you want to display to provide instructions or a link on the custom form. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hyperlink</td> 
      <td>(Descriptive Text fields only) If you want to apply a hyperlink to the Descriptive Text you have typed, add it here.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Make a required field</td> 
      <td>Select this option if you want the field to be required in order for the user to complete the custom form. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Display field changes in update feeds</td> 
      <td> <p>Select this option if you want the Updates area for objects where this custom form is attached to record changes that users make to information (values) in the field.</p> <p>Note:   <p>This option is not available for the following:</p> 
        <ul> 
         <li>Custom forms associated with the following object types: Expense, Company, Iteration, Billing Record, and Group.</li> 
         <li>The following field types: Calculated , Descriptive Text , and Section Break</li> 
        </ul> </p> <!--
        If this option is already enabled for at least one object type, and the custom form you're working on is associated with multiple object types, you can indicate other object types where you want to automatically track the field's value changes. SCREENSHOT Selecting or deselecting an object type here affects all custom forms that are associated with the selected object type and that contain this field. For example, if you deselect an object type here and save the custom form, the field's value changes are no longer tracked for that object type in both of the following places: The custom form you're working on All other custom forms that are associated with the deselected object type and that contain this field Note: After you select an object type here and save the custom form, the field that you're working on displays on the Custom Fields tab in the Update Feeds area in Setup. Conversely, if this field is deleted on that page, the object type is deselected for this setting on all custom forms that are associated with the object type and that contain this field. For more information, see the section Add fields you want Workfront to track in the article Configure system updates.
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Specify which fields should appear on the form, based on selections users make in existing fields. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Display logic and skip logic on a custom form</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Options</td> 
      <td> <p>(Dropdown, Checkboxes, or Radio Buttons only; optional) Select any option to do the following:</p> 
       <ul> 
        <li><span class="bold">Sort Choices A-Z</span>: Sort the choices you add alphabetically in the field.</li> 
        <li>Click <span class="bold">Show Values</span>: Show the values of each choice in the field. The label of each choice shows by default.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Choices <img src="assets/gear-icon-blue.png"></td> 
      <td>(Dropdown, Checkboxes, or Radio Buttons only; optional) For each choice you add for the user, select one of the following options: 
       <ul> 
        <li><span class="bold">Select by Default</span>: Select the choice by default in the field.</li> 
        <li><p><span class="bold">Hide Choice</span>: Hide the choice in the field.</p><p> Hidden choices remain accessible in reports.</p></li> 
        <li><p><span class="bold">Remove Choice</span>: Remove the choice from the field.</p><p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span> If you have current objects using this choice, do not remove it from the field. Removing it will cause historic data to be lost. Instead, select the option to hide it, which prevents users from selecting it in the future.</p></li> 
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditional) To change the display type of a field on the custom form, click the `Display Type` drop-down menu, then click the type you want.

   You can switch between the following field display types:

  * `Selection-type fields`: Checkboxes, Dropdown, Radio Buttons.
  * `Text-type fields`: Single Line Text Field, Paragraph Text Field. (You can’t switch a Text Field with Formatting to a different display type. However, you can remove it and add another type of field.)

   For example, if you have created a Checkboxes field, you can change it to a Dropdown field or a Radio Buttons field. Or, if you have created a Single Line Text Field, you can change it to a Paragraph Text field.

   >[!NOTE]
   >
   >Consider the following when you want to change a field's display type from a checkbox field or a multi-select dropdown field (a dropdown allowing more than one option to be selected) to a single-select field type:
   >
   >  
   >  
   >  * If you change to Radio Buttons, Workfront retains any multi-select values that a user may have entered in the field until the user changes and saves data in any part of the form. At this point, any values that were selected using the multi-select-type field are replaced by the selected Radio Button value.
   >  * If you change to a single-select Dropdown, Workfront retains any multi-select values that a user may have entered in the field until the user changes and saves the values in the field. At this point, any values that were selected using the multi-select-type field are replaced by the selected Dropdown value.
   >  
   >

1. (Optional) Repeat steps 2-6 to add other custom fields.

   Or

   Add fields that have already been created for your organization, as explained in [Add a custom field to a custom form](#add).

   >[!NOTE]
   >
   >You can add up to 500 fields on a single custom form. However, performance degradation can occur when more than 100 fields exist on a form, depending on the complexity of the form. Examples of complex forms include forms with cascading parameters, calculated custom data fields, and multiple value options in a single field.

1. If you want to continue building your custom form in other ways, continue on to one of the following articles:

  * [Position fields and widgets in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md) 
  * [Add a section break to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md) 
  * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) 
  * [Using an existing calculated custom field on a new custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md) 
  * [Display logic and skip logic on a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md) 
  * [Preview and complete a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

