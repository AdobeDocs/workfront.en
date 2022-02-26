---
filename: error-message-field-used-in-multi-form-config
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Error saving custom field: "There is a slight problem. [That field] is used in a multi-form configuration ..."
description: When you change a calculation on a calculated custom field on a custom form, Adobe Workfront might display the following warning:
---

# Error saving custom field: "There is a slight problem. [That field] is used in a multi-form configuration ..."

##  Problem

When you change a calculation on a calculated custom field on a custom form, *Adobe Workfront* might display the following warning:

There's a slight problem

[The field] is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation.

## Cause

This means that somewhere in your *Workfront* environment you have an object that has at least two different custom forms attached to it and both forms contain the field you are trying to change

In this case, you cannot change the calculation for the custom field in&nbsp;Form 1 because it would conflict with the formula in the same field on Form 2.

##  Solution

To resolve this conflict you must find the object that has the two forms in it and remove one of the forms from the object.

<ol> 
 <li value="1"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
     <span class="bold">Main Menu</span> icon 
     <img src="assets/main-menu-icon.png"> in the upper-right corner of 
     <em>Workfront</em>, then click 
     <span class="bold">Setup</span> > 
     <span class="bold">Custom&nbsp;Forms</span> > 
     <span class="bold">Fields</span>> apply the 
     <span class="bold">Field List</span> view to find the Calculated Field you are trying to modify and make note of every Custom Form on which it is used (e.g. Form 1, Form 2, Form 3) . 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner of 
    <em>Workfront</em>, then click 
    <span class="bold">Setup</span> > 
    <span class="bold">Custom&nbsp;Forms</span> > 
    <span class="bold">Fields</span>> apply the 
    <span class="bold">Field List</span> view to find the Calculated Field you are trying to modify and make note of every Custom Form on which it is used (e.g. Form 1, Form 2, Form 3) . 
   </MadCap:conditionalText> </p> </li> 
 <li value="2"> <p>Click&nbsp;<span class="bold">Forms</span>, then apply the <span class="bold">Form List</span> view. </p> </li> 
 <li value="3">Click the <span class="bold">Filter</span> drop-down list, then <span class="bold">New Filter</span>. </li> 
 <li value="4">Click&nbsp;<span class="bold">Add a Filter Rule</span>, then start typing "Custom&nbsp;Form Name" and select this value when it displays in the list. </li> 
 <li value="5">Select <span class="bold">Equal</span> for your filter modifier, then start typing the name of each form you made a note of in Step 1, then select it when it displays in the list. For example, Custom Form Name Equals Form 1,&nbsp;Form 2,&nbsp;Form 3. </li> 
 <li value="6">Click&nbsp;<span class="bold">Save Filter</span>, then name the new filter, and click&nbsp;<span class="bold">Save Filter</span>. </li> 
 <li value="7">In the list of forms, make note of the object type of the filter which displays in the <span class="bold">Type</span> column. For example, "Issue."</li> 
 <li value="8"> <p>On each Custom Form you found in Step 1, create a new Checkbox custom field with a single default value of Yes. For example, Field 1 on Form 1 = Yes, Field 2 on Form 2 = Yes, Field 3 on Form 3 = Yes. This means "The Calculated Custom&nbsp;Field exists on Form 1," or "The Calculated Custom Field exists on Form 2," etc. </p> </li> 
 <li value="9"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Search icon</span> <img src="assets/search-icon.png"> in the upper-right corner of the screen, then click&nbsp;<span class="bold">Advanced Search</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Search icon</span> <img src="assets/search-icon.png"> in the upper-right corner of the screen, then click&nbsp;<span class="bold">Advanced Search</span>. </p> </li> 
 <li value="10"> <p> Click the object of your custom form (for example, Issue), then click&nbsp;<span class="bold">Filter your results</span>, then click <span class="bold">Add a filter</span>. </p> </li> 
 <li value="11"> <p>Start typing the name of a Checkbox field in the <span class="bold">Start typing field name ...</span> and click it when it displays in the list, then select <span class="bold">Equal</span> and type "Yes" (without quotation marks) in the following box. For example: Field 1 Equal (Case Sensitive)&nbsp;Yes. </p> </li> 
 <li value="12"> <p>Click <span class="bold">Add a Filter</span> and add all Checkbox fields to your Advanced&nbsp;Search. </p> <p>Look for every possible combination. For example, build several filters with these combinations, as listed below. Only in one situation you should actually find objects with multiple forms containing the same calculated fields attached.&nbsp;For example, you may find the following scenarios: </p> <p>Field 1= Yes + Field 2 = Yes + Field 3 = Yes (no objects, for example)</p> <p>Field 1= Yes + Field 2 = Yes (no objects, for example) </p> <p>Field 1= Yes + Field 3 = Yes (two objects, for example)</p> <p>This means that the calculated field exists on both Form 1 and Form 3, because the corresponding Checkbox fields (Field 1 and Field 3) exist on these objects. </p> <p>Field 2 = Yes + Field 3 = Yes (no objects, for example)</p> </li> 
 <li value="13"> <p>Open each of the objects found in Step 12 and remove one of the two forms, then save the object. </p> <note type="note">
   You might need to edit the custom form that remains attached to the object to add the fields from the form you are removing from the object. This way, you can preserve the custom data information on the object.
  </note> </li> 
 <li value="14"> <p>Now, go back to your custom form and edit the calculation for the custom field you were originally trying to update. This time, <em>Workfront</em> should not encounter any more conflicts when saving the new calculation. </p> </li> 
 <li value="15"> <p>(Optional) Remove the Checkbox fields from the forms</p> <p>Or</p> <p>Delete the Checkbox fields from <em>Workfront</em>. </p> </li> 
</ol>

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error&nbsp;while editing a calculated Custom Field on a Custom Form:&nbsp;</p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple Custom Forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task&nbsp;with Custom Forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on Custom Form A.&nbsp;</p>
<h2>Solution</h2>
<p>Remove the field from the Custom Form and replace it with a new one containing the desired calculation.&nbsp;&nbsp;</p>
<p>To understand what Custom Forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing Custom Forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what Custom Form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a Custom Form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->

`<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">  <h2>Problem</h2>  <p>You get the following error&nbsp;while editing a calculated Custom Field on a Custom Form:&nbsp;</p>  <p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>  <h2>Cause</h2>  <p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple Custom Forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>  <p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>  <p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>  <p>For example, you have a task&nbsp;with Custom Forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on Custom Form A.&nbsp;</p>  <h2>Solution</h2>  <p>Remove the field from the Custom Form and replace it with a new one containing the desired calculation.&nbsp;&nbsp;</p>  <p>To understand what Custom Forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing Custom Forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>  <p>To understand what Custom Form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>  <p>For more information about creating a Custom Form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p> </blockquote>`  