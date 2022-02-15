---
filename: calculate-costs-resource-planner
product-area: resource-management
navigation-topic: resource-planning
---



# Calculate costs in the *`Resource Planner`*  {#calculate-costs-in-the-resource-planner}

You can budget your resources in the *`Resource Planner`* by using Cost values, instead of Hours or FTE values. Cost values are not available for the `View by User` view in the *`Resource Planner`*. 


>[!IMPORTANT] {type="important"}
>
>You must associate users and job roles with Cost per Hour rates in order to display Cost information in the *`Resource Planner`*.  
>For more information about associating Cost per Hour rates with job roles, see [Create and manage job roles](create-manage-job-roles.md).  
>For more information about associating Cost per Hour rates with users, see [Edit a user's profile](edit-a-users-profile.md).




Before budgeting your resources, ensure you have a good understanding of what work needs to be done (Planned Hours, FTE, or Cost) and what time your users are open to work (Available Hours, FTE, or Cost).  
For more information about understanding the information in the *`Resource Planner`* when budgeting by Hours or FTE, see [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](overview-of-planner-hour-fte-cost-information-in-role-project-views.md).


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> and higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Resource Management that includes access to&nbsp;Edit priorities and budget hours in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span></p> <p>Edit access to Financial Data, Projects, and Users</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the projects you want to budget information for with ability to Manage Finances</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Display information in the *`Resource Planner`* by Cost {#display-information-in-the-resource-planner-by-cost}

By default, the availability and allocation information is displayed in Hours in the *`Resource Planner`*. 


To display Available, Planned, and Budgeted information by Cost in the *`Resource Planner`*:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Resourcing</span>.</MadCap:conditionalText>` 
1. Go to the . 
1. (Conditional) Select `View by Project` or `View by Role`.  
   By default `View by Project` is selected.  
   The allocation and availability information displays in Hours.

1.  From the `Hours` drop-down menu, select `Cost`.


   If you do not have access to Financial Data in your access level, this option is not available.  
   If projects have a different currency than the system currency the Cost for these projects displays in the *`Resource Planner`* converted in the currency of the system. Your system administrator defines the system currency.  
   For more information about setting up the system currency in *`Workfront`* and conversion rates, see [Set up exchange rates](set-up-exchange-rates.md).  
   ![costs_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)







## Calculate Available Cost in the *`Resource Planner`* {#calculate-available-cost-in-the-resource-planner}

To display Available Cost values in the *`Resource Planner`* you must have the following:



* Cost per Hour rates for the users and roles
* Information about user availability.  
  Obtaining information about user availability depends on how your *`Workfront administrator`* configures your Resource Management Preferences.  
  For more information about calculating user availability and setting Resource Management Preferences, see [Configure Resource Management preferences](configure-resource-mgmt-preferences.md).



The following table illustrates how Available Cost is calculated in the *`Resource Planner`*: 

<table style="width: 567px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 232px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 768px;"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Available Cost</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Calculation</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">User Available Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The Available Cost per user is calculated using the following formula:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p>Note:  If the user does not have a Cost per Hour rate in their profile, the Cost per Hour rate of the job role under which they are listed is used in the calculation. If the user has no role associated with them, the Available User Cost is $0. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Role Available Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The Available Cost per role is calculated using the following formula:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p>Note:  If the role does not have a Cost per Hour rate, the Available Role Cost is $0.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Project Available Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The Available Cost per project is calculated using the following formula:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Calculate Planned Cost in the *`Resource Planner`* {#calculate-planned-cost-in-the-resource-planner}

Although you cannot view task information in the *`Resource Planner`*, the Planned Costs for users, roles, and the projects are calculated by taking into account the following task information:



*  The type of assignment on the task.  
  You can leave a task unassigned, or assign the following entities to a task: 
    
    
    * A User (with or without a Job Role)
    * A Role
    * A Team  
      A task assigned to a Team is considered unassigned, from the perspective of the *`Resource Planner`*. 
    
    
    

*  The `Cost Type` of the tasks on the project.  
  For more information about the Cost Type of a task, see [Track costs](track-costs.md).



This following table illustrates how Planned Cost is calculated in the *`Resource Planner`*, depending on the Cost Type of the tasks on the project: 

<table style="width: 717px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 142px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td rowspan="2" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> </p> <p> </p> </td> 
   <td colspan="3" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold">Cost Type = User Hourly</span> </p><span class="bold">User Planned Cost </span> </td> 
   <td colspan="3" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="bold">Cost Type = Role Hourly</span> </p><span class="bold">Role Planned Cost</span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">No Assignment</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">User <br>Assignment</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">Job Role Assignment</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">No Assignment</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">User Assignment</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="bold">Job Role Assignment</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold">User and Role Planned Cost</span> </p> <p> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>The Role and User Planned Costs are $0.00.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><p>Note:  The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.</p></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>The Role and User Planned Costs are $0.00.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td rowspan="2" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">Project Planned Cost</span> </p> <p> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The Project Planned Cost is $0.00.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The Project Planned Cost is $0.00.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The Project Planned Cost is $0.00.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>The Project Planned Cost is $0.00.</p> </td> 
   <td colspan="2" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td colspan="6" class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Note:  User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span>. </p> </td> 
  </tr> 
 </tbody> 
</table>



## Calculate Budgeted Cost in the *`Resource Planner`* {#calculate-budgeted-cost-in-the-resource-planner}

To display Budgeted Cost values in the *`Resource Planner`* you must have the following:



* Budgeted Hours for roles, users, and projects.
* Cost per Hour rates for users and roles.




>[!NOTE]
>
>The Budgeted Hours for the projects are calculated based on the Budgeted Hours for the Roles, not those of users.


The following table illustrates how Budgeted Cost is calculated in the *`Resource Planner`*: 

<table style="width: 567px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 214px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 786px;"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Budgeted Cost</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Calculation</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">User Budgeted Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The Budgeted Cost per user is calculated using the following formula:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p>Note:  If the user does not have a Cost per Hour rate in their profile, the Budgeted User Cost is $0.00.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Role Budgeted Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The Role Budgeted Cost is calculated using the following formula:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p>Note:  If the role does not have a Cost per Hour rate, the Budgeted Role Cost is $0.00.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Project Budgeted Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The Budgeted Cost per project is calculated using the following formula:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>

