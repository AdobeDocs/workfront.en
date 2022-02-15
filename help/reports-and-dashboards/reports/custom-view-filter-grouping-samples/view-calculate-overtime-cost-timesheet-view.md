---
filename: view-calculate-overtime-cost-timesheet-view
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
---



# View: calculate overtime cost in a Timesheet View {#view-calculate-overtime-cost-in-a-timesheet-view}

Overtime is not calculated by default in *`Adobe Workfront`*, but you can create a Timesheet report that calculates overtime.


If the user is associated with a Cost per Hour rate in their profile, you can also calculate the amount of cost for the overtime of that user.  
For information about associating users with Cost per Hour rates, see the article [Configure My Settings](configure-my-settings.md).


>[!NOTE]
>
>The Overtime field that you can add to a Timesheet view in a list or a report displays the information found in the Overtime field of the timesheet. This information is updated manually by a user with access to modify the timesheet. For more information about the Overtime field in a timesheet, see the article [Understand the Timesheet layout](timesheet-layout.md).





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


## Calculate overtime cost in a Timesheet View {#calculate-overtime-cost-in-a-timesheet-view}

To add a calculated Overtime column to a timesheet view:



1.  Go to a list of timesheets, or create a Timesheet Report.


   For information about creating reports, see the article [Create a custom report](create-custom-report.md).

1.  Click `Customize View` in a list of timesheets.


   Or


   Select the `Columns (View)` tab in a Timesheet report.

1.  Click `Add Column`.
1.  Click `Switch to Text Mode`.
1.  In the `Show in this column` area, click `Click to edit text`.
1.  Copy and paste the following text mode code in the `Text mode` dialog box.
   `<pre>displayname=Calculated Overtime Cost<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>` 

   >[!NOTE]
   >
   >This calculation assumes that the user usually works a 40-hour week.



1.  Click `Save`, then name the new view and click `Save View` in a list of timesheets.


   Or


   Click `Save + Close` in a Timesheet report.

1.  (Optional and conditional) if you are building a Timesheet report, specify a name for the report, then click `Save Report`.


   The cost of the overtime of each user is displayed in the `Calculated Overtime Cost` column.

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)




