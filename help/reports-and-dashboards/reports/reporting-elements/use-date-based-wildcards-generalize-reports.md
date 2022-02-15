---
filename: use-date-based-wildcards-generalize-reports
product-area: reporting
navigation-topic: reporting-elements
---



# Use date-based wildcards to generalize reports {#use-date-based-wildcards-to-generalize-reports}

You can generalize a report by using wildcards instead of specific information when building certain reporting elements. 


For example, if you want to create a report that shows the tasks that have a specific Planned Start Date, you can use the calendar date picker in a filter to select a specific date. However, if you want to create a report that shows tasks that have the Planned Start Date within a certain timeframe from the date when the report is accessed, you can use a wildcard that indicates that when someone views the report it displays information for a timeframe relevant for the moment when they view the report. 


For example in the past week, in the past year, in the next two weeks, etc. This way, you build the report once, but because you use a wildcard in the filter, it produces different results every time someone reads it because it adapts to the day when they run the report.


You can use date-based wildcards when building the following reporting elements:



* Filters
* Custom prompts
* Views when adding rules for columns





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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit reporting elements in a report</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a report to edit reporting elements in a report</p> <p>Manage permissions to a view or filter to edit them</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

You must create a report before you can add wildcard variables to it.


For information on creating a report, see [Create a report](create-report.md).


## Walk-through {#walk-through}

View the following video to learn how you can generalize the information in your reports and adapt them to the date when they are run by using date-based wildcards.


This video was recorded in *`Adobe Workfront`* Classic. However, the content also applies to the new Workfront experience.


[ ![](assets/video-date-based-wildcards-350x198.png)](https://workfront-video.wistia.com/medias/poww2vz0r4) 


## How-to steps {#how-to-steps}

To insert a date-based wildcard in a report:



1. Go to a report for which you want to insert a date-based wildcard.
1. Click `Report Actions`, then `Edit`.

1. Click the `Filters` tab.
1. Click `Add a Filter Rule`.
1.  Start typing the name of the field that you want to filter by.  
   You must type fields that reference a date.
1.  Select `Equal` in the drop-down menu for the filter variable.


   >[!TIP] {type="tip"}
   >
   >You must always select the `Equal` filter variable when working with wildcards in *`Adobe Workfront`*.



1.  In the `Start typing name ...` box, type: 

   ```
   $$TODAY
   ```

   if you want to display information about something that occurs the same day that the report is run.


   Or


   Type 

   ```
   $$NOW
   ```

   if you want to display information about something that occurs at the same date and time that the report is run.


   This date is always different, as it changes with the date the report is actually viewed by a user. so the information in the report is different from day to day.

1.  (Optional) If you want to display information that occurs within a timeframe after the date when the report is run, type

   ```
   $$TODAY+1w
   ```

   to display information in the following week, or 

   ```
   $$TODAY+2m
   ```

   to display information in the next two months. You can also indicate timeframes for quarters, hours, days, or years.
1.  (Optional) If you want to display information about something that occurred within a timeframe before the date when the report is run, type $$TODAY-1w to display information from the previous week, or 

   ```
   $$TODAY-2m
   ```

   to display information from the previous two months. You can also indicate timeframes for quarters, hours, days, or years.


   For a complete list of attributes, qualifiers, and operators that you can use in date-based wildcards, see the article [Wildcard filter variables](understand-wildcard-filter-variables.md).


   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)



1. Click `Save + Close`.




## Additional information {#additional-information}

See also:



*  [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) 
* [Wildcard filter variables](understand-wildcard-filter-variables.md) 
* [Create or edit filters in Adobe Workfront](create-filters.md) 
* [Add a prompt to a report](add-prompt-report.md) 
* [Use conditional formatting in Views](use-conditional-formatting-views.md) 


