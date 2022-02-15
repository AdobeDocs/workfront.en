---
filename: example-status-timestamp-in-calculated-field
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
---



# Calculated custom field example: display a Status timestamp in a Custom Form {#calculated-custom-field-example-display-a-status-timestamp-in-a-custom-form}

The following calculated field displays the date when the object status is marked as In Progress (INP.) You can use the same information for calculated custom fields for issues, tasks, or projects. 


>[!NOTE]
>
>If the status of the object changes to INP, then it changes to another status, then back to INP, *`Adobe Workfront`* captures only the timestamp of the first change to INP. 




## Access requirements {#access-requirements}

You must have the following:

<table class="TableStyle-TableStyle-HeaderRow" style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');caption-side: bottom;" cellspacing="15"> 
 <caption style="text-align: left;"> 
  <p>*To find out what plan, license type, or access you have, contact your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>.</p> 
 </caption> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 300px;"> 
 </col> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Any</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Access level configurations*</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Edit access to Create Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="text-align: left;"> <p><span class="bold">Object permissions</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Manage permissions on the object where the form is attached</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.<br>For more information on permissions for dashboards, see <a href="permissions-reports-dashboards-calendars.md" class="MCXref xref">Share reports, dashboards, and calendars in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Prerequisites {#prerequisites}

To add a calculated field that displays a field's edit history to a custom form, you must first:



*  Create the custom form 




## Display a Status timestamp in a Custom Form {#display-a-status-timestamp-in-a-custom-form}




1. Go to a custom form where you want to add the field.
1. Click `Calculated` to add a calculated custom field to the form.  

1. Specify a `Label` for the Custom Field, for example: *Status Timestamp Custom Field*.

1. (Optional) Click the `Name` field to update it. The Name of the field matches the Label you just entered by default. 
1. Click  `Done`. 
1. Click `Save+Close`.
1. Re-open the Custom Form, and click the new Status Timestamp Custom Field on the form.
1.  In the `Calculation` field, specify the following calculation for your Custom Field:  
   `<pre>IF(Status='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})</pre>`

   >[!NOTE]
   >
   >This calculation is identical for all objects and for all statuses. You must always use the three-letter key, and not the status name for the object status in this calculation.  
   >For more information about the keys for Statuses, see [Create or edit a status](create-or-edit-a-status.md).



1.  Click `Save+Close`.  
   You can then report on the Status Timestamp Custom Field, or use it in other calculations in reports or Custom Fields.  



