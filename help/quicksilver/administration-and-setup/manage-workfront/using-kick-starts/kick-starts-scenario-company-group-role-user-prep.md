---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: "Kick-Starts Scenario: Company, Group, Role, and User Kick-Starts Preparation"
description: When you begin implementing Adobe Workfront, rather than manually inputting data, you can import your customer list, internal departments, job roles, and user information.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
---
# Kick-Starts scenario: company, group, role, and user Kick-Starts preparation

When you begin implementing Adobe Workfront, rather than manually inputting data, you can import your customer list, internal departments, job roles, and user information.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## What you can import

The following table displays the companies, groups, and roles to import:

| Companies | Groups | Roles |
|---|---|---|
| Acme, Co <p>Workfront, Inc. <p>_Your Company_ <p>XYZ, Inc. | Finance <p>IT <p>Marketing <p>Sales | Business Analyst <p>Controller Creative <p>Designer <p>Resource Manager <p>Scrum Master <p>Technical Writer <p>Web Developer |

{style="table-layout:auto"}

Role names must be unique. Existing job roles cannot be imported.

The following tables display the users to import and several user attributes for each:

### User 1

| Attribute |Value |
|---|---|
| **First Name** |Chris |
| **Last Name** |Manning |
| **Username/Email** |mailto:cmanning@foo.com  |
| **Password** |updateMe |
| **Access** |Team Member |
| **Company** |<*Your Company>* |
| **Home Group** |Marketing |
| **Job Role** |Business Analyst |

{style="table-layout:auto"}

### User 2

| Attribute |Value |
|---|---|
| **First Name** |Jennifer |
| **Last Name** |Campbell |
| **Username/Email** |jcampbell@foo.com |
| **Password** |updateMe |
| **Access** |Project Manager |
| **Company** |<*Your Company>* |
| **Home Group** |Marketing |
| **Job Role** |Project Manager |

{style="table-layout:auto"}

### User 3

| Attribute |Value |
|---|---|
| **First Name** |Jill |
| **Last Name** |Sullivan |
| **Username/Email** |jsullivan@foo.com |
| **Password** |updateMe |
| **Access** |Help Desk |
| **Company** |<*Your Company>* |
| **Home Group** |Sales |
| **Job Role** |Sales Rep |

{style="table-layout:auto"}

### User 4

| Attribute |Value |
|---|---|
| **First Name** |Marc |
| **Last Name** |Lewis |
| **Username/Email** |mlewis@foo.com |
| **Password** |updateMe |
| **Access** |Portfolio Manager |
| **Company** |<*Your Company>* |
| **Home Group** |Finance |
| **Job Role** |Controller |

{style="table-layout:auto"}

### User 5

| Attribute |Value |
|---|---|
| **First Name** |Pam |
| **Last Name** |Reynolds |
| **Username/Email** |preynolds@foo.com |
| **Password** |updateMe |
| **Access** |Project Manager |
| **Company** |*Your Company>* |
| **Home Group** |Marketing |
| **Job Role** |IT |

{style="table-layout:auto"}

### User 6

| Attribute |Value |
|---|---|
| **First Name** |Ray |
| **Last Name** |Andrews |
| **Username/Email** |randrews@foo.com |
| **Password** |updateMe |
| **Access** |Administrator |
| **Company** |*Your Company>* |
| **Home Group** |Resource Manager |
| **Job Role** |none |

{style="table-layout:auto"}

## Download a Kick-Start Template

{{step-1-to-setup}}

1. Click **System** > **Kick-Starts** > **Import Data.**

1. Click **More Options** to see the full list of import options.
1. Select the Access Level, Company, Group, Job Role, and User objects that you want to import.
1. Click **Download**.

## Input company information

1. Open the **Workfront.xlsx** file you just downloaded.

   >[!TIP]
   >
   >When working with very wide data sheets, you may want to use your spreadsheet editor's Freeze Pane (or equivalent) tool to make the spreadsheet easier to work with.

1. Go to the **CMPY Company** sheet.

   It should be empty unless companies are already in the system.
   
   ![Company sheet](assets/cmpysheet-350x16.png) ![Company ID](assets/companyid--1--350x78.png)

1. Enter **TRUE** in the **isNew** column.

   Repeat this action for each company being added. (In this example, complete this action for rows 3-6, because four companies are being added.)

   ![Company is new](assets/cmpyisnew-350x86.png)

1. Enter a unique **ID**.

   You must enter an ID for each row. Integers starting at 1 work well when creating new records.

   ![Company is new](assets/cmpyisnew-350x86.png)

1. Enter the names of each customer in the **setName** column.

   ![Company ID](assets/companyid-350x78.png)

1. Go to the **GROUP Group** sheet.

   Unless you have already created groups in Workfront, this sheet should display only the Default Group provisioned with every account of Workfront.

   ![Group sheet](assets/groupsheet-350x15.png) ![Empty group sheet](assets/emptygroupsheet-350x85.png)

1. Enter **TRUE** in the **isNew** column.

   According to the scenario, 4 groups will be imported, so enter **TRUE** in the **isNew** column for rows 4 through 7.

1. Enter a unique **ID**.

   You must enter an ID for each row. Integers starting at 1 work well when creating new records.

   ![Group IDs](assets/groupids-350x85.png)

1. Enter the names of each department in the **setName** column.

   ![Group names](assets/groupnames-350x85.png)

1. Go to the **ROLE Role** sheet.

   Unless you have already created or deleted roles in your account, this sheet should display 8 roles that are provisioned with every account of Workfront.

   ![Group names](assets/groupnames-350x85.png)

1. Enter **TRUE** in the **isNew** column.

   According to the scenario, 7 Job Roles will be imported, so enter **TRUE** in the **isNew** column for rows 12 through 18.

   ![Role is new](assets/roleisnew-350x104.png)

1. Enter a unique **ID**.

   You must enter an ID for each row. Integers starting at 1 work well when creating new records.

   ![Role is new](assets/roleisnew--1--350x104.png)

1. Enter a name for each role in the **setName** column.

   ![Role is new](assets/roleisnew-350x104.png)

1. Provide additional details as needed.

   Include billing rates, cost rates, and descriptions for the Roles you are creating, as needed.

1. Go to the **USER User** sheet.

   Unless you have already created users in your account, this sheet should display only the Admin User that is provisioned with every account of Workfront.

   ![User sheet](assets/usersheet-350x16.png) ![Empty user sheet](assets/emptyusersheet-350x52.png)

1. Enter **TRUE** in the **isNew** column.

   According to the scenario, 6 users will be imported, so enter **TRUE** in the **isNew** column for rows 4 through 9.

   ![User is new](assets/userisnew-350x52.png)

1. Enter a unique **ID**.

   You must enter an ID for each row. Integers starting at 1 work well when creating new records.

   ![User is new](assets/userisnew-350x52.png)

1. Enter the names of each user in the **setFirstName** and **setLastName** columns.

   ![Usernames](assets/usernames-350x52.png)

1. Set detail values by entering values in the **setEmail**, **setPassword**, and **setUsername** columns.

   ![User credentials](assets/usercredentials-350x52.png)

1. Specify Access Level values.

   For example, Chris Manning is a Team Member. Look up the ID on the **ACSLVL Access Level** sheet for the Team Member access level. Copy the ID, and on the **USER User** sheet paste it in the **setAccessLevelID** column on that user's row. 

   Repeat this step for each user and access level.

   ![Copy access level ID](assets/copyalid-350x171.png) ![Paste access elevel ID](assets/pastealid-350x59.png)

1. Enter the user's Home Group details.

   According to the scenario, Chris Manning belongs to the Marketing group. On the **GROUP Group** sheet, locate the ID for the Marketing group, copy it, and on the **USER User** sheet paste it in the **setHomeGroupID** column on the user's row. ​Repeat this step for each user and group assignment.

   ![Copy group ID](assets/copygroupid-1-350x133.png) ![Paste group ID](assets/pastegroupid-350x59.png)

1. Enter the user's Company details.

   All of the users in this scenario belong to the same company. On the **CMPY Company** sheet, locate the ID for the **Your Own Company** company, copy the ID, and on the **USER User** tab, paste this value into each row of the **setCompanyID** column.​

   Repeat this step for each user and group assignment.

   ![Company ID](assets/companyid--1--350x78.png) ![Paste company ID](assets/pastecompanyid-350x84.png)

1. Enter the user's Job Role details.

   According to the scenario, Chris Manning will have the Business Analyst role. On the **ROLE Role** sheet, locate the ID for the Business Analyst role, copy it, and on the **USER User** sheet paste it in the **setRoleID** column on the user's row. ​Repeat this step for each user and group assignment.

   ![Copy role ID](assets/copyroleid-350x149.png) ![Paste role ID](assets/pasteroleid-350x95.png)

1. Fill in other user details, as needed, then save the file.
1. Import the Excel File.

   Follow the directions provided in [Import data into Adobe Workfront using a Kick-Start template](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

>[!NOTE]
>
>Users imported to Workfront are created in a Deactivated and Pending Approval status. 
> 
>If your organization has been migrated to the Adobe Admin Console, and a user does not move out of Deactivated and Pending Approval status within a few minutes, you can add the batch of users to the Adobe Admin Console directly.
>
>For instructions, see [Manage multiple users | Bulk CSV upload](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) in the Adobe documentation.
