---
filename: inline-edit-objects
product-area: projects
navigation-topic: use-lists
---



# Inline edit items in a list in  *`Adobe Workfront`* {#inline-edit-items-in-a-list-in-adobe-workfront}

You can edit objects inline when they display in a list or report. When you edit the information on objects displayed in a list or report, the object updates immediately.


When you inline edit a field contained in a custom form that is not attached to the object, the custom form is automatically added to the object. If the field exists on multiple custom forms, the custom form which was most recently updated is attached to the object.


For more information on lists, see [Get started with lists in Adobe Workfront](view-items-in-a-list.md).


While most objects displayed in lists or reports are inline editable in *`Adobe Workfront`*, there are some limitations, which include:



* You cannot edit calculated fields or *`Workfront`* built-in fields that are calculations.
* You can only edit fields associated directly to the objects in the list. You cannot edit fields that belong to objects associated with the objects in the list.   
  For example, you can edit the status of a task in a Task report, but you cannot edit the name of the project the task is associated with in the same report. You can edit the name of the project only in a Project report.
* You cannot inline edit fields when the view for a list is not displaying the default currency.  
  For information on displaying the default currency, see the section [Edit reports with unique currencies](create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) in the article [Create financial data reports with unique exchange rates](create-financial-data-reports-unique-exchange-rates.md).

* You cannot edit flags and icons displayed in a list.




## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to the area the list is in</p> <p>For example, to inline edit tasks in a project, you need Edit access to Projects.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level.<br>For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage</p> <p>You must also have permissions to edit certain fields, such as custom fields, status, etc.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Edit objects inline {#edit-objects-inline}




1.  Go to a list of objects you want to inline edit.


   The list should display fields that belong to the objects or fields that belong to objects associated with the objects in the list.

1.  Locate the object you want to edit, then click inside any field in the list.

   ` `**Tip: **`` If you have multiple pages, you can locate an object by using:

    
    
    *  `Pagination`: Click the backward and forward arrows to navigate between pages.  
      Located at the bottom-right corner of the list, the pagination area remains sticky as you scroll through the list.
    *  `Quick filter`: Click the filter icon or type Alt+F to open the quick filter, then enter text to display only items that contain the entered text.  
      The quick filter is located in the list toolbar. For more information, see [Apply the quick filter to a list](apply-quick-filter-list.md).
    
    
   If the field can be edited, this turns the field and all other fields displayed in the list into editable cells.


   ![](assets/nwe-editable-cells-350x131.png)



1.  Edit the information inside this cell, then press Enter.


   >[!NOTE]
   >
   >If a custom field has been configured to allow formatting, you can bold, italicize, or underline text when inline editing the field in an updated list.  
   >For information on configuring formatting for a custom field, see [Create or edit a custom form](create-or-edit-a-custom-form.md).  
   >For information on updated lists, see the section "The difference between the updated and the legacy lists" in the article [Get started with lists in Adobe Workfront](view-items-in-a-list.md).



1.  Press Tab to move to the next editable cell.
1.  (Conditional) If you are unable to save your edits and the cell is outlined in red, click inside the field to review the validation message that displays next to the cell and make the appropriate updates.


   Most commonly, this happens when the wrong format is used or a required field has been left blank.

1.  After you finish modifying all the cells, press Enter to save your changes.


