---
filename: recalculate-project-finances
title: Recalculate project finances
product-area: projects
navigation-topic: financials
---



# Recalculate project finances {#recalculate-project-finances}

Finances are calculated on a project as changes occur in the hours logged for the project or in the rates used to calculate costs and revenue. 



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Considerations about calculating finances in *`Adobe Workfront`* {#considerations-about-calculating-finances-in-adobe-workfront}

Finances are calculated in *`Enhanced analytics`* in the following ways: 



* You can manually recalculate costs and revenues on a project, by using the Recalculate Finance option on a project. 
* In addition, some actions trigger an automatic recalculation. 


When the rate of a user or a role changes during the life of a project, the following can occur: 



*  When the change is made, the updated rate is used from that point on as hours are logged and the financial information is calculated. Changing the rate does not affect how things were calculated before the change was made. For all the existing hours logged, the old rate is used to calculate financial information. 
* You can force *`Adobe Workfront`* to use the new rate retroactively for all the hours logged so far, by using the Recalculate Finance option. This forces *`Workfront`* to retroactively recalculate all previously entered hours, planned costs, and revenues in accordance with the new rate information.



` `**Warning: **``Prior to manually recalculating finances for a given project, you might want to preserve any financial data that has already been calculated at a previous rate. We recommend to use the Recalculate Finance option only when you are sure that you are not making changes to existing information, or only when such changes are desired. 


## Preserve financial data for tasks with existing hours {#preserve-financial-data-for-tasks-with-existing-hours}

When financial data for a project is recalculated, *`Workfront`* retroactively recalculates all previously logged hours, planned, actual costs, and planned and actual revenue, in accordance with any new or updated financial information. 



* [Preserve Project Revenue](#preserve-revenue) 
* [Preserve Project Cost](#preserve-cost) 




### Preserve Project Revenue  {#preserve-project-revenue}

Revenue rates can change during the lifetime of a project. 


For more information about billing rates and revenue, see the article [Overview of Billing and Revenue](billing-and-revenue-overview.md).


Revenue rates can change at the following levels:



* The system level (for job roles)  
  For more information about creating job roles with billing rates at the system level, see the article [Create and manage job roles](create-manage-job-roles.md).

* The user level  
  For more information about changing the billing rate information on users, see the article [Edit a user's profile](edit-a-users-profile.md).

* The Company level (for job roles)  
  For more information, see [Override job role billing rates at the company level](override-job-role-billing-rates-company-level.md).

* The Project level (for job roles)  
  For more information about overriding job role rates at the project level, see the article [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](override-role-billing-rates-and-calculate-project-revenue.md).



For example, a user's billing rate changes during the course of a project from $50 to $75 an hour and you want all existing data to remain calculated at the old rate ($50 and hour). However, when the project finances are recalculated, tasks that already have existing financial data will have the revenue updated to reflect the new billing rate (of $75 an hour). 



* [Preserve Project Revenue by creating a Billing Record](#create-billing-record) 
* [Preserve Project Revenue by using multiple Billing Rate overrides](#multiple-billing-rate-overrides) 




#### `Preserve Project Revenue by creating a Billing Record`  {#preserve-project-revenue-by-creating-a-billing-record}

When billing rates change at any level mentioned above, you can preserve existing revenue which has already been calculated on the project by avoiding to use the manual Recalculate Finance option or by locking the time recorded on the project and calculated using the old rate into a billing record with a status of Billed. 


When you do not recalculate finances on the project or when you lock the hours logged into a billed billing record, the hours logged after the rate changes will calculate with the new rate, and the hours logged before the cost rate changes remain calculated at the old rate. 


For more information about creating billing records, see the article [Create billing records](create-billing-records.md).


#### `Preserve Project Revenue by using multiple Billing Rate overrides`  {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

When billing rates change for job roles at the project level, you can preserve existing revenue which has already been calculated on the project by using multiple billing rates overrides which are locked within a specified time frame. 


For more information about using multiple billing rates overrides, see the article [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](override-role-billing-rates-and-calculate-project-revenue.md).


>[!NOTE]
>
>This only applies to job role billing rates that are changed at the project level. 




### Preserve Project Cost {#preserve-project-cost}

Cost rates can change at the following levels:



* System level (for job roles)  
  For more information about creating job roles with cost rates at the system level, see the article [Create and manage job roles](create-manage-job-roles.md).  

* User level  
  For more information about changing the cost rate information on users, see the article [Edit a user's profile](edit-a-users-profile.md).  



When billing rates change at any level mentioned above, you can preserve existing costs which have already been calculated on the project by locking the time recorded on the project and calculated using the old rate into a billing record with a status of Billed. For more information about creating billing records, see the article [Create billing records](create-billing-records.md).


You can also avoid using the manual Recalculate Finance option, if you don't want to create a billing record, as described in the section [Manually recalculate finances for a project](#manually-recalculating-finances-for-a-project) in this article. 


When you do not recalculate finances on the project or when you lock the hours logged into a billed billing record, the hours logged after the rate changes will calculate with the new rate, and the hours logged before the cost rate changes remain calculated at the old rate. 


## Manually recalculate finances for a project {#manually-recalculate-finances-for-a-project}

If your rates change during the life of a project and you want your cost and revenue calculations to reflect the new rates, you must manually recalculate the finances on the project. 


>[!NOTE]
>
>You can prevent revenue values from updating to reflect the new rates when you manually recalculate finance by following the steps in the section [Preserve financial data for tasks with existing hours](#preserving-financial-data-for-tasks-with-existing-hours) of this article. Cost values are always updated to reflect the new rates when you manually recalculate the finances on a project. 


To recalculate finances for a project manually:



1. Go to the project where you want to recalculate finances. 
1.  Click the `More` menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the project, then click `Recalculate Finance`. 


   All planned costs and revenue on the project are recalculated with any new information.  
  
   You should receive a confirmation at the top of the browser that the finances of the project have been recalculated successfully.  
   Existing cost values and some revenue values which have not been locked update to reflect the new rates. 





## Manually recalculate finances for several projects in bulk {#manually-recalculate-finances-for-several-projects-in-bulk}

You can manually recalculate the finances of several projects by editing them in bulk. This causes the revenue on the projects to recalculate retroactively. 




>[!IMPORTANT] {type="important"}
>
>You can prevent revenue values from updating to reflect the new rates when you manually recalculate finance by following the steps in the section [Preserve financial data for tasks with existing hours](#preserving-financial-data-for-tasks-with-existing-hours) of this article. Cost values are always updated to reflect the new rates when you manually recalculate the finances on projects. 





To manually recalculate the finances of several projects: 



1. Go to a list of projects.
1. Select several projects in the list, then click `Edit`.
1. Click `Settings`, then select `Recalculate Costs And Revenues`.

1. Click `Save Changes`.




## Actions that trigger an automatic recalculation of finances {#actions-that-trigger-an-automatic-recalculation-of-finances}

The following actions trigger the financial recalculation of projects in *`Workfront`*:



* Changing task status
* Moving a task with hours to another project
* Changing the project status from Complete to an active status




>[!NOTE]
>
>When you change the project status, only the planned values are being recalculated.


You can also recalculate finances manually under the `More` menu ![](assets/qs-more-menu.png) at the project level, by clicking `Recalculate Finances`. 
