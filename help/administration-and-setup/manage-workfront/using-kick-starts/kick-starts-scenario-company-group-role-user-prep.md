---
filename: kick-starts-scenario-company-group-role-user-prep
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Kick-Starts Scenario: Company, Group, Role, and User Kick-Starts Preparation
description: When you begin implementing Adobe Workfront, rather than manually inputting data, you can import your customer list, internal departments, job roles, and user information.
---

# Kick-Starts Scenario: Company, Group, Role, and User Kick-Starts Preparation

When you begin implementing Adobe Workfront, rather than manually inputting data, you can import your customer list, internal departments, job roles, and user information.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## What you can import

The following table displays the Companies, Groups, and Roles to import:

<table cellspacing="15" cellpadding="5"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Companies</span> </th> 
   <th><span class="bold">Groups</span> </th> 
   <th><span class="bold">Roles</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em>Your Company</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Finance</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Sales</p> </td> 
   <td valign="top"> <p valign="top">Business Analyst</p> <p valign="top">Controller Creative</p> <p valign="top">Designer</p> <p valign="top">Resource Manager</p> <p valign="top">Scrum Master</p> <p valign="top">Technical Writer</p> <p valign="top">Web Developer</p> </td> 
  </tr> 
 </tbody> 
</table>

Role names must be unique, existing&nbsp;job roles cannot be imported.

The following tables display the users to import and several user attributes for each:

### User 1

| `First Name`  |Chris |
|---|---|
| `Last Name`  |Manning |
| `Username/Email`  | [cmanning@foo.com](mailto:cmanning@foo.com)  |
| `Password`  |updateMe |
| `Access`  |Team Member |
| `Company`  |<*Your Company>* |
| `Home Group`  |Marketing |
| `Job Role`  |Business Analyst |

### User 2

| `First Name`  |Jennifer |
|---|---|
| `Last Name`  |Campbell |
| `Username/Email`  |jcampbell@foo.com |
| `Password`  |updateMe |
| `Access`  |Project Manager |
| `Company`  |<*Your Company>* |
| `Home Group`  |Marketing |
| `Job Role`  |Project Manager |

### User 3

| `First Name`  |Jill |
|---|---|
| `Last Name`  |Sullivan |
| `Username/Email`  |jsullivan@foo.com |
| `Password`  |updateMe |
| `Access`  |Help Desk |
| `Company`  |<*Your Company>* |
| `Home Group`  |Sales |
| `Job Role`  |Sales Rep |

### User 4

| `First Name`  |Marc |
|---|---|
| `Last Name`  |Lewis |
| `Username/Email`  |mlewis@foo.com |
| `Password`  |updateMe |
| `Access`  |Portfolio Manager |
| `Company`  |<*Your Company>* |
| `Home Group`  |Finance |
| `Job Role`  |Controller |

### User 5

| `First Name`  |Pam |
|---|---|
| `Last Name`  |Reynolds |
| `Username/Email`  |preynolds@foo.com |
| `Password`  |updateMe |
| `Access`  |Project Manager |
| `Company`  |*Your Company>* |
| `Home Group`  |Marketing |
| `Job Role`  |IT |

### User 6

| `First Name`  |Ray |
|---|---|
| `Last Name`  |Andrews |
| `Username/Email`  |randrews@foo.com |
| `Password`  |updateMe |
| `Access`  |Administrator |
| `Company`  |*Your Company>* |
| `Home Group`  |Resource Manager |
| `Job Role`  |none |

## Download a Kick-Start Template

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Kick-Starts</span> > <span class="bold">Import Data.</span></li> 
 <li value="3">Click <span class="bold">More Options</span> to see the full list of import options.</li> 
 <li value="4">Select the Access Level, Company, Group, Job Role, and User objects that you want to import.</li> 
</ol>

## Input company information

<ol> 
 <li value="1"> <p>Open the <span class="bold">Workfront.xlsx</span>&nbsp;file you just downloaded.</p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>When working with very wide data sheets, you may want to use your spreadsheet editor's Freeze Pane (or equivalent) tool to make the spreadsheet easier to work with.</p> 
   <p> <img src="assets/freezepanes-350x140.png" style="width: 350;height: 140;"> </p> 
  </div> </li> 
 <li value="2"> <p>Go to the 'CMPY Company' sheet.</p> <p>It should be empty unless companies are already in the system.<img src="assets/cmpysheet-350x16.png" style="width: 350;height: 16;"></p> <p> <img src="assets/companyid--1--350x78.png" style="width: 350;height: 78;"> </p> </li> 
 <li value="3">Specify&nbsp;TRUE&nbsp;into the <span class="bold">isNew</span>&nbsp;column.</li> 
 <li value="4"> <p>Repeat this action for each company being added. (In this example, complete this action for&nbsp;rows 3-6, because four&nbsp;companies are being added.)</p> <p> <img src="assets/cmpyisnew-350x86.png" style="width: 350;height: 86;"> </p> </li> 
 <li value="5"> <p>Specify a unique ID.</p> <p>This must be done for each row for the ID column. Integers starting at 1 work well when creating new records.</p> <p> <img src="assets/cmpyisnew-350x86.png" style="width: 350;height: 86;"> </p> </li> 
 <li value="6"> <p>Set a Name.</p> <p>Specify the names of each customer in&nbsp;the <span class="bold">setName</span>&nbsp;column.</p> <p> <img src="assets/companyid-350x78.png" style="width: 350;height: 78;"> </p> </li> 
 <li value="7"> <p>Go to the GROUP Group sheet.</p> <p>Unless you have already created groups in Workfront, this sheet should display only the Default Group provisioned with every account of Workfront.</p> <p> <img src="assets/groupsheet-350x15.png" style="width: 350;height: 15;"> <img src="assets/emptygroupsheet-350x85.png" style="width: 350;height: 85;"> </p> </li> 
 <li value="8">Set the <span class="bold">isNew</span>&nbsp;column.According to the scenario, 4 groups will be imported, so specify TRUE into rows 4 through 7 for the 'isNew' column.</li> 
 <li value="9"> <p>Specify a unique ID.</p> <p>This must be done for each row for the ID column. Integers starting at 1 work well when creating new records.</p> <p> <img src="assets/groupids-350x85.png" style="width: 350;height: 85;"> </p> </li> 
 <li value="10"> <p>Set a Name.</p> <p>Specify the names of each department in&nbsp;the <span class="bold">setName</span>&nbsp;column.</p> <p> <img src="assets/groupnames-350x85.png" style="width: 350;height: 85;"> </p> <p>Specify role information.&nbsp;Go to the ROLE Role sheet.</p> </li> 
 <li value="11"> <p>Unless you have already created or deleted roles in your account, this sheet should display 8 roles that are provisioned with every account of&nbsp;Workfront.</p> <p> <img src="assets/groupnames-350x85.png" style="width: 350;height: 85;"> </p> </li> 
 <li value="12"> <p>Set True statement.</p> <p>Seven Job Roles are importing, input TRUE into rows 12 through 18 for the 'isNew' column.</p> <p> <img src="assets/roleisnew-350x104.png" style="width: 350;height: 104;"> </p> </li> 
 <li value="13"> <p>Specify a unique ID.</p> <p>This must be done for each row for the ID column. Integers starting at 1 work well when creating new records.&nbsp;</p> <p> <img src="assets/usersheet-350x16.png" style="width: 350;height: 16;"> </p> <p> <img src="assets/roleisnew--1--350x104.png" style="width: 350;height: 104;"> </p> </li> 
 <li value="14"> <p>Provide a names for each role by typing it in the setName column.</p> <p> <img src="assets/roleisnew-350x104.png" style="width: 350;height: 104;"> </p> </li> 
 <li value="15"> <p>Provide additional details as needed.</p> <p>Include billing rates, cost rates, and descriptions for the Roles you are creating, as needed.</p> </li> 
 <li value="16"> <p>Go to the USER User sheet to input User Information.</p> <p>Unless you have already created users in your account, this sheet should display only the Admin User that is provisioned with every account of Workfront.</p> <p> <img src="assets/rolenames-350x104.png" style="width: 350;height: 104;"> <img src="assets/emptyusersheet-350x52.png" style="width: 350;height: 52;"> </p> </li> 
 <li value="17"> <p>Set True value by specifying&nbsp;TRUE into rows 4 through 9 for the 'isNew' column, since 6 users are being imported.</p> <p> <img src="assets/userisnew-350x52.png" style="width: 350;height: 52;"> </p> </li> 
 <li value="18"> <p>Set a unique ID by specifying&nbsp;a unique ID in each row for the ID column. Typically integers starting at 1 work well for new records.</p> <p> <img src="assets/userisnew-350x52.png" style="width: 350;height: 52;"> </p> </li> 
 <li value="19"> <p>Input the names of each user into the 'setFirstName'&nbsp;and 'setLastName' columns.</p> <p> <img src="assets/usernames-350x52.png" style="width: 350;height: 52;"> </p> </li> 
 <li value="20"> <p>Set detail values by specifying&nbsp;values into the 'setEmail,'&nbsp;'setPassword,' and 'setUsername' columns.</p> <p> <img src="assets/usercredentials-350x52.png" style="width: 350;height: 52;"> </p> </li> 
 <li value="21"> <p>Specify Access Level values.</p> <p>For example, Chris Manning, who is a Team Member, look up the ID on the ACSLVL Access Level sheet for the Team Member access level. Copy the ID into your clipboard, and on the USER User sheet paste it in the <span class="bold">setAccessLevelID</span> column on Chris' row.&nbsp;</p> <p>Repeat this step for each user and access level.</p> <p> <img src="assets/copyalid-350x171.png" style="width: 350;height: 171;"> <img src="assets/pastealid-350x59.png" style="width: 350;height: 59;"> </p> </li> 
 <li value="22"> <p>Specify&nbsp;Home Group details.</p> <p>According to the scenario, Chris Manning belongs to the Marketing group. On the GROUP Group sheet, locate the ID for the Marketing group, copy it into the clipboard, and on the USER User sheet paste it in the <span class="bold">setHomeGroupID</span>column on Chris' row.&nbsp;​Repeat this step for each user and group assignment.</p> <p> <img src="assets/copygroupid-1-350x133.png" style="width: 350;height: 133;"> <img src="assets/pastegroupid-350x59.png" style="width: 350;height: 59;"> </p> </li> 
 <li value="23"> <p>Specify Company details.</p> <p>All the users in this scenario belong to the same company. On the CMPY Company sheet, locate the ID for the <em>Your Own Company </em>company, copy the ID into the clipboard, and on the USER User tab, paste this value into each row of the 'setCompanyID' column.​</p> <p>Repeat this step for each user and group assignment.</p> <p> <img src="assets/companyid--1--350x78.png" style="width: 350;height: 78;"> </p> <p> <img src="assets/pastecompanyid-350x84.png" style="width: 350;height: 84;"> </p> </li> 
 <li value="24"> <p>Specify Job Role details.</p> <p>According to the scenario, Chris Manning will have the Business Analyst role. On the ROLE Role sheet, locate the ID for the Business Analyst role, copy it into the clipboard, and on the USER User sheet paste it in the 'setRoleID' column on Chris' row.&nbsp;​Repeat this step for each user and group assignment.</p> <p> <img src="assets/copyroleid-350x149.png" style="width: 350;height: 149;"> </p> <p> <img src="assets/pasteroleid-350x95.png" style="width: 350;height: 95;"> </p> </li> 
 <li value="25">Fill in other user details, as needed, then save the file.</li> 
 <li value="26"> <p>Import the Excel File.</p> <p>Follow the directions provided in the <span class="bold">Importing Kick Start Files</span> section of this article.</p> </li> 
</ol>

