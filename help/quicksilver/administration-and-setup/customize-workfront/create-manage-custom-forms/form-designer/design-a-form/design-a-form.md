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

You can design a custom form with the Form Designer. You can attach custom forms to different Workfront objects to capture data about those objects.

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
   
   You can also click the X on an object type to delete it from the form. 

   >[!CAUTION]
   >
   >Deleting a custom form also deletes all custom data on the objects associated with the form. The deleted data cannot be recovered. Consider deactivating a custom form instead—when deactivate a custom form you no longer use, you retain all of the associated historical data.
   >
   >For more information, see [Delete object types on a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Next, you can start adding fields to your custom form. See the following sections: 
    * [Add text fields](#add-text-fields)
    * [Add calculated fields](#add-calculated-fields)
    * [Add radio buttons and checkboxes](#add-radio-buttons-and-checkboxes)
    * [Add typeahead, drop-down, and date fields](#add-typeahead-drop-down-and-date-fields)
    * [Add images, PDFs, and Videos](#add-images-pdfs-and-videos)
    * [Add Adobe XD files](#add-adobe-xd-files)

## Add fields to your custom form

 ### Add text fields

 You can add several different text fields to a custom form. 

+++ **Expand to see descriptions of available text fields**

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
    <td><p>(Required) This name is how the system identifies the field. When you are configuring the widget for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p>
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
    <td>Switch between single line and paragraph text fields.</td>
    <td><ul>
    <li>Single line text</li>
    <li>Paragraph text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hyperlink</td>
    <td> If you want to apply a hyperlink to the Descriptive Text you have typed, add it here.</td>
    <td><ul><li>Descriptive text</li></ul></td>
    </tr>
   </table>

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**. 

 ### Add calculated fields

 In a custom form, you can add a calculated custom field that uses existing data to generate new data when the custom form is attached to an object. 

 +++ **Expand to see the types of calculations a custom field can contain**

* A simple reference to a single built-in field.

  >[!INFO]
  >
  > **Example:** To calculate the revenue generated by projects and tasks, you could create a calculated custom field  that contains the built-in  field Actual Revenue. When someone attaches the custom form to a project or task, the revenue for the project or task displays in the field.

* An expression that references one or more fields. These can be custom fields, other calculated custom fields, and built-in  fields.

  >[!INFO]
  >
  >**Example:** To calculate the profit generated by projects and tasks, you could create a calculated custom field called Profit containing a mathematical expression that subtracts cost from revenue.
  >
  >To do this, you could use the mathematical expression SUB (subtract) with the built-in Workfront fields Actual Cost and Actual Revenue.
  >
  >In the steps below, you can see how this example can be carried out.

 +++

 To add a calculated field:

 >[!IMPORTANT]
>
>Before you create a new calculated custom field, identify the existing fields that you want to include so that you are sure that the data necessary for the calculation is present in Workfront.

1. On the left side of the screen, find **Calculated** and drag it to a section on the canvas.

    ![](assets/drag-field-to-section.png)

1. On the right side of the screen, configure the options that are available for the type of custom field you are adding:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td>Type a label for the field. This is what users will see when they use the custom form. The field <b>Name</b>, which fills in automatically, is referenced by Workfront in reports.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instructions</td> 
      <td> By default, the formula you create for the field is stored here. You can add text to provide additional information about the field and the formula in it. This can be useful in two ways: 
       <ul> 
        <li> <p>As a reminder of what the formula is and how it works. This is especially helpful if you plan to use this calculated custom field on multiple forms.</p> </li> 
        <li> <p>As a tooltip users can see when they hover over the field. You add any text here that you want them to see in the tooltip.</p> <p>If you don't want them to see the formula in the tooltip, which might be confusing for them, you can hide it. For instructions, see the table row "Display formula in instructions" in the section <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">Build the calculation for your calculated custom field</a> in this article.</p> </li> 
       </ul> <p>For information about using the same calculated custom field on a new form, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Reuse an existing calculated custom field in a custom form</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>The format in which you want the results of the field to be stored and displayed.</p> <p>If the field will be used in mathematical calculations, always use a <strong>Number</strong> or a <strong>Currency</strong> format. When you select Number or Currency, the system automatically truncates numbers that start with 0.</p> 
      <p><b>IMPORTANT</b>: Before you choose a format, consider the correct format for the new field. The format field cannot be edited after the custom form is saved. And selecting the wrong format could impact future calculations and aggregate values in report and list groupings.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Calculation** box, begin building your calculation: 
   1. Click **Maximize** to open the Calculation Editor and build your calculation.</p> 
    A calculation usually starts with an expression, followed by parentheses containing the fields you want to reference when the custom form is attached to an object. 

      Each field must be surrounded with curly brackets. When you start typing the name of a field, the system makes suggestions and you can select one to insert it into your calculation.

      +++ **Expand to see syntax required in calculated custom fields**

      Each field must use the syntax explained below, with curly brackets around each field name. When you start typing the name of a field, the system makes suggestions and you can select one  to insert it into your calculation. If you enter data in a calculation incorrectly, a warning message alerts you. You cannot save the form unless you edit your calculation to contain valid fields and a valid calculated expression.

      >[!NOTE]
      >
      >Currently, the system makes suggestions only when you start typing the name of a field you want to reference on an object that the custom form will be attached to. Fields from the parent object are not suggested. 

      **Surround field names with curly brackets**

      * If you want the calculation to reference a built-in field, the name of the field must be surrounded by curly brackets.

      For example: `{actualRevenue}`

      Field names are case-sensitive and must appear in the calculation exactly how they appear in the Workfront system.

      * If you want the calculation to reference a custom field, the name of the field must be surrounded by curly brackets, and preceded by `DE:` within the brackets.

         For example: `{DE:Profit}`

         The system lists all of the custom fields you can choose from when you type `DE:`.  

         * If you want the calculation to reference a field that will pull data from  the *parent* object when the custom form is attached to an object, you must precede the field name with the object type of the parent object, also in curly brackets.

         For example, if the custom form is configured to work with tasks, and you want the field to calculate the actual revenue of the parent object when the form is attached to a task, you need to indicate `Project` as the object type of the field: 
         
         `{project}.{actualRevenue}`
         
         Or, if it's a custom field: 
         
         `{project}.{DE:profit}`

         If you're not sure what the object type of the parent object will be because the custom form is configured for multiple object types, you can use the wildcard filter variable `$$OBJCODE` to allow the calculation to work for each of the possible types. For more information, see the Calculated custom fields in multi-object custom forms section below.

         **Separate items with periods**

         When you reference a related object in a calculated custom field, you must separate object names and attributes with periods.

         For example, in a task-type custom form, to display the name of the Portfolio Owner in a calculated custom field, you would type the following: 

         `{project}.{porfolio}.{owner}`

         This would determine the following: From the object of the custom form (a task), you can access the next object related to the task (a project). From there, you can access the next related object to the project (a portfolio), then to the project (a portfolio), then reference the fields defined for portfolio object (the owner)

         **Name syntax for referencing a custom field**

         When you reference another custom field in a calculated custom field, you need to enter the name of the field appears as it displays in the Workfront user interface.

         For example, to reference the selected option in a custom field labeled Executive sponsor, you would type the following:

         `{DE:Executive sponsor}`

         >[!NOTE]
         >
         >The syntax for a typeahead field is a bit different than it is for other types of fields because you need to add `:name` at the end.
         >
         >For example, to reference the selected option in a custom typeahead field named "Executive sponsor," you would type:
         >
         >`{DE:Executive sponsor:name}`


         **Calculated custom fields in multi-object custom forms**

         In a multi-object custom form, the selected object types must be compatible with all fields referenced in the form's calculated custom fields. If there is an incompatibility, a message alerts you to make adjustments.

         >[!INFO]
         >
         >**Example:**
         >
         >In a custom form configured to work with the Task object type, you create a calculated custom field named In Charge. You configure it to reference the built-in field so that it can show the name of the primary assignee in charge whenever the form is attached to a task:
         >
         >`{assignedTo}.{name}`
         >
         >Later, you add the Project object type to the custom form. A warning message tells you that the Project object type is incompatible with the calculated custom field.

         When this occurs, you can do one of the following:

         * Remove one of the two incompatible items from the custom form—either the object type or the referenced calculated custom field.
         * Keep both items and use the wildcard filter variable `$$OBJCODE` as a condition in an IF expression to create two different versions of the In Charge field. This allows the field to function successfully, no matter which type of object the form is attached to. 

         >[!INFO]
         >
         >**Example:** Though there is no Assigned To: Name field in projects, there is a built-in Owner field (which fills in automatically with the name of the person who created the project, unless someone manually changes this).
         >
         >So, in your custom In Charge field, you could use `$$OBJCODE` as shown below to reference the Owner field when the custom form is attached to a project, and the Assigned To: Name field when the form is attached to a task:
         >
         >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

         For more information about variables like `$$OBJCODE,` see [Wildcard filter variables](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

         **Automatic updates of calculated custom fields**

         Calculated custom fields on an object recalculate automatically when the following things happen:

         * Something on the object changes, such as a daily timeline calculation.
         * Someone edits another field that is referenced by a calculated custom field on the object.
         * The calculated expression is empty and the field contains a value—this sets the value to null.

            >[!NOTE]
            >
            ><div>In a custom form attached to an object, date and time statements in calculated custom fields are calculated and saved by Coordinated Universal Time (UTC), not by the time zone configurations set for your organization's instance and your user profile. Calculations in a custom form generate based on each users' individual time zones.</div>

         +++

   1. Click in the large text box, then click **Expressions** and **Fields** that are available to add them to your calculation.

      You can also start typing an expression or field in the large text box, then select it when it displays. Each item displays with an "F" for field or an "E" for expression.

      If you type an opening parenthesis, the closing parenthesis is added automatically.

      +++ **Expand to see helpful tips**
      >[!TIP]
      >
      >You can do any of the following to get help with your calculation:
      > 
      >* Hover over an expression in your calculation to see a description, an example showing how it can be used, and a "Learn More" link to more information in the article [Calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
      >* Use the color coding to identify the components you have added. Expressions display in blue and fields display in green.
      >  ![](assets/colors-fields-expressions.jpg)
      >* Find calculation errors, highlighted in pink, as you go. You can hover over a highlighted error to display a brief description of its cause.
      >  ![](assets/error-help.png) 
      >* In the area below your calculation, preview the results on an existing Workfront object.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![](assets/preview-calc.jpg)
      >* Reference expressions in a long calculation using the line numbers that display on the left.

      +++
   1. Click **Minimize** when you are finished creating the calculation for the calculated custom field.

      >[!NOTE] 
      >
      >In the display area on the right, the field displays *12345.* This is merely an indicator to remind you that the field is a calculated custom field while you are creating or editing the custom form. When the form is attached to an object and users are filling it out, they see the result of the calculation in the field, never the *12345* indicator.

   1. (Optional) Use any of the following options to further configure your calculated custom field:

      <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Add Logic</td> 
      <td>You can add Display Logic to determine whether the calculated field displays, based on at least one choice that a user makes in a preceding multiple choice field (Dropdown, Checkboxes, or Radio Buttons) when filling out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>. <p>This is available only when at least one checkbox, radio button, or a drop-down field precedes the calculated custom field on the form. </p> <p>Skip Logic is unavailable for calculated custom fields.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Update previous calculations</td> 
      <td>When you are editing an existing calculated custom field, you can select this option to trigger an update in the calculation when you save the custom form. This happens only once when you save the custom form. The option returns to its disabled state after you do so.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Display formula in instructions</td> 
      <td>Leave this option enabled if you want the users who fill out the custom form to see the field's formula when they hover over the field. For more information, see the information about <a href="#instructions" class="MCXref xref">Instructions</a> earlier in this table.</td> 
     </tr> 
    </tbody> 
   </table>

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**. 

 ### Add radio buttons and checkboxes

 You can add radio buttons and checkboxes to a custom form. 

+++ **Expand to see descriptions of available fields**

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

+++ **Expand to see descriptions of available fields**

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

To add typeahead and date fields:

1. On the left side of the screen, find one of the following fields and drag it to a section on the canvas.

    * Typeahead
    * Dropdown
    * Date Field

    ![](assets/drag-field-to-section.png)

1. On the right side of the screen, configure the options that are available for the type of custom field you are adding:

    <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Field setting</td>
    <td>Description</td>
    <td>Available for </td>
    </tr>
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the custom field. You can change the label at any time.</p> <p><b>IMPORTANT</b>: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Dropdown</li>
    <li>Date Field</li>
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
    <li>Typeahead</li>
    <li>Dropdown</li>
    <li>Date Field</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Type any additional information about the custom field. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Dropdown</li>
    <li>Date Field</li>
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
    <li>Dropdown</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Display Type</td> 
      <td>Switch the type of option selection you want for the field.</td> 
       <td><ul>
    <li>Dropdown</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Display Time of Day</td> 
      <td>Select this option if you want to show the time of day along with the date in the field.</td> 
         <td><ul>
    <li>Date Field</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Referenced Object Type</td> 
      <td> <p>Select the object type that you want to associate with the field.</p> <p>Once you have clicked Apply or Save+Close, you cannot change the object type for the field.</p> <p><b>NOTE</b>:   
        <ul> 
         <li>If your Workfront administrator customized the name for Portfolios, Programs, or Projects in the Workfront user interface, the default Workfront name for the object appears in this drop-down list, not the customized name. See your Workfront administrator if you need help with this.<br></li> 
         <li>The following object types are supported in the iOS and Android Workfront Mobile Apps: User, Company, Group, Job Role, Portfolio, Program, Project, and Template.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Make a required field</td> 
      <td>Select this option if you want the field to be required in order for the user to complete the custom form. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Dropdown</li>
    <li>Date Field</li>
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
    <li>Dropdown</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**. 

 ### Add images, PDFs, and Videos

 You can add an images, PDFs, and Videos to a custom form. Users who work with the object the custom form is attached to can see the image, PDF, or video only in the following areas:

* The object's Details area (for example, for a project, the Project Details area)
* The Edit box for the object, if it has the new Adobe Workfront experience look and feel (for example, the Edit Project and Edit Task boxes)

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

 +++ **Expand to see descriptions of available fields**

* **Image**: Allows users to add _____ image files.
* **PDF**: Allows users to add PDFs
* **Videos**: Allows users to add ____ video files.

+++

 To add an images, PDFs, or videos:

1. On the left side of the screen, find one of the following fields and drag it to a section on the canvas.

   * Image
   * PDF
   * Video

   ![](assets/drag-field-to-section.png)

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
      <td> <p>(Required) This name is how the system identifies the widget.</p> <p>When you are configuring the widget for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p> <p><b>IMPORTANT</b>: Though it's possible to do so, we recommend that you do not change this name after you or other users start using the custom form in widget. If you do, the system will no longer recognize the widget where it might now be referenced in other areas of Workfront. </p> <p>Each widget name must be unique in your organization's Workfront instance. This way, you can reuse one that was already created for another custom form. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Required) Type or paste the URL of the widget where it is stored on the internet.</p> 
      <p>If you are adding a video widget, currently you can do so by adding the following in the URL box:</p> 
      <ul> 
      <li> <p>YouTube or Vimeo link</p> </li> 
      <li> <p>Google Drive video link</p> </li> 
      <li> <p>Link to video with MP4 and MOV extension</p> </li> 
      <li> <p>Link to video already uploaded to the Documents area in your Workfront instance. For instructions, see <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Add a video widget to a custom form from the Documents area</a> in this article.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Type any additional information about the widget. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Size</td> 
      <td>Change the display size of the widget as needed.</td> 
     </tr> 
    </tbody> 
   </table>

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**. 

#### **Add a video widget to a custom form from the Documents area**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>When you add a video to a custom form this way, only the permissions set for the custom form apply to the video when users access the form on an object, not the permissions that were set for the video in the Documents area.

1. Go to the video in the Documents area and generate a proof for it, as described in [Create an interactive proof for a website or other web content](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Open the proof.
1. Right-click anywhere on the video, then select **Copy Video Address**.
1. In the custom form where you are adding the video widget, paste the copied address in the **URL** box.
1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**. 

 ### Add Adobe XD files

 You can add an Adobe XD prototype directly to a custom form. Users who work with the object the custom form is attached to can see the Adobe XD file only in the following areas:

* The object's Details area (for example, for a project, the Project Details area)
* The Edit box for the object, if it has the new Adobe Workfront experience look and feel (for example, the Edit Project and Edit Task boxes)

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

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**. 

 ## Organize your custom form

 For information on how to organize your form, see [Organize a form with the Form Designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md). 