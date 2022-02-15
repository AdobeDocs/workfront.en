---
filename: set-up-exchange-rates
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
---



# Set up exchange rates {#set-up-exchange-rates}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


As an *`Adobe Workfront administrator`*, you can set up currency exchange rates in *`Workfront`*. This includes the following:



* Setting the default currency for the *`Workfront`*&nbsp;system
* Updating exchange rates in *`Workfront`* to match current exchange rates
* Configuring the exchange rates for&nbsp;multiple currencies (doing so enables&nbsp;users to choose a default currency for individual projects)


Exchange rates impact all financial elements in *`Workfront`*. The Base Currency is the default currency for all projects throughout the system, unless it is overridden for a given project `or job role`. You can also select to display financial information in currencies available in your system that are different than the base currency or that of the project when viewing them in a report or list. For more information, see [Create financial data reports with unique exchange rates](create-financial-data-reports-unique-exchange-rates.md).


For more information about overriding the Base Currency in  *`Workfront`* for projects `and job roles`, see the following articles: 



*  [Change the project currency](change-project-currency.md) 
*  
  [Create and manage job roles](create-manage-job-roles.md) 


The way that you set up exchange rates affects whether users can modify exchange rates for a given project.


>[!IMPORTANT] {type="important"}
>
>Exchange rates in *`Workfront`*&nbsp;are not dynamic; the value that you set must&nbsp;be updated when changes in exchange&nbsp;rates occur.&nbsp;




## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Set up exchange rates {#set-up-exchange-rates-1}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).  

1. Click `Project Preferences` > `Exchange Rates.`  

1. Click `Add Currency.`
1.  Begin typing the name of the currency, then click it when it appears in the drop-down list.  

1. In the provided field, specify the rate for the currency that you selected, as it relates to the currency that is set as the base currency in the system.
1.  (Optional) Set the currency as the base (default) currency for *`Workfront`*. 


   This is the currency that is used as the default for all projects and reports throughout the system.

1. Click `Save`&nbsp;to save your changes.&nbsp;




## Enable users to modify the default currency for a project {#enable-users-to-modify-the-default-currency-for-a-project}

Users can modify the default currency for a project when the following conditions are met:



*  The user has a Plan license with the administrative access to Exchange Rates.  



  For more information, see [Grant users administrative access to certain areas](grant-users-admin-access-certain-areas.md).

* More than one currency is enabled on the *`Workfront`* system.


For information about how users can change the default currency on a given project, see [Change the project currency](change-project-currency.md).



## Enable users to modify the default currency for a job role {#enable-users-to-modify-the-default-currency-for-a-job-role}

Users can modify the currency for a job role when the following conditions are met:



*  The user has a Plan license with the administrative access to Job&nbsp;Roles.  



  For more information, see [Grant users administrative access to certain areas](grant-users-admin-access-certain-areas.md).

* More than one currency is enabled on the *`Workfront`* system.


For information about how users can change the default currency on a given job role, see [Create and manage job roles](create-manage-job-roles.md).
