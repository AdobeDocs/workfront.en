---
filename: custom-field-manager-issue-creator-on-issue-form
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
---



# Calculated custom field example: display the manager of an issue's creator on the issue custom form {#calculated-custom-field-example-display-the-manager-of-an-issues-creator-on-the-issue-custom-form}

Using a calculated custom field, you can display the name of the manager of an issue's creator on a custom form attached to the issue. Using the same statement, you can build similar calculated fields for projects, issues, and other objects. 


>[!TIP] {type="tip"}
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site. 




## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table class="TableStyle-TableStyle-HeaderRow" style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');caption-side: bottom;" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Any</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Access level configurations*</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Administrative access to Custom forms<br>For information about granting administrative access from the access level, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="text-align: left;"> <p><span class="bold">Object permissions</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Contribute access to the object where the form is attached with access to Edit the Custom Form</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Display the manager of an issue's creator on the issue custom form {#display-the-manager-of-an-issues-creator-on-the-issue-custom-form}

The following steps show how you can create a calculated field for an issue custom form where you can capture the name of the manager of the user who created the issue.&nbsp;The process is identical when you want to capture the name of the manager of a user who created a task, a project, a portfolio, for example. 



1.  Create an issue custom form and add a calculated field to it.


   For information about creating a custom form and adding calculated fields to it, see the following articles: 

    
    
    * [Create or edit a custom form](create-or-edit-a-custom-form.md) 
    *  [Add calculated data to a custom form](add-calculated-data-to-custom-form.md)
    
    

1.  Copy the following text mode code and paste it in the `Calculation` field of the custom form: 




   ```
   Owner.Manager.Name
   ```




   >[!TIP] {type="tip"}
   >
   >Custom field calculations are case sensitive. 



1.  Click `Done`, then `Save + Close`.


   The manager of the user who created the issue displays in the calculated field when the form that contains the field is attached to an issue. 



