---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Understanding the Workfront Migration to the Adobe Admin Console
description: Understanding Workfront Product and User Migration to the Adobe Admin Console
author: Becky
feature: System Setup and Administration
role: administrator
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
---
# Understanding the Workfront Migration to the Adobe Admin Console  

Adobe is changing how you manage your Adobe Workfront users, bringing increased productivity to you and your organization. As part of this change, Adobe is migrating your Workfront instance and users to the Adobe Admin Console. This is a necessary migration, and will not affect any reporting, approval paths, content, or assets. It will impact how you manage user access and how your users sign in.  

 

To learn how you can use the Adobe Admin Console to manage your Adobe entitlements across your entire organization, see [Manage users in the Adobe Admin Console](/help/quicksilver/administratoristration-and-setup/add-users/create-and-manage-users/administrator-console.md).  

## What is Changing? 

As part of the migration, your user management will move from within the Workfront application to the Adobe Admin Console with the following administrative roles:  

* **System administrators** are super users with privileges of all administrators. They assign all administrative roles, and manage users for the entire organization for all products.  

* **Product Profile administrators (Workfront system administrators)** manage which users in the organization get access to Workfront.  

* **Users will sign in with Adobe Identity.** After Adobe migrates existing users to the Adobe Admin Console, users will sign in to their Workfront instances using their new Adobe Identity – either an Adobe ID or Adobe Federated ID (SSO). 

* **There is no change to how you manage all other functionality** within the Workfront application itself, including management of features, user roles, workspaces, functionality, and behavior. 

>[!NOTE]
>
> A user may be a Workfront System administrator, Product Profile administrator (Workfront System administrator), and an Adobe Admin Console System administrator, or none of the above 

## Migration Journey Timeline 

Adobe will migrate your Workfront instance to the Adobe Admin Console first, then migrate all existing users with verified email addresses. If you are a System administrator or Workfront Product Profile administrator (Workfront System administrator), you'll receive emails guiding you through the migration journey. Here's a timeline of what you can expect:  

### Workfront Migration to Adobe Admin Console Complete 

 System administrators will receive an email when Workfront migration to Adobe Admin Console is complete. At this time, System administrators may need to complete some required steps **before user migration starts**, to minimize impact to Workfront users.  

* **If your Workfront users currently log in with SSO**, you must set up SSO on the Adobe Admin Console so your users can continue logging in with SSO. If your Workfront users do not currently use SSO, but you would like to set it up on Adobe Admin Console, you can do so at this point in the migration journey. 
* **If you already manage other Adobe products in your Adobe Admin Console**, Adobe may seek your consent to automatically migrate users to your existing console. Click the **Get Started** button in the email to navigate to the consent page. 

 There is no change to user management at this time. Workfront administrators will continue to manage users in Workfront, and users will continue to log in with their Workfront ID or SSO until user migration is complete. 

### Schedule User Migration 

After the System administrator completes the prerequisites outlined in the previous section, Adobe will automatically schedule your user migration for 30 days after these prerequisites are complete, and will communicate with Workfront Product Profile administrators (Workfront System administrators) to manage the user migration.  

Workfront Product Profile administrators (Workfront System administrators) will:  

* Receive an email with their scheduled User Migration Start Date (about 30 days after these prerequisites are complete) 
* Gain access to the designated Workfront administrator Console, where they have the option to change their migration date 

   >[!NOTE]
   >
   >Due to the complexity of the migration, date changes are restricted to no more than 30 days beyond the scheduled date. Contact support if you require a later date.  

* Receive a reminder email 1 day before the User Migration Start Date 

### Prepare Users for Migration Day   

As a Workfront Product Profile administrator (Workfront System administrator), are responsible for ensuring all users are prepared for migration day.  

* Prepare all users for the upcoming migration to Adobe Identity by notifying them of the following:.  

   * As users migrate, they will receive an email from Adobe notifying them of the change to the way they log in to Workfront. Users will be invited to accept an invitation to sign in using Adobe Identity for the first time, either by signing in with an existing Adobe ID or by setting up a new one using the same email address. 

### What to Expect on Migration Day 

* **User migration will start at midnight of the customer's hosting Workfront Datacenter. ** 

* **Adobe will automatically migrate Workfront administrators first.** When Workfront administrators are migrated to Adobe Identity, they will be assigned the Adobe Product Profile administrator (Workfront System administrator) role. Existing roles a user may have prior to migration will not be impacted.  

  >[!NOTE]
  >
  >There will be no loss of access to the product during user migration. If a user is logged in during the time their user is being migrated, there will be no impact. However, upon their next sign-in they will be required to use their Adobe Identity.  

 

* **As users are migrated, they will receive an email from Adobe notifying them of the change to the way they sign in to Workfront.** Users will be invited to accept an invitation to sign in using Adobe Identity for the first time, either by signing in with an existing Adobe ID or by setting up a new Adobe ID using the same email address.

  For information on how to log into Workfront with an Adobe ID, see [Log in to Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud). 

### User Migration Complete 

Adobe will notify all System administrators and Product Profile administrators (Workfront System administrators) via email after all administrators and users are migrated. At this time, all Workfront users for that instance will sign in to Workfront using Adobe Identity. Workfront System administrators and Product Profile administrators (Workfront System administrators) may manage user access within the Adobe Admin Console. If customers are not using a form of directory synchronization within the administrator Console, they may continue to manage access to Workfront within the Workfront Application.  

## Get Support 

For questions or concerns please follow the steps outlined in the article [Contact Customer Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md). 

 

 