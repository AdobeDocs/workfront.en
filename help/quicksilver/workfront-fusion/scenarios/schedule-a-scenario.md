---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Schedule a scenario in Adobe Workfront Fusion
description: By default, a scenario runs every 15 minutes. You can change this by defining when and how often an activated scenario runs.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
---
# Schedule a scenario in [!DNL Adobe Workfront Fusion]

By default, a scenario runs every 15 minutes. You can change this by defining when and how often an activated scenario runs.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
  <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Schedule a scenario

1. In the upper-right corner of the Scenario detail page, click **[!UICONTROL Options]** > **[!UICONTROL Scheduling]**

   Or

   Click the **[!UICONTROL Scheduling]** icon (clock) on the scenario's trigger module.

1. Enter information into the following fields:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Run scenario]</td> 
      <td> <p>Select the frequency at which you want to run the scenario, then select the interval.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL At regular intervals]</strong> </p> <p>Enter the number of minutes between executions. The default value is 15 minutes.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>Enter the date and time that you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Every day]</strong> </p> <p>Enter the time at which you want the scenario to run. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Days of the week]</strong> </p> <p>Days: Select the days of the week that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the month]</strong> </p> <p>Days: Select the days of the month that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Specified dates]</strong> </p> <p>Months: Select the months that you want to run the scenario. You can select one or more months.</p> <p>Days: Select the days of the month that you want the scenario to run. You can select one or more days.</p> <p>Time: Enter the time that you want the scenario to run on the selected days. Use the format <code>h:mm A</code>. Example: <code>11:00 PM</code></p> </li> 
       </ul> <p>Note: A date must exist for a scenario to run on that date. For example, a scenario scheduled for only the 31st of the month will not run in February, April, June, September, or November, because those months do not have a 31st day.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>You can define specific time intervals during which your scenario is to run. You can specify time-of-day intervals, weekdays or months. For each interval, click <strong>[!UICONTROL Add]</strong> and fill in the fields as described in the [!UICONTROL Run scenario] field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Enter the date and time after which you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Enter the date and time before which you want the scenario to run. Use the format <code>MM/DD/YYYY h:mm A</code>. Example: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL OK]** to save the schedule settings and return to the scenario.
