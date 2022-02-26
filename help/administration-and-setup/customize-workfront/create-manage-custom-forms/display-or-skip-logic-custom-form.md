---
filename: display-or-skip-logic-custom-form
title: Display or skip logic on a Custom Form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Display logic and skip logic on a custom form
description: You can decide which sections of a custom form should be displayed or skipped based on the choices that a user makes when filling it out.
---

# Display logic and skip logic on a custom form

You can decide which sections of a custom form should be displayed or skipped based on the choices that a user makes when filling it out.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"> <p><em>Adobe Workfront</em> plan*</p> </td> 
    <td>Any</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><em>Adobe Workfront</em> plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>Administrative access to custom forms</p> <p>For information about how <em>Workfront administrators</em> grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how <em>Workfront administrators</em> grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="SnippetConditions.HIDE"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>Manage access to the <em>custom form</em></p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="SnippetConditions.HIDE"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the <em>custom form</em></p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your *Workfront administrator*.

## Considerations for using display logic and skip logic

* To add display logic on a custom field or a section break, you must have a multiple choice field (radio buttons, dropdown, or checkboxes) prior to the field you would like to display on the form.  

* If you want to add skip logic on a custom field, the field must be a multiple choice field.
* You cannot add skip logic to a section break.
* You can add both display logic and skip logic to a field if the field is:

  * A multiple choice field
  * Preceded by a multiple choice field
  * Followed by another field

* When copying forms with display logic or skip logic, the logic is copied to the new custom form.
* Keep the following in mind when you create a display rule for a custom form

  * Fields not included in a display logic statement show on a custom form, by default. 
  * Display logic can be applied to section breaks, as well as custom fields. 
  * Skip logic can be applied only to custom fields. 
  * You can create multi-field display logic statements. 
  * You can apply display rules to existing custom forms.

## Create a sample custom form that has display logic

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2"> In the left panel, click <span class="bold">Custom Forms</span> <img src="assets/custom-forms-icon.png">. </li> 
 <li value="3">Create the sample custom form:
  <ol>
   <li value="1">Click <span class="bold">New Custom Form</span>, then click <span class="bold">Project</span> in the drop-down list.</li>
   <li value="2">In the <span class="bold">Form Title</span> box, type <span class="bold">Sample custom form - Learning display logic and skip logic</span>.</li>
   <li value="3">Click <span class="bold">Add a Field</span> in the upper left corner.</li>
   <li value="4">Add a dropdown field called "Issue Field" by clicking <span class="bold">Dropdown</span>, then typing <span class="bold">Issue field</span> in the <span class="bold">Label</span> box.</li>
   <li value="5">Click <span class="bold">Save + Close</span> in the lower left corner.</li>
  </ol></li> 
 <li value="4"> Select the new <span class="bold"><span class="bold">Sample custom form - Learning display logic and skip logic</span></span> custom form, then click <span class="bold">Edit</span>. </li> 
 <li value="5">Add a new single line text field called "Other Research" by clicking <span class="bold">Single Line Text Field</span>, then typing&nbsp;<span class="bold">Other Research</span> in the <span class="bold">Label</span> box.</li> 
 <li value="6"> <p>Click <span class="bold">Add Logic</span> near the lower-left side of the <span class="bold">Edit Custom Form</span> screen.<br></p> </li> 
 <li value="7"> <p> In the box that appears, with the <span class="bold">Display Logic</span> tab open, set up the logic for when the <span class="bold">Other Research</span> field will appear on the form by clicking <span class="bold">Issue field</span> in the first drop-down, <span class="bold">Research Needed</span> in the second drop-down, and <span class="bold">Selected</span> in the third drop-down. </p> <p>Now, when someone selects <span class="bold">Research Needed</span> in the <span class="bold">Issue field</span> drop-down, the <span class="bold">Other Research</span> field will display.</p> </li> 
 <li value="8"> Click <span class="bold">Save</span> to close the <span class="bold">Field Logic</span> window, then click <span class="bold">Done</span> in the <span class="bold">Field Settings</span> area. </li> 
 <li value="9">Click <span class="bold">Preview</span> to make sure the logic appears the way you want it on the form.</li> 
 <li value="10">Click <span class="bold">End Preview</span> when you find that the logic works as expected.</li> 
 <li value="11">Click <span class="bold">Save + Close</span> on the <span class="bold">Edit Custom Form</span> window to save the form, then continue on to <a href="#skip-logic" class="MCXref xref">Skip logic on a custom form</a>below.</li> 
</ol>

## Skip logic on a custom form

Skip logic allows you determine which fields should be skipped, based on selections in the custom form. It functions similarly to display logic, but acts as the inverse: instead of making specific fields appear based on specific selections, you determine which fields should be skipped, based on selections.

To learn about skip logic on custom forms, continue working on the sample custom form you created in the section [Create a sample custom form that has display logic](#display-logic) above:

<ol> 
 <li value="1"><![CDATA[
          ]]>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2"> Click <span class="bold">Custom Forms</span>. </li> 
 <li value="3">Select the form <span class="bold">Sample custom form - Learning display logic and skip logic</span> that you created in the steps above, then click <b>Edit</b>. </li> 
 <li value="4"> Select the drop-down field you created named "Issue field." </li> 
 <li value="5"> Click the <span class="bold">Add Logic</span> button in the <span class="bold">Field Settings</span> sidebar. </li> 
 <li value="6"> In the <span class="bold">Field Logic</span> box, make sure the <span class="bold">Skip Logic</span> tab is selected. </li> 
 <li value="7"> Set the first drop-down to <b>No more research</b> and the second drop-down to <span class="bold">Selected</span>.</li> 
 <li value="8"> <p>In the <span class="bold">Then Skip To</span> drop-down, select <span class="bold">End of form.</span></p> <p>Now, when someone selects <span class="bold">No more research</span> in the <span class="bold">Issue field</span> drop-down field, the form will skip directly to the end of the form without displaying the <span class="bold">Other Research</span> field.</p> </li> 
 <li value="9"> Click <span class="bold">Save</span>. </li> 
 <li value="10"> Click <span class="bold">Preview</span> &nbsp;to make sure the logic applies&nbsp;the way you want it. </li> 
 <li value="11"> Click <span class="bold">Done</span> in the lower left side of the form. </li> 
 <li value="12"> Click <span class="bold">Save + Close</span> at the bottom of the Custom Forms window to save the changes you made to the form.&nbsp; </li> 
</ol>

