---
filename: import-users
title: Import users
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Import users
description: The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
---

# Import users

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

You can import users to the Adobe Workfront site by synchronizing users from network directory service (such as Active Directory or another LDAP directory), or you can import users using a spreadsheet import file.

Before you create a new user, first ensure that you have created all objects that you want to associate with the user. For example, if you have not created a schedule, you cannot assign a schedule to the new user, and the field you use to associate a schedule with the new user does not appear in the New User screen.

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
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b><img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Synchronize users from a directory service

For information about how to synchronize users to your Workfront site via LDAP, see [Configure Adobe Workfront with LDAP](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-ldap.md).

## Use a spreadsheet import file to import users

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Users . 
 <li value="2">Click the <span class="bold">New Person
   <!--
    User
   --></span> drop-down arrow, then click <span class="bold">Import People
   <!--
    Users
   --></span>.</li> 
 <li value="3"> <p>In the <span class="bold">Import People
    <!--
     Users
    --></span> box that displays, download the sample file, then update the sample file to include your own user's personal information.</p> <p>Each row includes the following fields:<br></p> 
  <ul> 
   <li><span class="bold">First Name</span> </li> 
   <li><span class="bold">Last Name</span> </li> 
   <li> <p><span class="bold">Email Address</span> </p> <p>Email addresses must be unique.<br></p> </li> 
   <li> <p><span class="bold">Access Level</span> </p> <p>Access Levels are case sensitive.<br></p> </li> 
   <li> <p><span class="bold">SSO Login ID</span> </p> <p>This field is included only if SSO is enabled in your system. You must add the Federation ID in this field for each user. When you create a user from the People tab, you can set up a password for the user if you want to allow users to log in without SSO. However, the import feature does not allow you to leave the SSO LOGIN ID blank.<br></p> </li> 
   <li> <p>Ensure that no extra spaces exist before or after a user's email address.</p> <p> <img src="assets/importing-new-users-350x211.png" alt="importing-new-users.png" style="width: 350;height: 211;"> </p> </li> 
  </ul> </li> 
 <li value="4">Save the file to a location on your workstation.</li> 
 <li value="5">Click <span class="bold">Choose File</span> in the <span class="bold">Import People
   <!--
    Users
   --></span> box.</li> 
 <li value="6">Navigate to and select the file that you saved.<br></li> 
 <li value="7"> <p>(Optional) Select the <span class="bold">Send an invite email to this person
    <!--
     user
    --></span> option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.</p> <p>Deselect this option if you want to set the password for the user.</p> </li> 
 <li value="8"> <p>Click <span class="bold">Import</span>.</p> <p>You receive a confirmation message at the top of the screen that the user was successfully imported.</p> </li> 
</ol>

