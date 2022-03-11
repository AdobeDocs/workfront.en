---
filename: calculated-field-example-edit-history-of-another-field
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: Calculated custom field example: display a field's edit history
description: If users update custom fields on a regular basis and you want to capture a log of all the changes made to a field as well as a date when the changes happen, you can capture this information in a calculated custom field.
---

# Calculated custom field example: display a field's edit history

If users update custom fields on a regular basis and you want to capture a log of all the changes made to a field as well as a date when the changes happen, you can capture this information in a calculated custom field.

The following example shows you how to build the *Instructions Edit History* calculated field to capture all the change made to a single-line text field called *Instructions*.

>[!TIP]
>
>You can follow this example for all types of custom fields, not just single-line text fields.

This does this following:&nbsp;

* Limits the *Instructions Edit History* field to the most recent 2000 characters to stay within the Workfront database limit. 
* Checks if the current value of the *Instructions* field matches the front of the *Instructions Edit History* value; it assumes it is blank and if it is not, it does the following:&nbsp;

  * If they match, it leaves the *Instructions Edit History* as is; 
  * If they do not match, it replaces the *Instructions Edit History* with the latest value in the *Instructions* field, followed by the current date in parentheses, a vertical bar, and the previous *Instructions Edit History*, which preserves the previous value(s) and the date(s) when they were entered.

## Access requirements

You must have the following:

<table cellspacing="15"> 
 <caption style="text-align: left;"> 
  <p>*To find out what plan, license type, or access you have, contact your <span>Workfront administrator</span>.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><span>Adobe Workfront</span> plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p><span>Workfront</span> license*</p> </td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Access level configurations*</span> </td> 
   <td> <p>Administrative access to Custom&nbsp;Forms</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Object permissions</span> </p> </td> 
   <td> <p>Manage permissions on the custom forms </p> <p>For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisites

To add a calculated field that displays a field's edit history to a custom form, you must first:

* Create the custom form 
* Add the field whose history you want to capture to the custom form

## Display a field's edit history

<ol> 
 <li value="1"> <p>Go to a custom form where you want to add the calculated field.</p> <note type="important">
   You must add the field whose history you want to capture on the form first and save the form at least once before you can add the calculated field. 
  </note> </li> 
 <li value="2"> <p>To create the single-line text custom field, for example, do the following:</p> 
  <ol> 
   <li value="1"> <p>Click&nbsp;<span class="bold">Single Line Text Field</span>.</p> </li> 
   <li value="2"> <p>Specify a <span class="bold">Label</span> for the custom field, for example: <i>Instructions</i>.</p> </li> 
   <li value="3"> <p>(Optional) Click the <span class="bold">Name</span> field to update it. The Name of the field matches the Label you just entered by default. </p> </li> 
   <li value="4"> <p>For this example, select&nbsp;<span class="bold">Text</span> in the <span class="bold">Format</span> field to format the custom field as text. This is the default. </p> </li> 
   <li value="5"> <p>Click&nbsp;<span class="bold">Done</span>, then <span class="bold">Save +&nbsp;Close</span>. </p> </li> 
  </ol> </li> 
 <li value="3"> <p>Click the name of the form you added the <i>Instructions</i> field to. </p> </li> 
 <li value="4">Click <span class="bold">Calculated</span> to add a calculated custom field to the form.<br></li> 
 <li value="5">Specify a <span class="bold">Label</span> for the calculated custom field, for example: <i>Instructions Edit History</i>. This is the field that will capture any changes made to the <i>Instructions</i> text field you created in Step 2. </li> 
 <li value="6">(Optional) Click the <span class="bold">Name</span> field to update it. The Name of the field matches the Label you just entered by default. </li> 
 <li value="7"> <p> In the <span class="bold">Calculation</span> field, specify the following calculation for your custom field:</p> <p><code>LEFT(IF(LEFT(Instructions Edit History,LEN(IF(ISBLANK(Instructions),"-",Instructions)))=Instructions ,Instructions Edit History,CONCAT(IF(ISBLANK(Instructions),"-",Instructions)," (",$$NOW,") | ",Instructions Edit History)),2000)</code> </p> <note type="tip">
   In the above code, replace 
   <i>Instructions</i> with the exact name of your single-line text field whose history you are tracking and 
   <i>Instructions Edit History</i> with the exact name of your calculated field. 
  </note> </li> 
 <li value="8"> <p>(Recommended) Type the same code in the <span class="bold">Instructions</span> field on the calculated field on the form. </p> </li> 
 <li value="9"> <p>Always select&nbsp;<span class="bold">Text</span> in the <span class="bold">Format</span> field to format the calculated custom field as text. This is the default. </p> </li> 
 <li value="10">Click&nbsp;<span class="bold">Done</span>, then <span class="bold">Save+Close</span>.</li> 
 <li value="11"> <p>(Optional)&nbsp;Attach the custom form to an object.</p> <p>When someone changes the information in the Instructions field</p> </li> 
</ol>

&nbsp;
