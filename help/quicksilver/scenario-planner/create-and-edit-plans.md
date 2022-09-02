---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Create and edit plans in the Scenario Planner
description: You can create plans as part of using the Workfront Scenario Planner, when prioritizing your company's higher-level strategy. For more information about plans, see Plans overview in the Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
---
# Create and edit plans in the Scenario Planner

You can create plans as part of using the Workfront Scenario Planner, when prioritizing your company's higher-level strategy. For more information about plans, see [Plans overview in the Scenario Planner](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Business or higher</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product</td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Scenario Planner to access functionality described in this article.</p> <p>For information about obtaining the Workfront Scenario Planner, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access or higher to the Scenario Planner</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Manage permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create or edit plans

You can create a plan from scratch or you can edit an existing one that was shared with you.

>[!NOTE]
>
>After you create a plan, you are considered the plan creator and owner. When a user is deactivated, the plan has no owner and is not visible to anyone unless previously shared with a link.

This article describes how you can create a plan from scratch or you can edit an existing plan.

For all considerations about plans including the information available for a plan, see [Plans overview in the Scenario Planner](../scenario-planner/plans-overview.md).

For information about deleting plans, see [Delete plans in the Scenario Planner](../scenario-planner/delete-plans.md).

To create or edit a plan:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png), then click&nbsp;Scenarios.

   A list of existing plans that you created displays in the Workfront Scenario Planner. 

1. (Optional) Click the **Filter** icon ![](assets/filter-icon-34x37.png)in the upper-right corner of the plan list, and select from the following:

   | All |Displays all plans that you created or that have been shared with you.  |
   |---|---|
   | My plans |Displays plans that you created.  |
   | Shared with me |Displays plans shared with you.  |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Optional)&nbsp;Click the **Search** icon ![](assets/search-icon.png) to type a keyword and quickly locate a plan in the list. 

1. Click the name of an existing plan to edit it and continue with step 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   Or

   Click **New Plan** in the upper-left corner to create a plan and continue with step 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   The New Plan box displays.

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Conditional) When you create a new plan, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Type a name for the plan. This is a required field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Important: <span style="font-weight: normal;">You cannot modify the following selections after you create and save the plan.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE (Full Time Equivalent) or Hours</span> </td> 
      <td> <p><span>Select one of the following options to indicate how you want to estimate job role information for this plan:</span> </p> 
       <ul> 
        <li> <p><span><strong>FTE</strong>.&nbsp;This is the default </span> </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>
         --> <p>For all calculations in the Scenario Planner, Workfront uses the following value: 1 FTE = 8 Hours. </p> </li> 
        <li> <p><strong>Hours</strong> </p> </li> 
       </ul> <p>Important: <span>The option you select here determines how job role information displays for the plan, the plan's scenarios, and initiatives.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Start date</td> 
      <td> <p>Select the month and year when you want the plan to start. You can select only months in this field. Workfront assumes that the start date of the plan is the first day of the selected month and the end date is the last day of the end of month in its duration. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duration</td> 
      <td> <p>From the drop-down menu select from the following durations:</p> 
       <ul> 
        <li>1 year. This is the default duration. </li> 
        <li>3 years</li> 
        <li> <p>5 years</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditional) Click **Next**.

   The timeline of the plan displays as the **Initial scenario**.

   For information about creating additional scenarios, see [Create and compare plan scenarios in the Scenario Planner](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Optional) From the timeline drop-down menu select one of the options in the following table to change the way you view the timeline of the plan.

   ![](assets/month-dropdown-with-all-options.png)

   | Month |Displays the timeline by month. This is the default and only option for a one year plan.  |
   |---|---|
   | Quarter |Displays the timeline by quarter. This option is available only when the Duration of the plan is 3 or 5 years. This is the default option for a 3-year plan. |
   | Year |Displays the timeline by year. This option is available only when the Duration of the plan is 5 years. This is the default option for a 5-year plan.  |

1. (Optional) Scroll from left to right to view the entire duration of the plan. 
1. (Optional) Click the **Today** indicator line to return to the current day.

   ![](assets/today-indicator-350x160.png)

1. Click the **Job Roles** box in the header of the plan to add job roles that will be available to execute the plan.

   The details of the Job&nbsp;Roles box display.

   >[!TIP]
   >
   >The role allocation unit (FTE or hours) that&nbsp;Workfront uses for this plan displays in parentheses in the title of the box.

   ![](assets/adding-people-to-plan-350x206.png)

1. Click the **Start typing job role** field and select a role from the list or start typing the name of an active job role.

   All active job roles in the system are listed when you click this field.

   This adds the job role to the Job&nbsp;Roles column. 

1. Update or review the following information for the job role:&nbsp;

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Max available (for FTE) </p> <p role="rowheader">or </p> <p role="rowheader"><span>Total available (for hours)</span> </p> </td> 
      <td> <p><span>Depending on whether you selected to use hours or FTE for your plan, type</span> the number of job role FTEs <span>or hours</span> that are available to execute work on the plan in the following fields: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>Total available</strong> (for hours): Indicate the total number of hours for all months during the duration of the scenario. By default, Workfront divides the Total available number equally across all months in the duration of the scenario. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If you enter 1200 hours for a Designer, this means the Designer is available for 100 hours for each month during the duration of the plan, when the plan Duration is 1 year. </p> </li> 
        <li> <p><b>Max available</b> (for FTE): Indicate the number of FTEs that the job role is available for each month during the duration of the plan. By default, <strong>Workfront</strong> assigns the Max available number to each month in the duration of the scenario.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If you enter 1 FTE for a Consultant, this means the Consultant is available for 1 FTE for each month during the duration of the plan. </p> <p>You can enter a number lower than 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>A 0.5 Consultant job role would mean that a consultant would dedicate half of their FTE (typically, 4 hours, where 8 hours is 1 FTE) to working on this plan. For all calculations in the Scenario Planner, Workfront uses the following value: 1 FTE = 8 Hours. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Max required (for FTE)</p> <p role="rowheader">or </p> <p role="rowheader"><span>Total required (for hours)</span> </p> </td> 
      <td> <p><span>Depending on whether you selected to use hours or FTE for your plan, review</span> the number of job role FTEs <span>or hours</span> that are required to complete the initiatives in the scenario. Review the following fields:</p> 
       <ul> 
        <li> <p><strong>Total required</strong> (for hours): The total number of hours required for all months during the duration of the plan.</p> </li> 
        <li> <p><strong>Max required</strong> (for FTE): The maximum number of FTEs required for any of the months during the duration of the plan. </p> </li> 
       </ul> <p>Tip: The <span>maximum</span> number of FTEs <span>or the total number of hours</span> required for that job role displays after you start adding initiatives.&nbsp;For information about adding initiatives to a plan, see <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Create and edit initiatives in the Scenario Planner</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Avg utilization</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>Workfront calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> Workfront calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the Utilization value for each role also updates and Workfront calculates a utilization percentage for the plan. For information about how Workfront calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the Scenario Planner</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">Hourly rate</td> 
      <td> <p>This is the Cost Hour rate for the job role. The hourly rate displays in the currency of your system. For information about setting up Exchange Rates for your system, see <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Hover over the name of a job role or click tab after updating the role information, then click the **trash can icon** ![](assets/delete.png) to remove it from the plan. 
1. Click **Job role distribution**.

   The job role distribution panel displays for all months in the duration of the scenario.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Type the name of a job role to add it to the plan in the **Start typing job role field**, then click&nbsp;Enter when it appears on the list. This adds the job role to the Job&nbsp;Roles column. 
1. Update or review the following information for each month of the scenario: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Job&nbsp;Roles (FTE or Hours)</td> 
      <td>Both the job role available for the scenario and those required for the initiatives on the scenario display in the job role distribution panel. There is an indication whether job role estimations are in FTEs or hours in the column header. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Available (max &lt;number of FTEs&gt;) </p> 
       <div> 
        <p>or</p> 
        <p>Available (total &lt;number of hours&gt;) </p> 
       </div> </td> 
      <td> <p><span>Depending on whether you selected to use hours or FTE for your plan, review or update</span> the monthly number of job role FTEs <span>or hours</span> available for the scenario in the following fields:</p> 
       <ul> 
        <li> <p><strong>Available (max &lt;number of FTEs&gt;)</strong>:&nbsp;The number in parentheses displays the maximum number of roles available for any one of the months for the scenario. Review or update the number of FTEs for each month of the scenario. Changing the monthly allocation might update the number of FTEs in the parentheses. </p> </li> 
        <li> <p><span><strong>Available (total &lt;number of hours&gt;)</strong>:&nbsp;The number in parentheses displays the total number of hours available for all the months in the scenario. Review or update the number of hours for each month of the scenario. Changing the monthly allocation updates the number of hours in the parentheses.</span> </p> </li> 
       </ul> <p>Manually updating the monthly job role allocations is another way of resolving job role conflicts between initiatives on the scenario. </p> <p>Tip:   <p><span>To update the monthly role availability for several months, type the number of hours or FTEs in the Available field of any month, then drag the corner of the field over the adjacent months to copy the same value for each month. Drop it to update all months.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Required (max &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">or</p> 
        <p role="rowheader">Required (total &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>Depending on whether you selected to use hours or FTE for your plan, review</span> the monthly number of job role FTEs or hours required for the scenario in the following fields:&nbsp;</p> 
       <ul> 
        <li> <p><strong>Required (max &lt;number of FTEs&gt;)</strong>:&nbsp;The number in parentheses displays the maximum number of roles required for any one of the months for the scenario. </p> </li> 
        <li> <p><span><strong>Required (total &lt;number of hours&gt;)</strong>:&nbsp;The number in parentheses displays the total number of hours required for all the months in the scenario.</span> </p> </li> 
       </ul> <p>Tip: You cannot modify the Required number of FTEs <span>or hours</span> for the job role. This number populates for the scenario after you start adding initiatives and their job role requirements. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Difference</td> 
      <td> 
       <div> 
        <p>The monthly difference between the amounts of required and available job roles for the scenario. Workfront calculates the difference for each job role for each month using the following formula:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (in FTEs or hours) </p> 
        <p>Tip: When the difference displays a negative number, the scenario requires more job roles than the plan has available. Your resources are overallocated. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utilization %</td> 
      <td> 
       <div> 
        <p>The percentage of utilization displays how many of the job roles available are actually used (or required) on the initiatives in the scenario. </p> 
        <p>Workfront calculates the utilization per job role per month using the following formula: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>The utilization percentage might display in the following colors, depending on the allocation of your resources:</p> 
        <ul> 
         <li> <p><b>Green</b>: The available and required numbers of job roles match. The resources are fully allocated and the utilization percentage is 100%. </p> </li> 
         <li> <p><b>Red</b>: There are more required job roles than the plan has available. The resources are overallocated and the utilization percentage is higher than 100%.</p> </li> 
         <li> <p><b>Blue</b>: There are more available job roles than they are required. The resources are underallocated and the utilization percentage is lower than 100%. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click&nbsp;**Apply** to save the monthly job role distribution

   Or

   Click **Cancel** to close the job role distribution list and return to the scenario. 

1. Click the **Financial** box in the header of the plan, to add the budget for this plan.

   The details of the Financial box display.

   >[!TIP]
   >
   >The currency that&nbsp;Workfront uses for this plan displays in parentheses in the title of the box.

1. Specify the **Yearly budget**.

   >[!NOTE]
   >
   >If your plan spans multiple years, you must specify a budget amount for each year.

1. Press Enter to save the yearly budget, then Tab to move to the following year.

   The yearly budget is automatically distributed equally for each month of the selected year. 

1. Click **Advanced** to see the monthly budget distribution. The yearly and monthly budgets are always rounded numbers. When the budget amount cannot be distributed equally to all the months within a year because of decimals a **Remaining** indicator displays under the yearly budget distribution.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Manually adjust the monthly budgets to eliminate the exceeding amounts.

   When the total of all monthly budget amounts is larger than the yearly budget, an **Exceeding** warning indicator displays under the yearly budget distribution. Manually adjust the monthly budget amounts until they are equal or lower to the available budget for the plan.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Disable the **Include people costs** setting to exclude costs associated with job roles from counting towards the overall cost of the plan. Fixed Costs are always counting towards the overall cost of the plan. This setting is enabled by default and affects all scenarios on the plan. 
1. Click anywhere outside the Financial box to close it. The information you entered is automatically saved.

   You can now start creating the initiatives on the plan, and adding scenarios. 

1. (Recommended) Click **New initiative** to add a new initiative.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   For information about adding initiatives, see the article [Create and edit initiatives in the Scenario Planner](../scenario-planner/create-and-edit-initiatives.md).

1. (Optional) Make a copy of the existing scenario to create a new scenario of the same plan. For more information about creating and working with multiple scenarios, see [Create and compare plan scenarios in the Scenario Planner](../scenario-planner/create-and-compare-scenarios-for-a-plan.md). 
1. Click **Save Plan**.

   Your plan is created or updated.

1. (Optional) Click the **Favorites icon** ![](assets/favorites-icon-small.png) to the right of the plan name to add the plan to your list of Favorites. 

1. (Optional) Copy the URL of the plan and send it to any other user that might need to review or update it. They must have at least View access in their access level to be able to view the plan. They must have Edit access to edit it. If they must review financial information on the plan, like budgets, costs, and job role rates information, they must also have access to Financial Data in their Access level. For information about the access needed for the Scenario Planner, see [Access needed to use the Scenario Planner](../scenario-planner/access-needed-to-use-sp.md).
