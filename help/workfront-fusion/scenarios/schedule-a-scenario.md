---
filename: schedule-a-scenario
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
---



# Schedule a scenario {#schedule-a-scenario}

By default, a scenario runs every 15 minutes. You can change this by defining when and how often an activated scenario runs. 


## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Schedule a scenario {#schedule-a-scenario-1}




1.  In the upper-right corner of the Scenario detail page, click `Options` > `Scheduling`


   Or


   Click the `Scheduling`icon (clock) on the scenario's trigger module.

1.  Enter information into the following fields:

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Run scenario</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the frequency at which you want to run the scenario, then select the interval.</p> 
    <ul> 
     <li> <p><span class="bold">At regular intervals</span> </p> <p>Enter the number of minutes between executions. The default value is 15 minutes.</p> </li> 
     <li> <p><span class="bold">Once</span> </p> <p>Enter the date and time that you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</p> </li> 
     <li> <p><span class="bold">Every day</span> </p> <p>Enter the time at which you want the scenario to run. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code>.</p> </li> 
     <li> <p><span class="bold">Days of the week</span> </p> <p>Days: Select the days of the week that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
     <li> <p><span class="bold">Days of the month</span> </p> <p>Days: Select the days of the month that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
     <li> <p><span class="bold">Specified dates</span> </p> <p>Months: Select the months that you want to run the scenario. You can select one or more months.</p> <p>Days: Select the days of the month that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
    </ul> <p>Note: A date must exist for a scenario to run on that date. For example, a scenario scheduled for only the 31st of the month will not run in February, April, June, September, or November, because those months do not have a 31st day.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Advanced scheduling</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">You can define specific time intervals during which your scenario is to run. You can specify time-of-day intervals, weekdays or months. For each interval, click <span class="bold">Add </span>and fill in the fields as described in the Run scenario field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Start</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Enter the date and time after which you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">End</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">Enter the date and time before which you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</td> 
  </tr> 
 </tbody> 
</table>


1. Click `OK` to save the schedule settings and return to the scenario.


