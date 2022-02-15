---
filename: report-budgeted-hour
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
---




# Report: Budgeted Hour {#report-budgeted-hour}

When you want to share Budgeted Hour information with other users who do not have access to the Resource Planner, you can do so by building a Budgeted Hour report. You can then share the report with them.


>[!IMPORTANT] {type="important"}
>
>Budgeted Hours are updated every hour in the `Workfront` database. Refreshing the report does not necessarily refresh the hour information in it. You can view the time lapsed since the last update in the upper-right corner of every Budgeted Hour report. Refreshing the report refreshes the information in it only when there has been more than one hour since the last update. 
>
>
>![](assets/budgeted-hour-report-time-sync-warning-600x127.png)>
>






##  Build a Budgeted Hour report {#build-a-budgeted-hour-report}




1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <b>Main Menu</b>  <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp; <b>Reports</b>. </MadCap:conditionalText>` 
1.  Click&nbsp;**New Report> Budgeted Hour**.


   The default view is applied to the report.

1.  (Optional) To make the report easier to read, click the **Budgeted Hours** column, then **Switch to Text Mode**, then change the 

   ```
   valuefield
   ```

   line to 

   ```
   valueexpreesion
   ```

   and enter the rounding expression. This rounds the number of Budgeted Hours to a number of decimals that you specify.


   For information about how to round a number in `Workfront`, see the article [Calculated data expressions](calculated-data-expressions.md).

1. (Optional)&nbsp;Click **Add Column** to add additional columns. 
1.  (Optional) To make the report easier to read, we recommend that you add a grouping to it. We suggest the following grouping: 


   Click the **Groupings** tab, then do one or several of the following:

    
    
    1. Click&nbsp;**Add Grouping** and start typing "Project&nbsp;Name", then select it when it appears in the list.
    1. Click **Add Grouping** and start typing "Job&nbsp;Role Name", then select it when it appears in the list.
    1.  Click **Add Grouping** and start typing **Allocation Date**, select it when it appears in the list, and then select the timeframe you want to group by from the **Group Dates by** field. 
    
    

1. (Optional) Click&nbsp;**Filters** to add filters to the report.
1. (Optional)&nbsp;Click&nbsp;**Chart** to add a chart to the report.
1. Click&nbsp;**Save +&nbsp;Close**. 




## Review the Budgeted Hour report {#review-the-budgeted-hour-report}

The following information is available in the Budgeted Hour report by default:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Project </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This is the name of the project associated with the Budgeted Hour. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"> <p>Job&nbsp;Role</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">This is the name of the job role associated with the Budgeted Hour. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">User</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This is the name of the user associated with the Budgeted Hour. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Alloc. Date</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This is the Allocation Date. It is the first day (a Sunday) of the week for which you budgeted the hours. </p> 
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span> 
     <p>If a week spans for two months, this generates two rows in the report: one corresponding to the first day of the week (the Sunday of the week which is during the first month), and a second one corresponding with the first day of the second month (and which could be any day of the week.) </p> 
     <p>For example, if you budget 8 hours for a user for the week of June 30 (Sunday) - July 6 (Saturday), the two rows show an Allocation Date of June 30, and July 1. </p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Bud. Hours</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">These are the Budgeted Hours allocated to the User in the Resource Planner. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Pln. Bud. Hours</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">These are the Budgeted Hours allocated to the Job&nbsp;Role or the Project in the Resource Planner. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

