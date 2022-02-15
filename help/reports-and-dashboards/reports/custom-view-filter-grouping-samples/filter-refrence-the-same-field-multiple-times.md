---
filename: filter-refrence-the-same-field-multiple-times
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
---



# Filter: create multiple filter rules that reference the same field ("AND" statements) {#filter-create-multiple-filter-rules-that-reference-the-same-field-and-statements}

In the standard mode interface, when attempting to create multiple filters that reference the same field (using the AND qualifier), one of the filters is deleted when you save the report and exit the report builder.

` `**Example: **`` You might want to view only tasks that contain the word "green" but do not contain the word "red" in the name. *`Adobe Workfront`* does not allow you to save the following filter rules using the standard mode interface because it references the same field (Task&nbsp;Name) but uses different modifiers and refers to different values:



*  Task Name > Contains > Green
*  Task Name > Does Not Contain > Red


However, you can create this filter using text mode. 



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.
&nbsp;


## Create multiple filter rules that reference the same field {#create-multiple-filter-rules-that-reference-the-same-field}




1. Go to a list of tasks.
1. From the `Filter`drop-down menu, select `New Filter`.

1. Click `Switch to Text Mode`.
1. Hover over the text mode area, and click `Click to edit text`.
1.  In the Set Filter Rules for your Report area, add the following code: 
   `<pre>name=green<br>name_Mod=cicontains<br>AND:1:name=red<br>AND:1:name_Mod=cinotcontains</pre>` 
   ` `**Tips: **`` To build similar filters, build the first statement first.&nbsp;For example: 




   ```
   name=green<br>name_Mod=cicontains
   ```




   Copy and paste the statement as many times as needed. You can then add as many statements as you need to reference the same field (in our case "name") and make the following modifications to the additional statements: 

    
    
    1.  Precede the two copied lines with "AND:1:", "AND:2:", "AND:3:", etc for each new field possible value. 
    1.  Replace the field line with the new field value (after the "=" sign). 
    1.  Replace the modifier line (_Mod) with the new modifier. 
    
    
   These statements are case-sensitive.   


1. Click `Done`, then `Save Filter`.



