---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Understanding the Workfront Migration to the Adobe Admin Console
description: Understanding Workfront Product and User Migration to the Adobe Admin Console
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
---
# Understanding the Workfront Migration to the Adobe Admin Console  

Adobe is changing how you manage your Adobe Workfront users, bringing increased productivity to you and your organization. As part of this change, Adobe is migrating your Workfront instance and users to the Adobe Admin Console. This is a necessary migration, and will not affect any reporting, approval paths, content, or assets. It will impact how you manage user access and how your users sign in.  

 

To learn how you can use the Adobe Admin Console to manage your Adobe entitlements across your entire organization, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## What is Changing? 

As part of the migration, your user management will move from within the Workfront application to the Adobe Admin Console with the following administrative roles:  

* **System administrators** are super users with privileges of all administrators. They assign all administrative roles, and manage users for the entire organization for all products.  

* **Product Profile administrators (Workfront system administrators)** manage which users in the organization get access to Workfront.  

* **Users will sign in with Adobe Identity.** After Adobe migrates existing users to the Adobe Admin Console, users will sign in to their Workfront instances using their new Adobe Identity – either an Adobe ID or Adobe Federated ID (SSO). 

* **There is no change to how you manage all other functionality** within the Workfront application itself, including management of features, user roles, workspaces, functionality, and behavior. 

>[!NOTE]
>
> A user may be a Workfront System Admin, Product Profile Admin (Workfront System Admin), and an Adobe Admin Console System Administrator, or none of the above 

## Migration Journey Timeline 

Adobe will migrate your Workfront instance to the Adobe Admin Console first, then migrate all existing users with verified email addresses. If you're a System Admin or Workfront Product Profile Admin (Workfront System Admin), you'll receive emails guiding you through the migration journey. Here's a timeline of what you can expect:  

 

Workfront Migration to Adobe Admin Console Complete 

 

System Admins will receive an email when Workfront migration to Adobe Admin Console is complete. At this time, System Admins may need to complete some required steps before user migration starts to minimize impact to Workfront users.  

If your Workfront users currently log in with SSO, you will be required tomust set up SSO on the Adobe Admin Console so your users can continue logging in with SSO. If your Workfront users do not currently utilize use SSO, but you would like to set it up on Adobe Admin Console, you can do so at this point in the migration journey. 

If you already manage other Adobe products in your Adobe Admin Console, Adobe may seek your consent to automatically migrate users to your existing console. Click the "Get Started" button in the email to navigate to the consent page. 

 

There is no change to user management at this time. Workfront Admins will continue to manage users in the Workfront Admin area, and users will continue to log in with their Workfront Identity ID or SSO until their user migration is complete. 

 

 

Schedule User Migration 

 

After your System Admin completes the prerequisites outlined in the previous section, Adobe will automatically schedule your user migration for 30 days after these prerequisites are complete, in the future and will communicate with Workfront Product Profile Admins (Workfront System Admins) to manage the user migration.  

 

Workfront Product Profile Admins (Workfront System Admins) will:  

Receive an email with their scheduled User Migration Start Date ( 30 days after these prerequisites are complete) ahead in the future 

Gain access to the designated Workfront Admin Console, where they have the option to change their migration date 

Due to the complexity of the migration, date changes are restricted to no more than 30 days beyond the scheduled date. Contact support if you require a later date.  

Receive a reminder email 1 day before the User Migration Start Date 

 

Prepare Users for Migration Day   

 

As a Workfront Product Profile Admin (Workfront System Admin), you're encouraged are responsible for to ensureing all users are prepared for migration day.  

Prepare all users for the upcoming migration to Adobe Identity by notifying them of the following:.  

As users migrate, they will receive an email from Adobe notifying them of the change to the way they log in to Workfront. Users will be invited to accept an invitation to sign in using Adobe Identity for the first time, either by signing in with an existing Adobe ID or by setting up a new one using the same email address. 

 

What to Expect on Migration Day 

 

User migration will start at midnight of the customer's hosting Workfront Datacenter.  

 

Adobe will automatically migrate Workfront Admins first. When Workfront Admins are migrated to Adobe Identity, they will be assigned the Adobe Product Profile Admin (Workfront System Admin) role. Existing roles a user may have prior to migration will not be impacted.  

 

There will be no loss of access to the product during user migration. If a user is logged in during the time their user is being migrated, there will be no impact. However, upon their next sign-in they will be required to use their Adobe Identity.  

 

As users are migrated, they will receive an email from Adobe notifying them of the change to the way they sign in to Workfront. Users will be invited to accept an invitation to sign in using Adobe Identity for the first time, either by signing in with an existing Adobe ID or by setting up a new Adobe ID using the same email address. More information on how to log in to Workfront with an Adobe ID can be found here. 

 

 

User Migration Complete 

 

Adobe will notify all System Admins and Product Profile Admins (Workfront System Admins) via email once all Admins and users are migrated. At this time, all Workfront users for that instance will sign in to Workfront using Adobe Identity. Workfront System Admins and Product Profile Admins (Workfront System Admins) may manage user access within the Adobe Admin Console. If customers are not using a form of directory synchronization within the Admin Console, they may continue to manage access to Workfront within the Workfront Application.  

 

 

Get Support 

 

For questions or concerns please follow the steps outlined in this article here in the article Contact Customer Support. 

 

 