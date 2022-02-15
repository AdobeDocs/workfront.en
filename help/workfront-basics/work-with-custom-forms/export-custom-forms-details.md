


# Export custom forms and object details in *`Adobe Workfront`* {#export-custom-forms-and-object-details-in-adobe-workfront}

You can export the Overview and the custom form information from the Details section of an object to a PDF file. You can then print or share the PDF with other users.


This functionality is supported for the following objects:



*  Projects
*  Tasks
*  Issues
*  Portfolio
*  Programs




>[!NOTE]
>
>The fields in the Details section that your *`Workfront`* or *`group administrator`* removed using a layout template do not display. 




## Access requirements {#access-requirements}

You must have the following:

<table class="TableStyle-TableStyle-HeaderRow" style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');caption-side: bottom;" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 300px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Any</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher for issues</p> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher for projects and tasks</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Access level configurations*</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>View or higher for Projects,&nbsp;Tasks, and Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="text-align: left;"> <p><span class="bold">Object permissions</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you start, you must: 



*  Have a custom form attached to an object or have the correct access to attach a custom form and edit the information on the form. 


  For information about attaching forms to objects, see [Add a custom form to an object](add-a-custom-form-to-an-object.md).


  For information about creating custom forms, see [Create or edit a custom form](create-or-edit-a-custom-form.md).





## Export information in the Details section {#export-information-in-the-details-section}

Exporting information from the Details section of an object is identical for all objects.



1. Go to a project, task, `portfolio, program,` or issue for which you have at least View permissions. 
1.  Click `Details` on the left panel.


   For example, for a project, click `Project Details`.

1.  (Optional) If there is no custom form attached to the object, start typing the name of a custom form in the `Add custom form field`, then click it when it appears in the list.


   You can add up to 10 forms.

1. (Optional) Update information in the Details section, then click `Save Changes`.
1.  Click the `Export` drop-down menu in the upper-right corner, select `Overview`, or the forms you want to export, then click `Export`.


   You can also select `Select all` if you want to export the Overview area and all the custom forms. 


   ![](assets/export-custom-form-button-menu.png)



   ` `**Tips: **``  The following scenarios may exist:

    
    
    *  When your group or *`Workfront administrator`* deselects all fields in the Overview area and the object has custom forms attached, the Overview section does not display.
    *  When your group or *`Workfront administrator`* deselects all fields in the Overview area and the object has no custom forms attached, the Export drop-down menu is not visible.
    *  When the object has no custom forms attached, you can export only the Overview area.
    *  Custom fields that are behind logic and are not visible on the form do not export. For information about adding logic to a custom form, see [Display logic and skip logic on a custom form](display-or-skip-logic-custom-form.md).
    
    
   A PDF file is produced and downloaded to your computer. The PDF file contains the following information:

    
    
    *  The name of the object the form is attached to
    *  The name of the user who exported the PDF
    *  The date and time when the PDF was produced
    *  The name of the forms you exported
    *  Information from the fields completed on the form
    
    



