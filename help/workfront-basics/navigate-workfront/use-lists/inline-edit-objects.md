---
filename: inline-edit-objects
product-area: projects
navigation-topic: use-lists
title: Inline edit items in a list in Adobe Workfront
description: You can edit objects inline when they display in a list or report. When you edit the information on objects displayed in a list or report, the object updates immediately.
---

# Inline edit items in a list in&nbsp;Adobe Workfront

You can edit objects inline when they display in a list or report. When you edit the information on objects displayed in a list or report, the object updates immediately.

When you inline edit a field contained in a custom form that is not attached to the object, the custom form is automatically added to the object. If the field exists on multiple custom forms, the custom form which was most recently updated is attached to the object.

For more information on lists, see [Get started with lists in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

While most objects displayed in lists or reports are inline editable in Adobe Workfront, there are some limitations, which include:

* You cannot edit calculated fields or Workfront built-in fields that are calculations.
* You can only edit fields associated directly to the objects in the list. You cannot edit fields that belong to objects associated with the objects in the list.   
  For example, you can edit the status of a task in a Task report, but you cannot edit the name of the project the task is associated with in the same report. You can edit the name of the project only in a Project report.
* You cannot inline edit fields when the view for a list is not displaying the default currency.  
  For information on displaying the default currency, see the section [Edit reports with unique currencies](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) in the article [Create financial data reports with unique exchange rates](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* You cannot edit flags and icons displayed in a list.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the area the list is in</p> <p>For example, to inline edit tasks in a project, you need Edit access to Projects.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage</p> <p>You must also have permissions to edit certain fields, such as custom fields, status, etc.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Edit objects inline

<ol> 
 <li value="1"> <p>Go to a list of objects you want to inline edit.</p> <p>The list should display fields that belong to the objects or fields that belong to objects associated with the objects in the list.</p> </li> 
 <li value="2"> <p>Locate the object you want to edit, then click inside any field in the list.</p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>"> <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>If you have multiple pages, you can locate an object by using:</p> 
   <ul> 
    <li> <p><span class="bold">Pagination</span>: Click the backward and forward arrows to navigate between pages.<br>Located at the bottom-right corner of the list, the pagination area remains sticky as you scroll through the list.</p> </li> 
    <li> <p><span class="bold">Quick filter</span>: Click the filter icon or type Alt+F to open the quick filter, then enter text to display only items that contain the entered text.<br>The quick filter is located in the list toolbar. For more information, see <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Apply the quick filter to a list</a>.</p> </li> 
   </ul> 
  </div> <p>If the field can be edited, this turns the field and all other fields displayed in the list into editable cells.</p> <p>  </p> </li> 
 <li value="3"> <p>Edit the information inside this cell, then press Enter.</p> <note type="note">
   If a custom field has been configured to allow formatting, you can bold, italicize, or underline text when inline editing the field in an updated list.
   <br>For information on configuring formatting for a custom field, see 
   <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.
   <br>For information on updated lists, see the section "The difference between the updated and the legacy lists" in the article 
   <a href="../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md" class="MCXref xref">Get started with lists in&nbsp;Adobe Workfront</a>.
  </note> </li> 
 <li value="4"> <p>Press Tab to move to the next editable cell.</p> </li> 
 <li value="5"> <p>(Conditional) If you are unable to save your edits and the cell is outlined in red, click inside the field to review the validation message that displays next to the cell and make the appropriate updates.</p> <p>Most commonly, this happens when the wrong format is used or a required field has been left blank.</p> </li> 
 <li value="6"> <p>After you finish modifying all the cells, press Enter to save your changes.</p> </li> 
</ol>

