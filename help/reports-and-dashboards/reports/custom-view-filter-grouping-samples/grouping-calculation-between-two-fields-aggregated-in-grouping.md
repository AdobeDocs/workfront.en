---
filename: grouping-calculation-between-two-fields-aggregated-in-grouping
content-type: reference
product-area: reporting;projects
keywords: calculated,aggregates,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
---



# Grouping: display the result of aggregating multiple calculated values in a grouping {#grouping-display-the-result-of-aggregating-multiple-calculated-values-in-a-grouping}

You can use text mode in a column to display a calculation between two fields in the view of a report or list. Each line displays the calculation for each object in the report or list. 


For example, you can display the difference between&nbsp;Actual Hours and Planned Hours in a third column called Work Balance for each task in a task report. For more information about calculated data expressions, see [Calculated data expressions](calculated-data-expressions.md).


You can display the aggregated value of multiple calculated view items in the same column in a grouping by adding a calculation to the 

```
aggregator.
```

line of the column that contains the calculated value. For example, you can aggregate (display the sum of) the amount of Work Balance hours of all the tasks in the grouping of the report or the list for the Work Balance column. This article describes how to do this.



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


## Display the result of aggregating multiple calculated values in a grouping {#display-the-result-of-aggregating-multiple-calculated-values-in-a-grouping}




1.  Go to a task report, click `Report Actions` >  `Edit`.
1. In the `Groupings` tab, click `Add Grouping`, and start typing `Project Name` in the `Group your Report` > `First by` field, then select it when it displays in the list. 

1.  In the `Columns(View)` tab, click `Add Column`, then start typing `Planned Hours` in the `Show in this column` field, then select it when it displays in the list.


   >[!TIP] {type="tip"}
   >
   >Always start adding as much information using the Standard interface before you edit information in text mode. Add fields that are closest to or contain the most amount of information that for the calculation you are trying to make. 



1. In the `Summarize this column by` field, select `Sum`, then click `Done`.

1. Click `Switch to Text Mode` in the column you added. 
1. Hover over the text mode area, and click `Click to edit text`.
1.  Replace the 

   ```
   valuefield.
   ```

   and the 

   ```
   aggregator.valuefield.
   ```

   lines with the lines highlighted in the following text mode example: 
   `<pre>valueformat=compound<br>aggregator.displayformat=minutesAsHoursString<br><span style="font-weight: normal;">aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)</span><br>aggregator.function=SUM<br>aggregator.valueformat=val<br>aggregator.namekey=workrequired<br>linkedname=direct<br>textmode=true<br>valuefield=workRequired<br>namekey=workrequired<br>valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours")viewalias=workrequired<br>displayname=Work Balance<br><br></pre>` 
   ` `**Tip: **`` In order to get the aggregated value in the grouping to display the aggregated difference between the Planned Hours and Actual Hours fields, input the same equation into the 

   ```
   aggregator.valuefield
   ```

   line. The 

   ```
   aggregator.displayformat
   ```

   used for the Planned Hours column converts minutes to hours. Because the Planned Hours field was used as a placeholder, this line doesn’t need to be adjusted.


   The 

   ```
   minutesAsHoursString
   ```

   definition of the 

   ```
   aggregator.displayformat
   ```

   line means there is no need to divide each field by 60 as done on the 

   ```
   valueexpression
   ```

   for the results. In this 

   ```
   aggregator.valuefield=workRequired
   ```

   becomes: 

   ```
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2
   ```

   . 

1. Click `Save+Close`.


&nbsp;



