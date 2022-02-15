---
filename: inline-edit-objects
product-area: projects
navigation-topic: use-lists
---




# Inline edit objects {#inline-edit-objects}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


## Inline editing considerations {#inline-editing-considerations}

There are some limitations when inline editing a list of objects:



* You can only edit fields or objects you have permissions to Contribute or Manage.
* You can only edit fields you have permissions to Edit.  
  For example, you may not have access to edit certain custom fields, or the status of an item.
* You cannot edit calculated fields or `Workfront` native fields that are calculations.&nbsp;
* Fields that belong to objects associated with the objects in the list are not editable.   
  Only fields associated directly to the objects in the list can be edited.  
  For example, you can edit the Status of a task in a task report, but you cannot edit the Name of the Project the Task is associated with in the same report. You can edit the Name of the Project only in a Project report.&nbsp;

* You cannot edit flags and icons displayed in a list.&nbsp;
* When an object does not have the custom form which contains the field displayed in the list associated with the object, and you inline edit the field in a list, this action automatically attaches the custom form to the object.  
  If the field exists on multiple custom forms, the custom form which was most recently updated is attached to the object.




## Edit objects inline {#edit-objects-inline}

You can edit objects inline when they display in a list or report. Virtually all objects displayed in lists or reports are inline editable in `Workfront`.


When you edit the information on objects displayed in a list or report, the object is also updated immediately.&nbsp;


To inline edit any object:



1. Go to a list of objects you want to inline edit.  
   The list should display fields that belong to the objects or fields that belong to objects associated with the objects in the list.&nbsp;&nbsp;
1. Click inside any field displayed in the list.  
   If the field can be edited, this turns the field and all other fields displayed in the list into editable cells.  

1.  Edit the information inside this cell, then press Enter.


   >[!NOTE]
   >
   >`If a custom field has been configured to allow formatting, you can bold, italicize, or underline text when inline editing the field in an updated list.  
   >For information on configuring formatting for a custom field, see` [Create a Custom Form](create-a-custom-form.md) `.  
   >For information on updated lists, see [View items in a list](view-items-in-a-list.md).` 



1. Press Tab to move to the next editable cell.
1. (Optional) When you enter information in the wrong format, or leave a required field blank, the editable cell is outlined in red and you cannot save the new information on that field.  
   Click inside the field and a validation message displays next to the cell to inform you why the information you entered cannot be saved.&nbsp;
1. After you finish modifying all the cells, press Enter to save your changes.&nbsp;


