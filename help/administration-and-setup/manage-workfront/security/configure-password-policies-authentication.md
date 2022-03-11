---
filename: configure-password-policies-authentication
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configure password policies for authentication
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Configure password policies for authentication

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

As an `Adobe Workfront administrator`, you can configure password policy options to customize the authentication experience to your `Workfront` system.

We recommend that you configure authentication preferences during the `Workfront` implementation and only occasionally revisit them afterward.

Improved password management capabilities are coming soon or might already be available for your organization. Use either of the following sections, depending on whether your organization has access to the new authentication experience.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure authentication (available for all customers)

Authentication options are displayed for all customers. Improved password management capabilities are coming soon or might already be available for your organization, as described in the section [Configure enhanced authentication (coming soon)](#configuring-unified-authentication) in this article.

>[!NOTE]
>
>This is not available if your organization’s `Workfront` instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

To configure authentication preferences:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Authentication</span>.</li> 
 <li value="3"> <p>Select any of the following fields to establish the authentication settings for your organization:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Force users to reset their password every <em><value></em> days</td> 
     <td>This establishes the time frame for users to reset their <span>Workfront</span> password. By default, this option is disabled. When you enable it, you can choose between 30, 60, 90, 120, 180 days. The default is 30 days.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Don't allow users to set the same password as any of their previous <em><value></em> passwords</td> 
     <td> <p>This field prohibits users from reusing passwords for a set number of resets. By default, this field is disabled. When you enable it, you can set this value to 5, 10, or 15 resets before a password can be reused.</p> <p>When this option is selected, users cannot reset their passwords more than one time in a given day</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">If an incorrect password is entered five consecutive times, lock the account for <em><value></em> minutes: </td> 
     <td> <p>Select how long a user will be locked out of <span>Workfront</span> after entering an incorrect password five consecutive times. By default, this option is enabled, and the amount of wait time is 10 minutes. You can lock accounts for 10 minutes, 30 minutes, 1 hour, 8 hours, or 24 hours. </p> <p>Manually resetting the password for the user overrides this default wait value. <br>Users can reset their own passwords when they are locked out via the login screen. For more information about how they can reset their password, if they forgot it, see <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Reset your password</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Passwords must contain at least <em><value></em> different types of characters:</td> 
     <td> <p>Determines how strong user passwords are required to be by allowing you to select the number of different types of characters required in your passwords.</p> <p>A recognizable dictionary word cannot be used as a password.<br>By default, <span>Workfront</span> requires that at least 2 of the following are present in passwords (you can also require 3 of these characters to be present for a valid password): </p> 
      <ul> 
       <li>Uppercase characters</li> 
       <li>Lowercase characters</li> 
       <li>Numbers</li> 
       <li>Symbols</li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">Click <span class="bold">Save</span>.</li> 
</ol>

## Configure enhanced authentication (coming soon)

This section describes the enhanced authentication experience, which might not yet be available for your organization. If your organization has not been migrated to the new authentication experience, you must configure the authentication settings, as described in [Configure authentication (available for all customers)](#configuring-legacy-authentication).

To configure enhanced authentication preferences:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>Click <span class="bold">System</span> > <b>Enhanced Authentication</b>.</p> </li> 
 <li value="3"> <p>In the <span class="bold">Password Length</span> box, enter the minimum number of characters required for a valid password.</p> <p><span>Workfront</span> requires at least 6 characters.</p> </li> 
 <li value="4"> <p>(Optional) In the <span class="bold">Password Requirements</span> section, select the types of characters required in user passwords.</p> <p>You can increase the strength of user passwords by requiring any or all the types of characters in the Password Requirement section. The following options are available:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Lowercase Letters</td> 
     <td>Require at least one lowercase letter</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Uppercase Letters</td> 
     <td>Require at least one uppercase letter</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Numbers</td> 
     <td>Require at least one number</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Special Characters</td> 
     <td>Require at least one special character</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

