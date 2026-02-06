---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Calculate Overtime Cost in a Timesheet View'
description: Overtime is not calculated by default in Adobe Workfront, but you can create a Timesheet report that calculates overtime.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
---
# View: calculate overtime cost in a Timesheet View

<!--Audited: 11/2024-->

Overtime is not calculated by default in Adobe Workfront, but you can create a Timesheet report that calculates overtime.

If the user is associated with a Cost per Hour rate in their profile, you can also calculate the amount of cost for the overtime of that user.  
For information about associating users with Cost per Hour rates, see the article [Configure My Settings](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>The Overtime field that you can add to a Timesheet view in a list or a report displays the information found in the Overtime field of the timesheet. This information is updated manually by a user with access to modify the timesheet. For more information about the Overtime field in a timesheet, see the article [Timesheet layout overview](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Calculate overtime cost in a Timesheet View

To add a calculated Overtime column to a timesheet view:

1. Go to a list of timesheets.

1. Click the **View** drop-down menu, then click **New View**.

1. Click **Add Column**.
1. Click **Switch to Text Mode**, then click **Edit Text Mode**.
1. In the **Edit Text Mode** box, remove the text in the box, then copy and paste the following text mode code:

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >This calculation assumes that the user usually works a 40-hour week.

1. Click **Done**, then name the new view and click **Save View** in a list of timesheets.

   The cost of the overtime of each user is displayed in the **Calculated Overtime Cost** column.

   
