---
filename: proof-perm-profiles-in-wp
content-type: reference
product: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Proof Permissions Profiles in Workfront Proof
description: Important: This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see Proofing.
---

# Proof Permissions Profiles in *Workfront Proof*

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product *Workfront Proof*. For information on proofing inside *Adobe Workfront*, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

As a *Workfront administrator* or *Workfront Proof administrator*, you can assign a Proof Permissions Profile to a user to specify the *proofing* capabilities that user will have for all proofs in the system. For information about configuring a user's Proof Permission Profile, see [Configure a user's Proof Permission Profile in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>You can also do the following:
>
>* Grant users specific roles on individual *proofs*. For more information about *proof* roles, see&nbsp; [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>
>* Create custom profiles for users in your organization. For more information, see [Configure custom profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>

The following table displays the permissions available with each Proof Permissions Profile.

| `Own Items`  | `Other Users' Items`  | `Admin`  | `Billing`  |
|---|---|---|---|
|   | `Add`  | `View`  | `Edit`  | `Delete`  | `View`  | `Edit`  | `Delete`  | `Edit and Delete`  | `Edit`  |
| Billing Admin | ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

|
| Admin | ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

|&nbsp; |
| Supervisor | ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

|&nbsp; |&nbsp; |
| Manager | ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

| ![](assets/cleaner2.png)

|&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| Observer |&nbsp; | ![](assets/cleaner2.png)

|&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| Visitor |&nbsp; | ![](assets/cleaner2.png)

|&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| Visitor |&nbsp; | ![](assets/cleaner2.png)

|&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

Consider the following about roles and permissions:

* Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the&nbsp;account settings&nbsp;and billing of those accounts from the hub account level.
* Billing Administrators and Administrators can delete users. This can only be done in&nbsp;Account settings.
* When Billing Administrators and Administrators view *proofs* that are owned by other users in their account, they view them with the role of a Reviewer.
* Using the Read Only role, Billing Administrators and Administrators can access *proofs* in folders shared with them or in folders created by them.&nbsp;

The following sections describe each profile and the permissions associated with the profile in a standard *Workfront Proof* setup:

* [Billing Administrator](#billing-administrator) 
* [Administrator](#administrator) 
* [Supervisor](#supervisor) 
* [Manager](#manager) 
* [Observer](#observer) 
* [Visitor](#visitor) 
* [Guest](#guest)

### Billing Administrator

Billing Administrators have access to&nbsp; [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)&nbsp;and [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md), and have the following permissions:

![](assets/cleaner2.png)Can generate proofs, upload files, and create folders. For more information, see [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Upload Files and Web Content to Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), and [Create Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Can view, edit, and delete own *proofs* and files they create.

![](assets/cleaner2.png)Can view, edit, and delete *proofs* and files created by all users in the organization.

![](assets/cleaner2.png)Can&nbsp;delete the public&nbsp;folders of other users. For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Has edit rights on all *proofs* created in the account.

![](assets/cleaner2.png)Can be set as the Dropzone owner. For more information, see [Configure the dropzone in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Can access the billing page and edit the billing details.&nbsp;For more information, see [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Can access the&nbsp;Account Settings page and edit the account details.&nbsp;For more information, see [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).&nbsp;

![](assets/cleaner2.png)Can empty the trash. For more information, see [Restore and Empty the Trash in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Can add, edit, and delete users.

![](assets/cleaner2.png)Can create groups and add new contacts.

![](assets/cleaner2.png)Can delete contacts.&nbsp;

![](assets/cleaner2.png)Can edit *proofs* if there are no replies on them.

![](assets/no2.png)Cannot edit *proof*&nbsp;replies.&nbsp;

![](assets/no2.png)Cannot delete the private folders of other Users.&nbsp;For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

For information on Account settings, see [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

For information on Billing, see [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administrator

Administrators have access to&nbsp; [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)and have the following permissions:

![](assets/cleaner2.png)Can create proofs, upload files, and create folders. For more information, see [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Upload Files and Web Content to Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), and [Create Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Can view, edit, and delete *proofs* and files they created.

![](assets/cleaner2.png)Can view, edit, and delete *proofs* and files created by all users in the organization.

![](assets/cleaner2.png)Can&nbsp;delete the public&nbsp;folders of other Users. For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Has edit rights on all *proofs* created in the account.

![](assets/cleaner2.png)Can be set as the Dropzone owner. For more information, see [Configure the dropzone in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Can access the&nbsp;Account Settings page and edit the account details.&nbsp;For more information, see [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Can empty the&nbsp;trash. For more information, see [Restore and Empty the Trash in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).&nbsp;

![](assets/cleaner2.png)Can add, edit, and delete users.

![](assets/cleaner2.png)Can create groups and add new contacts.

![](assets/cleaner2.png)Can delete contacts.

![](assets/cleaner2.png)Can edit *proofs*&nbsp;if there are no replies on them. &nbsp;

![](assets/no2.png)Cannot edit *proof* replies.

![](assets/no2.png)Cannot delete the private&nbsp;folders of other Users.&nbsp;For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).&nbsp;

![](assets/no2.png)Cannot access the&nbsp;Billing pageor edit the billing details. For more information, see [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisor

Supervisors have the following permissions:

![](assets/cleaner2.png)Can create proofs, upload files, and create folders. For more information, see [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Upload Files and Web Content to Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), and [Create Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Can view, edit, and delete own *proofs* and files they created.

![](assets/cleaner2.png)Can view, edit, and delete *proofs* and files created by all users in the organization.

![](assets/cleaner2.png)Can&nbsp;delete the public&nbsp;folders of other Users. For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Has edit rights on all *proofs* created in the account.

![](assets/cleaner2.png)Can be set as the Dropzone owner. For more information, see [Configure the dropzone in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Can create groups and add new contacts.

![](assets/cleaner2.png)Can delete contacts.&nbsp;

![](assets/cleaner2.png)Can edit *proofs*&nbsp;&nbsp;if there are no replies on them.&nbsp;

![](assets/no2.png)Cannot edit *proof* replies.

![](assets/no2.png)Cannot delete the private&nbsp;folders&nbsp;of other Users.&nbsp;For more information, see [Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)Cannot access the&nbsp;Billing page or Account settings. For more information, see [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)&nbsp;and [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Cannot add, edit, or delete users.

![](assets/no2.png)Cannot empty the&nbsp;trash. For more information, see [Restore and Empty the Trash in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Manager

Managers have the following permissions:

![](assets/cleaner2.png)Can create proofs, upload files, and create folders. For more information, see [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Upload Files and Web Content to Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), and [Create Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Can view, edit, and delete own *proofs* and files they create or own.&nbsp;

![](assets/cleaner2.png)Can see, review, and approve *proofs* of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Can create groups and add a new contact.

![](assets/no2.png)Cannot view, edit, or delete *proofs* and files created by other users in the organization.&nbsp;

![](assets/no2.png)Cannot edit *proofs*&nbsp;or replies.&nbsp;

![](assets/no2.png)Cannot delete the private&nbsp;folders of other Users.&nbsp;For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).&nbsp;

![](assets/no2.png)Cannot delete the public&nbsp;folders of other Users.&nbsp;For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).&nbsp;

![](assets/no2.png)Cannot access the&nbsp;Billing page or Account settings. For more information, see [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)&nbsp;and [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Cannot be set as the Dropzone owner. For more information, see [Configure the dropzone in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Cannot empty the&nbsp;trash. For more information, see [Restore and Empty the Trash in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Cannot add, edit, or delete users.

![](assets/no2.png)Cannot delete contacts. &nbsp;

### Observer

Observers have the following permissions:

![](assets/cleaner2.png)Can see, review, and approve *proofs* of other users that are explicitly shared with them (Read-only&nbsp;rights to everything in a shared folder). For more information, see [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Can view files that are explicitly shared with them.&nbsp;

![](assets/cleaner2.png) Can view contacts and groups

![](assets/no2.png)Cannot&nbsp;create *proofs*, upload files, and create folders. For more information, see [Upload Files and Web Content to Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Cannot view, edit, or delete *proofs* and files created by other users in the organization.

![](assets/no2.png)Cannot edit *proofs*&nbsp;or replies.

![](assets/no2.png)Cannot delete any items created in the organization.

![](assets/no2.png)Cannot access&nbsp;the Billing page or Account settings. For more information, see [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)&nbsp;and&nbsp; [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Cannot be set as the Dropzone owner. For more information, see [Configure the dropzone in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Cannot empty the&nbsp;trash. For more information, see [Restore and Empty the Trash in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Cannot add, edit, or delete users.&nbsp;

![](assets/no2.png)Cannot create groups or add new contacts.&nbsp;

![](assets/no2.png)Cannot delete contacts.&nbsp;

>[!NOTE]
>
>Menus and functions available to Observers are limited.&nbsp;
>
>* Observers do not see the Header menu or the green New menu in their Dashboard
>* Observers do not see the following links in their Settings:&nbsp;Account settings,&nbsp;Billing 
>

### Visitor

Visitors have the following permissions:

![](assets/cleaner2.png)Can see, review, and approve *proofs* of other users that are explicitly shared with them (Read-only&nbsp;rights to everything in a shared folder). For more information, see [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Can view files that are explicitly shared with them.&nbsp;

![](assets/no2.png) Cannot view contacts and groups

![](assets/no2.png)Cannot&nbsp;create *proofs*, upload files, and create folders. For more information, see [Upload Files and Web Content to Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Cannot view, edit, or delete *proofs* and files created by other users in the organization.

![](assets/no2.png)Cannot edit *proofs*&nbsp;or replies.

![](assets/no2.png)Cannot delete any items created in the organization.

![](assets/no2.png)Cannot access&nbsp;the Billing page or Account settings. For more information, see [The Workfront Proof Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)&nbsp;and&nbsp; [Account settings in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Cannot be set as the Dropzone owner. For more information, see [Configure the dropzone in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Cannot empty the&nbsp;trash. For more information, see [Restore and Empty the Trash in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Cannot add, edit, or delete users.&nbsp;

![](assets/no2.png)Cannot create groups or add new contacts.&nbsp;

![](assets/no2.png)Cannot delete contacts.&nbsp;

>[!NOTE]
>
>Menus and functions available to Visitors are limited.&nbsp;
>
>* Visitors do not see the Header menu or the green New menu in their Dashboard
>* Visitors do not see the following links in their Settings:&nbsp;Account settings,&nbsp;Billing 
>

### Guest

The Guest profile is used to give access to *proofs* for reviewers who do not have their own *Workfront Proof* account. Guests can access *proofs* shared with them directly via their personal email notifications.

![](assets/cleaner2.png)Can view, review, and approve *proofs* that are explicitly shared with them.

![](assets/cleaner2.png)Can view files that are explicitly shared with them.

![](assets/no2.png)Cannot access the Dashboard.

![](assets/no2.png)Cannot have folders shared with them. For more information, see [Manage Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Cannot be added as Authors or Moderators to the *proofs*. For more information, see [Manage Proof Roles in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>&nbsp;Guests are not *Workfront Proof* users, so they cannot see all the *proofs* shared with them in their own Dashboard.

## Edit a user's Proof Permission Profile

Administrators and Billing Administrators can edit the permission profiles of all users in the account.&nbsp;

<ol> 
 <li value="1">To find the user to edit, do one of the following:&nbsp; 
  <ul>
   <li>Navigate to&nbsp;<span class="bold">Account Settings,&nbsp;</span>then click the&nbsp;<span class="bold">Users&nbsp;</span>tab.</li>
   <li>Go to the&nbsp;<span class="bold">Contacts&nbsp;</span>page.</li>
  </ul></li> 
 <li value="2">Click the user's name whose permissions you want to edit.<span class="bold"><br></span><img src="assets/screenshot-2018-03-30-14-16-05a-350x69.png" style="width: 350;height: 69;"></li> 
 <li value="3"> <p>Click the&nbsp;<span class="bold">Permissions profile&nbsp;</span>drop-down menu and select a new permission profile. :</p> <p> <img src="assets/screenshot-2018-03-30-14-18-03a.png" alt="Screenshot_2018-03-30_14-18-03.png"> </p> <p>Permission profiles are&nbsp;Administrator, Supervisor, Manager,&nbsp;and Observer.&nbsp;<span class="bold"><br></span></p> </li> 
 <li value="4">Click anywhere outside of the menu to save.&nbsp;</li> 
</ol>

>[!NOTE]
>
>Administrators cannot assign the Billing Administrator profile. You can find a list of Profile changes in the following logs: 
>
>* The Account activity logs 
>* The User's profile log (accessible only to that User) 
>

For more information on activity logs, see [Understanding the Workfront Proof Activity Audit Trail](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
