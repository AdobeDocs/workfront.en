---
filename: schedule-a-scenario
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Schedule a scenario
description: By default, a scenario runs every 15 minutes. You can change this by defining when and how often an activated scenario runs.
---

# Schedule a scenario

By default, a scenario runs every 15 minutes. You can change this by defining when and how often an activated scenario runs.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Schedule a scenario

1. In the upper-right corner of the Scenario detail page, click `Options` > `Scheduling`

   Or

   Click the `Scheduling`icon (clock) on the scenario's trigger module.

1. Enter information into the following fields:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Run scenario</td> 
      <td> <p>Select the frequency at which you want to run the scenario, then select the interval.</p> 
       <ul> 
        <li> <p><span class="bold">At regular intervals</span> </p> <p>Enter the number of minutes between executions. The default value is 15 minutes.</p> </li> 
        <li> <p><span class="bold">Once</span> </p> <p>Enter the date and time that you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><span class="bold">Every day</span> </p> <p>Enter the time at which you want the scenario to run. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code>.</p> </li> 
        <li> <p><span class="bold">Days of the week</span> </p> <p>Days: Select the days of the week that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
        <li> <p><span class="bold">Days of the month</span> </p> <p>Days: Select the days of the month that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
        <li> <p><span class="bold">Specified dates</span> </p> <p>Months: Select the months that you want to run the scenario. You can select one or more months.</p> <p>Days: Select the days of the month that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
       </ul> <p>Note: A date must exist for a scenario to run on that date. For example, a scenario scheduled for only the 31st of the month will not run in February, April, June, September, or November, because those months do not have a 31st day.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Advanced scheduling</td> 
      <td>You can define specific time intervals during which your scenario is to run. You can specify time-of-day intervals, weekdays or months. For each interval, click <span class="bold">Add </span>and fill in the fields as described in the Run scenario field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Start</td> 
      <td>Enter the date and time after which you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">End</td> 
      <td>Enter the date and time before which you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click `OK` to save the schedule settings and return to the scenario.

