---
filename: view-calculation-between-two-fields
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
---



# View: display the result of a calculation between two fields in a column {#view-display-the-result-of-a-calculation-between-two-fields-in-a-column}

You can use text mode in a column to display a calculation between two fields. 


For example, if you want to find out the number of week days that elapsed between two dates, you can use text mode syntax and data expressions to calculate this difference.  
For example, you can calculate the week day difference between the Planned Completion Date and the Actual Completion Date of a task and display the result in a column. 


You can use any other two dates in this calculation (Actual Start, Actual Completion, Projected Start, Projected Completion, etc).  
For more information about calculated data expressions, see [Calculated data expressions](calculated-data-expressions.md).



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


## Display the result of a calculation between two fields in a column {#display-the-result-of-a-calculation-between-two-fields-in-a-column}

To add this column to a task view:



1. Go to a list of tasks.
1. From the `View` drop-down menu, click `New View`.

1. Click `Add Column`, then `Switch to Text Mode`.

1. Hover over the text mode area, and click `Click to edit text`.
1.  Remove the text you find in the `Text Mode` box, and replace it with the following code:
   `<pre>displayname=Week Day Difference<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>` 

1. (Optional) To aggregate the values displayed in the view in a grouping, follow the steps described in [Grouping: display the result of aggregating multiple calculated values in a grouping](grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Click `Save`, then `Save View`.



  

