---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Add users
description: As a Workfront administrator or a user with full administrative access, you can add users in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Add users

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Create users in Workfront with the Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

You can add users in Adobe Workfront by creating individual users from scratch or by copy existing users.

For information about how to import multiple users simultaneously, see [Import users](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Access requirements

You must have the following to perform the steps in this article:

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
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisites

Before you add a user, gather the information about the user listed below and determine which information you want to associate with that user:

* What is the user's personal information? At a minimum you need the following:

   * Full name
   * A user name
   * Default password
   * Email address

  >[!NOTE]
  >
  >You can determine whether users can view other users' contact information by fine-tuning the Users View setting when specifying access levels for Workfront objects. For more information, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* What is the position of the new user within the company? Does this person have any direct reports? Who does this person report to?
* What job role does the person fill? Does this job role exist in Workfront? Is there a limit to the number of people who can fill this job role? For information about creating job roles, see [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* What access level should the user have? Does it already exist or do you need to create a new one? For more information, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* What home group should this user be in? Should the person be in more than one group? For information about groups, see [Groups overview](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* What home team should this user be in? Should the person be on more than one team? For information about teams, see [Teams overview](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* What custom information do you need to associate with this user?

  If information about users is captured in custom fields that you created, you must have a custom form ready when creating a user. For information about custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Create a user from scratch

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Users** ![](assets/users-icon-in-main-menu.png). 

1. Click **New User > New User** to add a user who has not yet been added to Workfront.

   Or

   Click **New User > Import Users** to add users by uploading a spreadsheet import file.

   If you are importing users, you don't need to continue these steps. For more information, see [Import users](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. In the **New User** box that appears, click **Show Advanced Options**, then configure the available options to enter the person's information,

   For information about these options, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Do one of the following:

   * Leave **Send an invite email to this person** enabled. If you do this, the user receives an email where they can follow a link to create their own password for Workfront. Users who do not accept the email invitation and create a Workfront password are listed as Unregistered in Workfront.
   * Disable **Send an invite email to this person**, then type a **Password** for the person and confirm it in the **Confirm Password** box. You will need to share this password with the user outside of Workfront.
 
   >[!NOTE]
   >
   >If your Workfront administrator enabled an SSO integration with Workfront, then the Only Allow &lt;SSO Configuration&gt; Authentication field is hidden if you disable the email invitation. The Federation ID or &lt;SSO Configuration&gt; Username field remains visible.
 
1. Click **Add This User**.

   Or

   Click **Add Person User & Start Another** to save the new user and add another one.

## Copy a user to create a new one

You can create a user by copying an existing user.

>[!NOTE]
>
>When you create a user this way, all information is copied from the original user to the newly created user except for the following:
>
>* The information in the Personal Info section.
>* When I log in, show: The default landing tab for the access level is selected in this box.
>* Direct Reports
>

To create new user by copying an existing one:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Users** ![](assets/users-icon-in-main-menu.png). 
1. Select the user that you want to copy, then click the Copy icon ![](assets/copy-icon.png).
1. In the **New User** box that displays, edit the fields available for the new user.

   For information about all fields associated with a user, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Click **Add This User**.

   Or

   Click **Add Person User & Start Another** to save the new user and add another one.

This creates a new account in Workfront for the user.

If you selected the option to send an invite to the user, they should receive an email where they can follow a link to create their Workfront password.
