---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Initiatives overview in the Scenario Planner
description: The Scenario Planner is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see The Scenario Planner overview.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
---
# Initiatives overview in the [!DNL Scenario Planner]

As a business manager, you can create initiatives for plans in the [!DNL Adobe Workfront Scenario Planner]. For information about creating plans, see the article [Create and edit plans in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Initiatives overview

Using the [!DNL Workfront Scenario Planner], you can estimate and review the following information for each initiative:

* Estimate the kind and number of job roles that might be required to complete the initiative. This adds to the Required job role count for the plan as well as calculates the People Costs that you can review for an initiative. 
* Estimate the Fixed Costs associated with the work needed to complete the initiative.
* Estimate the Planned Benefit that your company might gain when the initiative is completed.

To view information about your initiatives, you can access individual initiatives within a plan. For information about creating and accessing initiatives, see the article [Create and edit initiatives in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Considerations about initiatives

Consider the following when creating initiatives:

* You must create a plan before you can create an initiative. 
* You can create initiatives from scratch or you can import projects into a plan. The projects become initiatives within the plan.

  For information about creating initiative from scratch, see [Create and edit initiatives in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  For information about importing projects into a plan to create initiatives from projects, see [Import projects to plans in the [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md). 

* Initiatives are smaller planning units than plans and they are created only as part of a plan.
* The shortest initiative can have a duration of 1 month. The longest initiative can have a duration of 5 years. 
* You cannot do actual work on an initiative. At the initiative level, you can define what resources are needed and what cost those resources will incur so you can start executing one of the demands of the plan. For example, if your company has a plan to expand and acquire a new office in a new location, your department might have an initiative to install the network infrastructure for that new location. 
* You can create multiple initiatives in a plan. With each initiative, you can outline a high-level strategy to accomplish the work in your department. 
* You can prioritize initiatives within a plan, to ensure that the most important initiative receives the most budget and the most resources. 
* When you create initiatives within a plan everyone that views that plan can also view all the initiatives within the plan.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* You can publish initiatives to create projects or to update the projects that are linked to them. For information about publishing initiatives, see [Update or create projects by publishing initiatives in the [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Financial information about initiatives

You can review financial information about individual initiatives to understand how the initiatives fit within the plan. For information about accessing an initiative, see the article [Create and edit initiatives in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

You can view the following financial indicators about an initiative by accessing it within a plan:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs total amount]</td> 
   <td> <p style="font-weight: normal;">This is a calculation of the total cost of an initiative. </p> <p style="font-weight: normal;">[!DNL Workfront] calculates the total Costs value of an initiative using this formula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fixed Costs]</td> 
   <td> <p><span style="font-weight: normal;">This is a manual entry where you can estimate <span>a monthly amount of Fixed Costs for each month of the initiative.</span> This does not include the costs associated with the roles added to the initiative which are captured in the [!UICONTROL People Cost] field.</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costs]</td> 
   <td> <p style="font-weight: normal;">This is a total calculation of the costs associated with the job roles of the initiative for the duration of the initiative. This number depends on how many FTEs or hours you estimate for a job role for each month of the initiative. </p> 
     <p><b>TIPS</b>  
     <ul> 
      <li> <p>The number of monthly FTEs for the same job role may be different from month to month.</p> </li> 
      <li> <p>[!DNL Workfront] considers that there are 160 working hours in one month. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calculates the [!UICONTROL People Costs] of an initiative using the following formula:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calculates the Monthly People Costs for each month during the Initiative's duration using the following formula:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EXAMPLE</b></p>
      <p>If you have an initiative with a duration of 6 months that requires 1 Designer with a $50 hourly rate for 1 FTE every month and a Web Designer with an hourly rate of $100 for 2 months of the initiative, the People Costs of the initiative is calculated as follows:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>This is a manual entry where you can estimate the overall benefit that your department would gain by completing this initiative. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value amount]</td> 
   <td> <p style="font-weight: normal;">This represents the value of your initiative when taking into account the overall costs and the Planned Benefit estimated on the initiative. [!DNL Workfront] calculates the Net Value of an initiative using the following formula:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->
      
## Initiative information in reports

You can display initiative information in reports, as described in the table below. This information is available in your Workfront instance only when your company has purchased a Workfront Scenario Planner license.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Report type</b></td> 
   <td><b>Initiative information</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Name, Duration, Start and End Dates, Entered by, ID, Last Published Date*, All Project fields including custom fields*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>All Initiative information as listed above, (Job Role) ID, Project*, Project Assignment Planned Hours*, Initiative Job Role Hours, (Job Role) Count, All Project fields including custom fields*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>All Initiative information as listed above*</p> </td> 
  </tr> 
 </tbody> 
</table>

*These fields populate with information from the project linked to the initiative, only when the initiative was created from a project or was published to a project at least once. For information about publishing initiatives, see [Update or create projects by publishing initiatives in the [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
