---
filename: manage-project-expenses
product-area: projects
navigation-topic: financials
---



# Manage project expenses  {#manage-project-expenses}

The process for creating and managing expenses&nbsp;is the same for both project and task-related expenses. Any expenses that are added to the project in the Business Case are added to the Expenses tab as planned expenses. For more information on the Business Case, see the article [Create a Business Case for a project in Adobe Workfront](create-business-case.md).


The total amount of your expenses from all the tasks and the project contributes to the total cost of the project. The Planned Amount of the expenses contributes to the Planned Cost of the project, and the Actual Amount of the expenses contributes to the Actual Cost of the project.



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


## Add Expenses {#add-expenses}




1. Go to the&nbsp;project where you want to enter expenses.  
   If you want to add expenses to a task, navigate to a task instead.&nbsp;
1.  Click ```<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">Show </span></MadCap:conditionalText>` `More,`then click  `Expenses.`
1.  Click  `Add an Expense.`  
   The `Add an Expense`&nbsp;dialog box is displayed.
1.  Specify the following information:

    
    
    *  `Description:` Description of the expense.  

    * `Expense Type:` (Required) Select the category that best describes the expense.
    * `Task:` Begin typing the name of the task that this expense is associated with, then click it when it appears in the drop-down list.
    * `Planned Amount:` The planned budgeted amount for the expense.  
      This affects the Budgeted Cost of the project.
    
    * `Actual Amount:` The amount that the expense actual cost.  
      This affects the Actual Cost of the project.
    
    * `Planned Date:` The expected date for the expense to occur. You&nbsp;can type the&nbsp;date in the field using the *mm/dd/yy* format, or you can click&nbsp;the calendar icon&nbsp; ![](assets/calendar-icon.png)&nbsp;and select the date dynamically.
    
    * `Date Paid:` The date the expense was paid.
    * `Billable:` Select this option&nbsp;if you want to&nbsp;bill this expense. Categorizing an expense as billable is important when creating billing records.
    * `Reimbursable:` Select this option&nbsp;if the expense needs to be reimbursed. You can then mark the expense as reimbursed after the expense has been reimbursed.
    
    

1. Select a `Custom Form` and specify any additional information required. You must create a custom form before you can associate it with an expense. Only active custom forms display in the list. For information about creating custom forms, see the article [Create or edit a custom form](create-or-edit-a-custom-form.md).

1. Click `Save Changes.`




## Delete Expenses {#delete-expenses}




1. Go to the&nbsp;project where you want to delete expenses.
1.  Click ```<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">Show </span></MadCap:conditionalText>` `More,`then click  `Expenses.`
1. Select the expenses that you want to delete, then click `Delete.`
1. Click  `Yes, Delete It` to confirm deletion.&nbsp;


