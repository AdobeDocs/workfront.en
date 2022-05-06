---
filename: add-a-custom-field-to-a-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Add a custom field to a custom form
description: When you are working on a custom form, you can create a new custom field and add it to a custom form.
---

# Add a custom field to a custom form

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

When you are working on a custom form, you can create a new custom field and add it to a custom form.

You can also add a custom field that was already added to another custom form. For instructions, see [Reuse a custom field or widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

>[!NOTE]
>
>In a custom form containing a lot of custom fields or a lot of multi-select options in custom fields, users might experience a slower performance when adding or changing values in those fields. For example, a form containing 100 custom fields, or multi-select custom fields with more than 200 options, might be slower when users interact with it.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Add a custom field to a custom form {#add-a-custom-field-to-a-custom-form}

1. Begin creating or editing a custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Open the **Add a field** tab.

   ![](assets/add-a-field-350x189.jpg)

1. With **New Field** ![](assets/new-field.jpg) selected, select one of the field types listed below:

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
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Text Field with Formatting</td> 
      <td> <p>Allows users to type multiple lines of text in the field and format the text with bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. This is available in Home, the Updates area, lists, and the Details area for Workfront objects. A character limit of 15,000 allows for plenty of text and formatting.</p> <p>For information about accessing this field through the API, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Rich text field storage in the API</a>.</p> <p>Note:    In lists throughout Workfront, you can't inline edit custom fields with rich text formatting. Text fields with formatting are not available for Workfront mobile apps (available in coming releases). </p> <p>Important:   <p>For the best performance in large lists where objects contain formatted text fields, limit the number of shown objects to 250 in the lower right corner of the window.</p> <p> <img src="assets/limit-list-objects-250-350x154.png" style="width: 350;height: 154;"> </img> </p> </p> </td> 
     </tr> 
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
      <td> <p>A section break is actually not a field. You can use a section break to organize your custom fields and widgets into sections and, if necessary, configure different viewing and editing permissions for each section. For information about adding and configuring section breaks, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Add a section break to a custom form</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. On the **Field Settings** tab, configure the options that are available for the type of custom field you are adding:

   <table cellspacing="0"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the custom field. You can change the label at any time.</p> <p>Important: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Required) This name is how the system identifies the custom field when you add it to various areas throughout Workfront, such as reports, Home, and API interactions.</p> <p>When you are configuring the custom field for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p> <p>Important:   
        <ul> 
         <li> <p><span>Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in Workfront. If you do, the system will no longer recognize the custom field where it might now be referenced in other areas of Workfront.</span> </p> <p>For example, if you add the custom field to a report and later change its name, Workfront doesn't recognize it in the report and it will stop functioning correctly there unless you re-add it to the report using the new name.</p> </li> 
         <li> <p>We recommend that you do not type a name that is already used for built-in Workfront fields.</p> </li> 
        </ul> </p> <p>Each custom field name must be unique in your organization's Workfront instance. This way, you can reuse one that was already created for another custom form. For more information, see <a href="#Add" class="MCXref xref">Add a custom field to a custom form</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Type any additional information about the custom field. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p> <p> <img src="assets/custom-field-tooltip-350x83.png" alt="custom_field_tooltip.png" style="width: 350;height: 83;"> </img> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Select the type of data that will be captured in the custom field.</p> <p>Note:   
        <ul> 
         <li>This field cannot be edited after the form is saved. If you intend to use your field in mathematical calculations, ensure that you select a Number or Currency format.<br></li> 
         <li>When you select Number or Currency, the system automatically truncates numbers that start with 0.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Display Type</td> 
      <td>(Dropdown, checkboxes, and radio buttons only) Switch the type of option selection you want for the field.</td> 
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
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Add Filter</td> 
      <td> <p>(Typeahead fields only) Add a filter for an object type to limit the objects users can choose when they are using the field. </p> <p>For example, you could limit a field so that user names can be selected only if they meet the following criteria:</p> 
       <ul> 
        <li>They belong to a group or groups that you specify</li> 
        <li>They are associated with a role or job title you specify</li> 
        <li>They belong to the same group as the person using the field</li> 
       </ul> <p>You must define the filter for the object type you selected using Text Mode syntax. For instructions on creating a filter, see <a href="#add-a-custom-field-to-a-custom-form" class="MCXref xref">Add a custom field to a custom form</a> in the article <a href="#" class="MCXref xref" xrefformat="{para}">Add a custom field to a custom form</a>. For information about creating a filter using Text Mode, see the section <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">Edit text mode in a filter</a> in the article <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Text Mode overview</a>. </p> <p>Note:   
        <ul> 
         <li>If you are editing an existing custom form, adding a filter to a Typeahead field does not remove any objects (outside the scope of the filter) that users have already added using the field.</li> 
         <li>This filter is not available on mobile devices. If you use the filter for a Typeahead field, the field will appear on users' mobile devices unaffected by the filter.</li> 
        </ul> </p> </td> 
     </tr> 
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
      <td role="rowheader">Track field changes in update feeds</td> 
      <td> <p>Note:   <p>This option is not available for the following:</p> 
        <ul> 
         <li>Custom forms associated with the following object types: Expense, Company, Iteration, Billing Record, and Group.</li> 
         <li>The following field types: Calculated , Descriptive Text , and Section Break</li> 
        </ul> </p> <p data-mc-conditions="QuicksilverOrClassic.Classic">Select this option if you want the Updates area for all objects where the form is attached to record value changes that users make in the field.</p> <p>For more information, see the section <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">Add fields you want Workfront to track</a> in the article <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">Configure system updates</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Specify which fields should appear on the form, based on selections users make in existing fields. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Choices </td> 
      <td> <p>(Dropdown, Checkboxes, or Radio Buttons only; optional)</p> 
       <ol> 
        <li value="1"> <p> <!--
           <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
             In Production, 
           </MadCap:conditionalText>
          -->Click <b>Options</b>, then select any of the following:</p> 
         <ul> 
          <li><strong>Sort Choices A-Z</strong>: Sorts the choices you add alphabetically in the field.</li> 
          <li><strong>Show Values</strong>: Shows the values of each choice in the field. The label of each choice shows by default.</li> 
         </ul> <!--
          <div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
           <p>Or, in Preview, enable any of the following:</p> 
           <ul> 
            <li><strong>Show Values</strong>: Shows the values of each choice in the field. The label of each choice shows by default.</li> 
            <li><strong>Sort Choices A-Z</strong>: Sorts the choices you add alphabetically in the field.</li> 
           </ul> 
          </div>
         --> </li> 
        <li value="2"> <p>For each choice you add for the user, click the gear icon <img src="assets/gear-icon-settings.png">, then select one of the following options:</p> 
         <ul> 
          <li><strong>Select by Default</strong>: Select the choice by default in the field.</li> 
          <li> <p><strong>Hide Choice</strong>: Hide the choice in the field. Hidden choices remain accessible in reports.</p> </li> 
          <li> <p><strong>Remove Choice</strong>: Remove the choice from the field.</p> <p>Warning:  If you have current objects using this choice, do not remove it from the field. Removing it will cause historic data to be lost. Instead, select the option to hide it, which prevents users from selecting it in the future.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditional) To change the display type of a field on the custom form, click the **Display Type** drop-down menu, then click the type you want.

   You can switch between the following field display types:

   * **Selection-type fields**: Checkboxes, Dropdown, Radio Buttons.
   * **Text-type fields**: Single Line Text Field, Paragraph Text Field. (You can’t switch a Text Field with Formatting to a different display type. However, you can remove it and add another type of field.)

   For example, if you have created a Checkboxes field, you can change it to a Dropdown field or a Radio Buttons field. Or, if you have created a Single Line Text Field, you can change it to a Paragraph Text field.

   >[!NOTE]
   >
   >Consider the following when you want to change a field's display type from a checkbox field or a multi-select dropdown field (a dropdown allowing more than one option to be selected) to a single-select field type:
   >
   >   
   >   
   >   * If you change to Radio Buttons, Workfront retains any multi-select values that a user may have entered in the field until the user changes and saves data in any part of the form. At this point, any values that were selected using the multi-select-type field are replaced by the selected Radio Button value.
   >   * If you change to a single-select Dropdown, Workfront retains any multi-select values that a user may have entered in the field until the user changes and saves the values in the field. At this point, any values that were selected using the multi-select-type field are replaced by the selected Dropdown value.
   >   
   >

1. (Optional) Repeat steps 2-6 to add other custom fields.

   Or

   Add fields that have already been created for your organization, as explained in [Reuse a custom field or widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >You can add up to 500 fields and widgets on a single custom form. However, performance degradation can occur when more than 100 exist on a form, depending on its complexity. 
   >
   >
   >Examples of complex forms include forms with cascading parameters, calculated custom data fields, and multiple value options in a single field.

1. Click **Apply**.
1. If you want to continue building your custom form in other ways, continue on to one of the following articles:

   * [Position custom fields and widgets in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md) 
   * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) 
   * [Add a section break to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md) 
   * [Reuse an existing calculated custom field in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md) 
   * [Add display logic and skip logic to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md) 
   * [Preview and complete a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

