



# Create a Custom Form {#create-a-custom-form}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


Custom Forms enable you to include your organization's unique information in `Workfront`. You can categorize work based on custom attributes and include all of the data needed for tracking.


You can create a new Custom Form or copy a Custom Form to create a new one that is based on the original.


To create a Custom Form, you must have at least a Plan license with administrative access to Custom Forms in your group. For more information about allowing users administrative access, see [Assign users administrative access](assign-users-administrative-access.md).


## Start creating a Custom Form {#start-creating-a-custom-form}




1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png)..

1.  Click **Custom Forms** in the left panel.  



   In the view that appears, you can review all Custom Forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it.  



   ![custom_forms_main_ui.png](assets/custom-forms-main-ui-600x294.png)



1.  Click **New Custom Form**, then click the object type in the drop-down list that you want to associate with the Custom Form. 


   The object type that you select is the only type that you can associate with the form.

1. On the **Form Settings** tab that opens, type a **Form Title** and (optional) a **Description** for the Custom Form.  

1.  Click **Done**.


   >[!TIP] {type="tip"}
   >
   >You can click **Apply** at any point during creating a Custom Form to save your changes and keep the form open.



1. Continue on to [Add a field to a Custom Form](#add2).




## Add a field to a Custom Form {#add-a-field-to-a-custom-form}

You can add a field that has already been created for your organization. You can also create a new field and add it to a Custom Form.


>[!NOTE]
>
>You can add up to 500 fields on a single Custom Form. However, performance degradation can occur when more than 100 fields exist on a form, depending on the complexity of the form. Examples of complex forms include forms with cascading parameters, calculated custom data fields, and multiple value options in a single field. 





* [Reuse an existing field](#add) 
* [Create and add a new field](#create) 




### Reuse an existing field {#reuse-an-existing-field}




1. Begin creating a Custom Form, as described in [Start creating a Custom Form](#start) in this article.
1.  Click **Field Library**, then select the field in the list that appears below.


   You cannot use an existing form field more than once on a form.


   >[!IMPORTANT] {type="important"}
   >
   >When you modify an existing field,&nbsp;any changes you make impact that field on all forms where it is used.



1. Click **Apply**.
1. (Optional) Repeat the two previous steps to add any other existing fields.
1. (Optional) Create and add any new fields you need that have not yet been created for your organization, as explained in [Create and add a new field](#create) in this article.
1.  (Optional) To position fields on the same row, drag them next to each other until a line appears between them.


   When you drop the field where you want it, a gray outline box appears around the two fields, indicating that they share a row. If you drag a field until the blue line appears above or below another field, the fields do not share a row.


   >[!NOTE]
   >
   >
   >    
   >    
   >    * You can use the **Preview** button in the lower-right corner to to get an idea of how the fields will display in the form.
   >    * Fields may not display exactly the same way in the form; depending on how much screen space is available when a user is viewing the form. For example, the third field in a row of fields may wrap to the next row of fields if horizontal space is limited.
   >    
   >    




1. If you want to create a new field for your Custom Form, continue on to [Create and add a new field](#create).




### Create and add a new field {#create-and-add-a-new-field}




1. Begin creating a Custom Form, as described in [Start creating a Custom Form](#start) in this article.
1.  Click **New Field**, then select one of the field types listed below:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Single Line Text Field</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Allows users to type a single line of text in the field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Paragraph Text Field</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Allows users to type multiple lines of text in the field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><span class="preview">Text Field with Formatting</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p class="preview">Allows users to type multiple lines of text in the field and format the text with bold, italics, and underline. They can do this in Home, lists, and the Details area for <span class="WFVariablesProdNameWF">Workfront</span> objects. A character limit of 15,000 allows for plenty of text and formatting.</p> <p class="preview">For information about accessing this field through the API, see <a href="#rich" class="MCXref xref">Rich text field storage in the API</a> in this article.</p> <p>Note:  <p class="preview">Text fields with formatting are not available for the following:</p> 
     <ul> 
      <li class="preview" value="1"><span class="WFVariablesProdNameWF">Workfront</span> mobile apps (available in coming releases)</li> 
      <li value="2"> <p class="preview">Lists in <span class="WFVariablesWorkfrontClassic">Workfront Classic</span>. </p> <p class="preview">Formatting is visible in Project, Task, and Hour lists in <span class="WFVariablesWorkfrontClassic">Workfront Classic</span>, but we don’t support its use there; it should be used in lists only the new Workfront experience.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Dropdown</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Provides a list of drop-down choices.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Typeahead </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Allows users to type the name of an object that exists in <span class="WFVariablesProdNameWF">Workfront</span>. A list of suggestions appears when the user starts typing. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Calculated</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Allows you to define an expression and display the result on the Custom Form. For more information, see <a href="add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a Custom Form</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Date</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Displays a calendar where users can select a date and time.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Checkboxes</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Allows users to select multiple choices.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Radio Buttons</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Requires users to select only one choice.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Descriptive Text</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Allows you to include instructions and link to pages outside <span class="WFVariablesProdNameWF">Workfront</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Section Break</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Allows you to break up the information on the form in separate sections. You can nest additional custom fields under one section.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  On the **Field Settings** tab, change any of the following options available for the type of field you are adding:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 260px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Label</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>(Required) Type a descriptive Label for the custom field. The Label is what displays above the field when users view the field on a custom form attached to an object.</p> <p>You can change a field's Label at any time.</p> <p>Important:  Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><span class="preview">Name</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p class="preview">(Required) This name is how the system identifies the field when you add it to various areas throughout Workfront, such as reports, Home, Storyboard customizations, and API interactions.</p> <p class="preview">When you are configuring the field for the first time and you type the Label, the Name populates automatically to match it. But the Label and Name are not synchronized—this gives you the freedom to change the Label that your users see without changing the Name that the system sees.</p> <p>Important:  <p class="preview"><span class="preview">Though it's possible to do so, we recommend that you do not change a field's Name after you or other users start using the field in <span class="WFVariablesProdNameWF">Workfront</span>. If you do, the system will no longer recognize the field where it is being used.</span> </p> <p class="preview"><span class="preview">For example, if you add the field to a report and later change the field's Name, <span class="WFVariablesProdNameWF">Workfront</span> won't recognize the field in the report and it will stop functioning correctly there unless you re-add the field to the report using the new Name.</span> </p> </p> <p class="preview">Each field name must be unique in your organization's Field Library. You can reuse a field already created for another Custom Form by choosing it from this library. For more information, see <a href="#add" class="MCXref xref">Reuse an existing field</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Instructions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Type any additional information about the field. The information displays in a tool tip next to the field on the Custom Form:</p> <p> <img src="assets/custom-field-tooltip-564x134.png" alt="custom_field_tooltip.png" style="width: 564;height: 134;"> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Format</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the type of data that will be captured in the field</p> <p>Note:  
     <ul> 
      <li value="1">This field cannot be edited after the form is saved. If you intend to use your field in mathematical calculations, ensure that you select a Number or Currency format.<br></li> 
      <li value="2">When you select Number or Currency, the system automatically truncates numbers that start with 0.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Size</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">(Text fields only) Select a width for the field. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Display Time of Day</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">(Date fields only) Select this option if you want to show the time of day along with the date in the field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Referenced Object Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>(Typeahead fields only) Select the object type that you want to associate with the field.</p> <p>Once you have clicked Apply or Save+Close, you cannot change the object type for the field.</p> <p>Note:  
     <ul> 
      <li value="1">If your <span class="WFVariablesAdminWF">Workfront administrator</span> has customized the name for Portfolios, Programs, or Projects in the <span class="WFVariablesProdNameWF">Workfront</span> user interface, the default <span class="WFVariablesProdNameWF">Workfront</span> name for the object appears in this drop-down list, not the customized name. See your <span class="WFVariablesAdminWF">Workfront administrator</span> if you need help with this.<br></li> 
      <li value="2">Currently, User is the only object type fully supported in the Workfront Mobile App. The following object types&nbsp;Company, Group, Job Role, Portfolio, Program, Project, and Template are not yet supported. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Add Filter</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Typeahead fields only) Add a filter for an object type to limit the objects users can choose when they are using the field. </p> <p>For example, you could limit a field so that user names can be selected only if they meet the following criteria:</p> 
    <ul> 
     <li value="1">They belong to a group or groups that you specify</li> 
     <li value="2">They are associated with a role or job title you specify</li> 
     <li value="3">They belong to the same group as the person using the field</li> 
    </ul> <p>You must define the filter for the object type you selected using Text Mode syntax. For information about how to create a filter, see <a href="#create" class="MCXref xref">Create and add a new field</a> in the article <a href="#" class="MCXref xref" xrefformat="{para}">Create a Custom Form</a>. For information about creating a filter using Text Mode, see the section <a href="understand-text-mode.md#editing2" class="MCXref xref">Edit text mode in a filter</a> in the article <a href="understand-text-mode.md" class="MCXref xref">Understand Text Mode</a>. </p> <p>Note:  
     <ul> 
      <li value="1">If you are editing an existing Custom Form, adding a filter to a Typeahead field does not remove any objects (outside the scope of the filter) that users have already added using the field.</li> 
      <li value="2">This filter is not available on mobile devices. If you use the filter for a Typeahead field, the field will appear on users' mobile devices unaffected by the filter.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Descriptive Text</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">(Descriptive Text fields only) Type the text that you want to display to provide instructions or a link on the Custom Form. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Hyperlink</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">(Descriptive Text fields only) If you want to apply a hyperlink to the Descriptive Text you have typed, add it here.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Make a required field</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select this option if you want the field to be required in order for the user to complete the Custom Form. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Display field changes in update feeds</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select this option if you want the Updates area for objects with this field to record changes that users make to the field values. (This option is not available for Calculated fields or Descriptive Text fields.)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Add Logic</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify which fields should appear on the form, based on selections users make in existing fields. For more information, see&nbsp;<a href="display-or-skip-logic-custom-form.md" class="MCXref xref">Display or skip logic on a Custom Form</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Options</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Dropdown, Checkboxes, or Radio Buttons only; optional) Select any option to do the following:</p> 
    <ul> 
     <li value="1"><b>Sort Choices A-Z</b>: Sort the choices you add alphabetically in the field.</li> 
     <li value="2">Click <b>Show Values</b>: Show the values of each choice in the field. The label of each choice shows by default.</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Choices <img src="assets/gear-icon.png"> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">(Dropdown, Checkboxes, or Radio Buttons only; optional) For each choice you add for the user, select one of the following options:
    <ul>
     <li value="1"><b>Select by Default</b>: Select the choice by default in the field.</li>
     <li value="2"><p><b>Hide Choice</b>: Hide the choice in the field.</p><p> Hidden choices remain accessible in reports.</p></li>
     <li value="3"><p><b>Remove Choice</b>: Remove the choice from the field.</p><p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span> If you have current objects using this choice, do not remove it from the field. Removing it will cause historic data to be lost. Instead, select the option to hide it, which prevents users from selecting it in the future.</p></li>
    </ul></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">In order to VIEW this section, people must have permission to</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> (Section Break only) Select the permissions users need on the object associated with the form in order to view this section:</p> 
    <ul> 
     <li value="1"><b>View</b>: The user needs View permissions to the object to be able to view this section.</li> 
     <li value="2"><b>Manage</b>: The user needs Manage permissions to the object to be able to view this section.</li> 
     <li value="3"><b>Admin only</b>: Only the <span class="WFVariablesAdminWF">Workfront administrator</span> can see this section.</li> 
    </ul> <p>Note: Users who don't have the permissions you specify here cannot see the values of the fields in the section. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">In order to EDIT this section, people must have permission to</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>(Section Break only) Select the permissions users need on the object associated with the form in order to edit information in this section:</p> 
    <ul> 
     <li value="1"><b>Manage</b>: The user needs Manage permissions to the object to be able to edit this section.</li> 
     <li value="2"> <p><b>Admin only</b>: Only the <span class="WFVariablesAdminWF">Workfront administrator</span> can edit this section.</p> </li> 
    </ul> <p>Note:  
     <ul> 
      <li value="1">The access you are setting here is related to the permissions of the user to the object associated with the Custom Form, not the permissions of the user to the Custom Form itself.</li> 
      <li value="2">Users who don't have the permissions you specify here cannot edit the values of the fields in the section. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Conditional) If you need to change the display type of a field you have added, click the **Display Type** drop-down menu, then click the type you want.


   You can switch between the following field display types:

    
    
    *  Selection-type fields: Checkboxes, Dropdown, Radio Buttons
    * Text fields: Single Line Text Field, Paragraph Text Field, `Text Field with Formatting`
    
    
   For example, if you have created a Checkboxes field, you can change it to a Dropdown field or a Radio Buttons field. Or, if you have created a Single Line Text Field, you can change it to a Paragraph Text field.


   >[!NOTE]
   >
   >Consider the following when you want to change a field's display type from a Checkboxes field or a multi-select Dropdown field (a Dropdown allowing more than one option to be selected) to a single-select field type: 
   >
   >    
   >    
   >    * If you change to Radio Buttons, `Workfront` retains any multi-select values that a user may have entered in the field until the user changes and saves data in any part of the form. At this point, any values that were selected using the multi-select-type field are replaced by the selected Radio Button value.
   >    * If you change to a single-select Dropdown, `Workfront` retains any multi-select values that a user may have entered in the field until the user changes and saves the values in the field. At this point, any values that were selected using the multi-select-type field are replaced by the selected Dropdown value.
   >    
   >    




1. (Optional) Add any fields the form needs that have already been created for your organization, as explained in [Reuse an existing field](#add).
1. Continue on to [Position fields in a Custom Form](#configur).




## Position fields in a Custom Form {#position-fields-in-a-custom-form}

By default, a Custom Form is visible to each user in the system who has at least View access to the type of object associated with the form. If a Custom Form has been shared with certain users, they can attach it to objects where they have access to do so. 


If you make a Custom Form visible system-wide, users cannot automatically find the form to attach it to an object, nor can they see it in the Custom Forms area in Setup, if they have access to see that area.



1. Begin creating a Custom Form and add fields, as described in [Start creating a Custom Form](#start) and [Add a field to a Custom Form](#add2).

1.  (Optional)&nbsp;To position fields on the same row, drag one field next to the other until a line appears between them.


   When you drop the field, a gray box appears around the two fields to indicate that they share a row on the Custom Form.


   You can use the **Preview** button in the lower-right corner to see the fields as they will appear in the form.

1. (Optional)To position a field above or below another field, drag it above or below the field until a horizontal blue line appears between the fields.
1. Continue to [Configure user access to a Custom Form](#configur2).




## Configure user access to a Custom Form {#configure-user-access-to-a-custom-form}




1. Begin creating a Custom Form and add position fields, as described in the sections above.
1.  Open the **Form Sharing** tab to configure user access to the Custom Form.
1.  (Optional) To restrict visibility to you and the users in your Home Group, click the gear icon ![](assets/gear-icon-remove-system-wide-access.png), then click **Remove system-wide access**.


   >[!IMPORTANT] {type="important"}
   >
   >By making the Custom Form visible system-wide, users cannot automatically find the form to attach it to an object, nor can they see it in the Custom Forms area in Setup (if they have access to see that area). 



1.  (Optional) In the **Give Custom Form access to** field in the lower-left corner, designate specific users, teams, roles, groups, or companies that you want to have access to the Custom Form. 


   Ensure that all users that you specify have access to any objects associated with the form.


   In addition to being able to view the Custom Form on objects, users you specify can apply the Custom Form to an object if they have Manage rights on the object. (For information about how to apply a Custom Form to an object, see .) If you grant access to a group, members of the group who have `Workfront administrator` rights can also modify the Custom Form via the Setup area.


   >[!NOTE]
   >
   >At least one group must have access to the form. As the creator of the form, if you remove your Home Group from the form and do not give access to any other groups, your Home Group is re-added when you save the form.



1. Continue with [Complete a Custom Form](#complete).




## Complete a Custom Form {#complete-a-custom-form}




1. Begin creating a Custom Form and configuring a Custom Form, as described in the sections above.
1. (Optional) Click **Preview **to see how the form will look when being used, then click **End Preview** to return to editing the form.  

1.  Click **Save+Close**&nbsp;to save your changes.  



   Or  



   If you don't want to keep your changes on the form, click **Cancel**, then click **Go Ahead and Close**.   


1.  Apply the form to the object with which you associated it, as described in .


   After you apply the Custom Form to an object, users&nbsp;with permissions to manage the object and edit the Custom Form can edit the information in the custom fields.





## Copy a Custom Form to create a new one {#copy-a-custom-form-to-create-a-new-one}

You can create a new Custom Form that is based on an existing one. 



1.  Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Click **Custom Forms.**  

1. Select the Custom Form that you want to use as the basis for a new Custom Form, then click **Copy**.
1.  In the **Custom Form Copy** box that appears, type the following information:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 271px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Form Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify a new name for the Custom Form.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray">Form Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select which object type that you want to associate the Custom Form with. The object type that you select is the only object type to which the form can be applied.</p> <p>Note:  You can change the object of the form as you are copying a Custom Form. This is helpful when you want to create an identical form for two different objects. For example, you can copy an Issue Custom Form and create a Project Custom Form which has the same fields and the same logic as the original Issue form.</p> </td> 
  </tr> 
 </tbody> 
</table>


1. Click **Copy Form**.
1. Select the form that you just copied, then click **Edit**.
1. Make any changes to the form, then click **Save+Close**.
1.  Apply the form to the object with which you associated it, as described in .




## View a list of your Custom Forms and Custom Fields {#view-a-list-of-your-custom-forms-and-custom-fields}




1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png)..

1.  Click **Custom Forms**.


   On the **Forms** tab that displays, all of your organization's Custom Forms are listed in the Form List view, along with the object associated with each Custom Form (Custom Forms are object-specific) and the name of the user who created the form.

1.  Click the **Fields** tab.  



   All of your organization's Custom Fields display in the Field List view, along with information about the type of each field, instructions and details about the field, and a list of the Custom Forms that contain it.


   >[!NOTE]
   >
   >Custom Fields that are Section Breaks are not displayed in the Fields tab.



1.  Select the **Sections** tab.


   All the Custom Fields that are Section Breaks display in the Parameter Group List view, along with a list of Custom Forms that contain the Section Break.





## Rich text field storage in the API {#rich-text-field-storage-in-the-api}

If an object such as a project, issue, or task contains rich text, it is stored and accessible as a parameter value through the Workfront API.


Requesting text information from a project object that contains rich text can be done using the field **parameterValues**.

` `**Example: **`` A simple HTTP request could resemble the following:
`<pre>https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*</pre>` If this example project contained a custom form with 3 custom fields: calc field, paragraph text, and rich 1. Then the above request would return a response that resembles the following, where the field "rich 1" is a rich text parameter field and the text value is “**Hello ***World!*”:
`<pre>{	Data: {		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,		name: “new project with rich text”,		objCode: “PROJ”,		- parameterValues: {			DE:rich 1: “{				"blocks":[				{					"key":"7eibh",					"text":"Hello Word!",					"type":"unstyled",					"depth":0,					"inlineStyleRanges":[					{						"offset":0,						"length":6,						"style":"BOLD"					},					{						"offset":6,						"length":5,						"style":"ITALIC"					}					],					"entityRanges":[					],				"data":{				}				}				],			"entityMap":{			}		}”,		DE: paragraph text: “here is some paragraph text”,		DE: calc field: “here is a calc field entry”,		}	}}</pre>` For a more in depth look at how rich text information is stored and can be retrieved through the `Workfront` API, see [Rich text fields in the Workfront API](rich-text-field-api.md).
