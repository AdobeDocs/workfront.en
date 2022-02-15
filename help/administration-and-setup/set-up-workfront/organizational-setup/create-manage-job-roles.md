---
filename: create-manage-job-roles
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
---



# Create and manage job roles {#create-and-manage-job-roles}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


As an *`Adobe Workfront administrator`* or a user with administrative access to Job Roles, you can create job roles which can be assigned to users and delete default job roles that are not relevant to your organization. For information about administrative access in *`Workfront`*, see [Grant users administrative access to certain areas](grant-users-admin-access-certain-areas.md).


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Administrative access to Job roles</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create a job role {#create-a-job-role}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Job Roles.`
1.  Click `New Job Role.`


   ![](assets/new-job-role-box-with-currency-override-nwe-350x312.png)



1.  Update the following fields: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Indicate a name for the job role.&nbsp;This is the name that displays everywhere in&nbsp;<span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> where the Job&nbsp;Role field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span>Is Active</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ul> 
     <li> <p><span><span>Select <span class="bold">Yes</span> if you want the role to be active and available everywhere in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> to be associated with users, work items, etc. </span></span> </p> </li> 
     <li> <p><span><span>Select <span class="bold">No</span>, if you want the role to be deactivated</span></span><span> and not available to assign to users, work items, etc. </span> </p> </li> 
    </ul> <p><span>For information about deactivating job roles, see</span> <a href="deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Enter a description for the role that indicates what is unique about it. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="preview">Base Currency</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="preview">This is the Base Currency, as set in the Setup area by your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For information, see</span> <a href="set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span class="preview">You cannot edit the Base Currency at the job role level.&nbsp;This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Cost/ Hr.</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. <span class="preview">Enter the rate using the Base Currency. </span></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Bill/ Hr. </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. <span class="preview">Enter </span><span class="preview" data-mc-edit-date="2021-11-22T14:56:29.1266973-05:00" data-mc-editor="alinaw" data-mc-comment="drafted, yellow and will stay nwe always" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2021-11-22T14:56:19.0720157-05:00">the</span><span class="preview"> rate using the Base Currency. </span></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="preview">Override Currency</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <div class="preview"> 
     <p>Select a currency associated with this job role. This is the currency that <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> uses for calculating costs and revenue associated with this job role. </p> 
     <p><span>This is a different than the Base Currency set up by your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> in the Setup area, and can be different than the currency associated with a project. </span> </p> 
     <p>Tip: Only currencies available in the Exchange Rates area in your system are available in this field.</p> 
    </div> <p><span class="preview">For information about setting up the Base Currency in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see</span> <a href="set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span class="preview">For information about changing the currency of a project, see</span> <a href="change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="preview">Override Currency Cost/ Hour</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <div class="preview"> 
     <p>This is the cost per hour rate of the job role using the selected Override Currency. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
     <p><span>Enter the rate in the Override Currency specified above. This also updates the Cost/ Hour rate for this job role when using the Base Currency. </span> </p> 
     <p>For information about how <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates cost, see <a href="track-costs.md" class="MCXref xref">Track costs</a>.</p> 
    </div> <p>Tip: <span class="preview">When updating an existing job role that already has a Cost/ Hour rate associated with it, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost/ Hour, the Cost/ Hour of the job role also updates automatically. </span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="preview">Override Currency Billing/ Hour</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> 
    <div class="preview"> 
     <p>This is the billing per hour rate of the job role using the selected Override Currency. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p> 
     <p><span>Enter the rate in the Override Currency specified above. This also updates the Billing/ Hour rate for this job role when using the Base Currency. </span> </p> 
     <p>For information about how <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates revenue, see <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> 
    </div> <p>Tip: <span class="preview">When updating an existing job role that already has a Billing/ Hour rate associated with it, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing/ Hour, the Billing/ Hour of the job role also updates automatically. </span> </p> </td> 
  </tr> 
 </tbody> 
</table>



   >[!TIP] {type="tip"}
   >
   >Job roles are an integral&nbsp;part of managing resources. To use the resource planning tools, job roles need a cost and billing rate associated with them. For information, see [Get started with Resource Management](get-started-resource-management.md). 



1.  Click `Create Job Role`. The job role is now available to be assigned to tasks, issues, approvals, or you can share layout templates or other objects with it. For information about all uses of job roles in  *`Workfront`*, see [Job role overview](job-role-overview.md). For information about deleting a job role, see [Delete job roles](delete-job-roles.md). 




##  

