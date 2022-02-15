---
filename: delete-or-deactivate-a-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
---



# Delete or deactivate a custom form {#delete-or-deactivate-a-custom-form}

You can delete or deactivate a custom form from the system.


` `**Warning: **``Deleting a custom also deletes all custom data on the objects associated with the form. The deleted data cannot be recovered. Consider deactivating a custom form instead—when deactivate a custom form you no longer use, you retain all of the associated historical data.


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table class="TableStyle-TableStyle-List-options-in-steps" style="margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Any</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Administrative access to custom forms</p> <p>For information about how <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span> grants this access, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="SnippetConditions.HIDE"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage access to the <span class="mc-variable snippet-variables-custom-forms.custom-form-or-field variable varname">custom form</span></p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your *`Workfront administrator`*.


## Delete a custom form {#delete-a-custom-form}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Custom Forms.`
1. Select the custom form, then click `Delete`.
1.  If you are sure you want to permanently delete the custom form and all associated data on objects where it was attached, click `Yes, Delete It`. 




## Deactivate a custom form {#deactivate-a-custom-form}

You can deactivate custom forms you no longer use while retaining all of the associated historical data. 


If you deactivate a custom form, the custom form does not display in any drop-down menus on the object. However, the form does still display on any object it is attached to.


Fields on a deactivated custom form are still available to inline-edit in a View. If you add a field during an inline edit, the form attaches automatically, even though the custom form is deactivated.



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click the name of the custom form you want to deactivate.
1. Click the `Form Settings` tab.
1. Disable the `Is Active` option.
1. Click `Save + Close`.


