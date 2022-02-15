---
filename: kick-starts-scenario-company-group-role-user-prep
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
---



# Kick-Starts Scenario: Company, Group, Role, and User Kick-Starts Preparation  {#kick-starts-scenario-company-group-role-and-user-kick-starts-preparation}

When you begin implementing *`Adobe Workfront`*, rather than manually inputting data, you can import your customer list, internal departments, job roles, and user information.


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



## What you can import {#what-you-can-import}

The following table displays the Companies, Groups, and Roles to import:

<table cellspacing="15" cellpadding="5" style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow"> 
 <col style="width: 165px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 165px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 165px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Companies</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Groups</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Roles</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Acme, Co</p> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, Inc.</p> <p><em>Your Company</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p valign="top" rowspan="7">Finance</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Sales</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p valign="top">Business Analyst</p> <p valign="top">Controller Creative</p> <p valign="top">Designer</p> <p valign="top">Resource Manager</p> <p valign="top">Scrum Master</p> <p valign="top">Technical Writer</p> <p valign="top">Web Developer</p> </td> 
  </tr> 
 </tbody> 
</table>

Role names must be unique, existing&nbsp;job roles cannot be imported.


The following tables display the users to import and several user attributes for each:


### User 1 {#user}




### User 2 {#user-1}




### User 3 {#user-2}




### User 4 {#user-3}




### User 5 {#user-4}




### User 6 {#user-5}




## Download a Kick-Start Template {#download-a-kick-start-template}




1. Click `Setup` near the upper-right corner of *`Adobe Workfront`* on the Global Navigation Bar.

1. Click `System`> `Kick-Starts` > `Import Data.`

1. Click `More Options` to see the full list of import options.
1. Select the Access Level, Company, Group, Job Role, and User objects that you want to import.




## Input company information {#input-company-information}




1.  Open the ` *`Workfront`*.xlsx`&nbsp;file you just downloaded.

   ` `**Tip: **`` When working with very wide data sheets, you may want to use your spreadsheet editor's Freeze Pane (or equivalent) tool to make the spreadsheet easier to work with.


   ![](assets/freezepanes-350x140.png)



1.  Go to the 'CMPY Company' sheet.


   It should be empty unless companies are already in the system. ![](assets/cmpysheet-350x16.png)




   ![](assets/companyid--1--350x78.png)



1. Specify TRUE into the `isNew`&nbsp;column.
1.  Repeat this action for each company being added. (In this example, complete this action for&nbsp;rows 3-6, because four&nbsp;companies are being added.)


   ![](assets/cmpyisnew-350x86.png)



1.  Specify a unique ID.


   This must be done for each row for the ID column. Integers starting at 1 work well when creating new records.


   ![](assets/cmpyisnew-350x86.png)



1.  Set a Name.


   Specify the names of each customer in the `setName`&nbsp;column.


   ![](assets/companyid-350x78.png)



1.  Go to the GROUP Group sheet.


   Unless you have already created groups in *`Workfront`*, this sheet should display only the Default Group provisioned with every account of *`Workfront`*.


   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)



1. Set the `isNew`&nbsp;column.According to the scenario, 4 groups will be imported, so specify TRUE into rows 4 through 7 for the 'isNew' column.
1.  Specify a unique ID.


   This must be done for each row for the ID column. Integers starting at 1 work well when creating new records.


   ![](assets/groupids-350x85.png)



1.  Set a Name.


   Specify the names of each department in the `setName`&nbsp;column.


   ![](assets/groupnames-350x85.png)




   Specify role information.&nbsp;Go to the ROLE Role sheet.

1.  Unless you have already created or deleted roles in your account, this sheet should display 8 roles that are provisioned with every account of  *`Workfront`*.


   ![](assets/groupnames-350x85.png)



1.  Set True statement.


   Seven Job Roles are importing, input TRUE into rows 12 through 18 for the 'isNew' column.


   ![](assets/roleisnew-350x104.png)



1.  Specify a unique ID.


   This must be done for each row for the ID column. Integers starting at 1 work well when creating new records.&nbsp;


   ![](assets/usersheet-350x16.png)




   ![](assets/roleisnew--1--350x104.png)



1.  Provide a names for each role by typing it in the setName column.


   ![](assets/roleisnew-350x104.png)



1.  Provide additional details as needed.


   Include billing rates, cost rates, and descriptions for the Roles you are creating, as needed.

1.  Go to the USER User sheet to input User Information.


   Unless you have already created users in your account, this sheet should display only the Admin User that is provisioned with every account of *`Workfront`*.


   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)



1.  Set True value by specifying&nbsp;TRUE into rows 4 through 9 for the 'isNew' column, since 6 users are being imported.


   ![](assets/userisnew-350x52.png)



1.  Set a unique ID by specifying&nbsp;a unique ID in each row for the ID column. Typically integers starting at 1 work well for new records.


   ![](assets/userisnew-350x52.png)



1.  Input the names of each user into the 'setFirstName'&nbsp;and 'setLastName' columns.


   ![](assets/usernames-350x52.png)



1.  Set detail values by specifying&nbsp;values into the 'setEmail,'&nbsp;'setPassword,' and 'setUsername' columns.


   ![](assets/usercredentials-350x52.png)



1.  Specify Access Level values.


   For example, Chris Manning, who is a Team Member, look up the ID on the ACSLVL Access Level sheet for the Team Member access level. Copy the ID into your clipboard, and on the USER User sheet paste it in the `setAccessLevelID` column on Chris' row.&nbsp;


   Repeat this step for each user and access level.


   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)



1.  Specify&nbsp;Home Group details.


   According to the scenario, Chris Manning belongs to the Marketing group. On the GROUP Group sheet, locate the ID for the Marketing group, copy it into the clipboard, and on the USER User sheet paste it in the `setHomeGroupID`column on Chris' row.&nbsp;​Repeat this step for each user and group assignment.


   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)



1.  Specify Company details.


   All the users in this scenario belong to the same company. On the CMPY Company sheet, locate the ID for the *Your Own Company *company, copy the ID into the clipboard, and on the USER User tab, paste this value into each row of the 'setCompanyID' column.​


   Repeat this step for each user and group assignment.


   ![](assets/companyid--1--350x78.png)




   ![](assets/pastecompanyid-350x84.png)



1.  Specify Job Role details.


   According to the scenario, Chris Manning will have the Business Analyst role. On the ROLE Role sheet, locate the ID for the Business Analyst role, copy it into the clipboard, and on the USER User sheet paste it in the 'setRoleID' column on Chris' row.&nbsp;​Repeat this step for each user and group assignment.


   ![](assets/copyroleid-350x149.png)




   ![](assets/pasteroleid-350x95.png)



1. Fill in other user details, as needed, then save the file.
1.  Import the Excel File.


   Follow the directions provided in the `Importing Kick Start Files` section of this article.



