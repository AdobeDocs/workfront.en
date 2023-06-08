---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Prevent duplicate users
description: When creating a new user in Adobe Workfront, you can no longer use an email address that is already being used by another user, even if the email address varies by case (for example, JohnDoe@example.com and johndoe@example.com). In addition, to prepare for future authentication enhancements, ensure that all users have unique email addresses in a Workfront instance.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
---
# Prevent duplicate users

When creating a new user in Adobe Workfront, you can no longer use an email address that is already being used by another user, even if the email address varies by case (for example, JohnDoe@example.com and johndoe@example.com). In addition, to prepare for future authentication enhancements, ensure that all users have unique email addresses in a Workfront instance.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create users with unique email addresses

Beginning with the 2019.4 release, when creating a new user in Workfront, you can no longer use an email address that is already being used by another user, even if the email address varies by case. For example, you cannot create one user with the email address of JohnDoe@example.com if another user has the email address of johndoe@example.com.

## Update email addresses of existing users in your Workfront instance

As the Workfront administrator, you must update existing users who have matching email addresses that differ only by case.
To fix duplicate email addresses within a Workfront instance:

1. Examine any duplicate users and decide which user is no longer needed.

   1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Users**. ![](assets/users-icon-in-main-menu.png)

   1. In the **Filter** menu, select **All**.
   
   1. In the **View** menu, select **User Login**.
   
   1. In the **Grouping** menu, select **Nothing**.
   
   1. Customize the User Login view.

      1. Click **View** > **Customize View**.
      
      1. Replace the **ID** column with the **Email Address** column.
      
      1. Rename the View and save it.

   1. Create a new Grouping.

      1. Click **Grouping** > **New Grouping**.
      
      1. Click **Switch to Text Mode** in the upper-right corner of the page.
      1. Paste the following Text Mode code:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   
   1. Rename the Grouping and save it.

1. Do any of the following:

   * (Preferred method) Add a + address to the user's email address for each additional account.

     Choose this option if a single user in your organization needs access to more than 1 user account. If plus addressing is not supported by your email provider you must provide a separate email account for each Workfront account.

     For example, John Doe can have one user account for his daily-use account and one to use for testing purposes: 

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Change the domain to use a fake domain by appending the following text to the email address:
     
     `.inactive`
     
     For example,John Doe could have the following domains: (These must be unique.)

     * johndoe@workfront.inactive
     * johndoe@workfront.inactive2

     You can no longer log in to these accounts because password resets require a valid email address. These accounts can be accessed only by using the Login As feature.
   
   * Delete unneeded users

     >[!IMPORTANT]
     >
     >Choose this option only for accounts that were created by mistake or for test accounts. This option is usually performed only for accounts with zero or 1 mistaken login. Accounts that have been regularly used should never be deleted.

If you have users in a Workfront instance with matching email addresses that differ only by case, Workfront will contact you with additional information and a timeline when these need to be updated.
