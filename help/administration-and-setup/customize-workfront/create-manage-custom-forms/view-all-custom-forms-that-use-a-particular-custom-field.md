---
filename: view-all-custom-forms-that-use-a-particular-custom-field
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
---



# View all custom forms that use a particular custom field {#view-all-custom-forms-that-use-a-particular-custom-field}

You can find out which custom forms are using a custom field that you want to change. It’s important to assess whether those custom forms will need adjustments in order to keep working properly after you make any changes to the field or delete the field.


##  

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Administrative access to custom forms</p> <p>For information about how <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span> grants this access, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your *`Workfront administrator`*.
{#access-requirements-you-must-have-the-following-to-perform-the-steps-in-this-article-adobe-workfront-plan-any-adobe-workfront-license-plan-access-level-configurations-administrative-access-to-custom-forms-for-information-about-how-workfront-administrators-grants-this-access-see-grant-users-administrative-access-to-certain-areas-to-find-out-what-plan-license-type-or-access-level-configurations-you-have-contact-your-workfront-administrator}



## Find out which custom forms use a particular custom field {#find-out-which-custom-forms-use-a-particular-custom-field}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  In the left panel, click `Custom Forms`.
1.  Open the custom form containing the field you want to modify, then click the field on the right side of the screen.


   A warning message displays if the field is used on another custom form.


   ![](assets/warning-message-fields-used-elsewhere-350x242.png)



1.  Click the blue arrow in the warning message to see which custom forms are using the field.
1.  (Optional) Click the name of any custom form listed to go to that form and consider what changes you might want to make there if you modify the field.


