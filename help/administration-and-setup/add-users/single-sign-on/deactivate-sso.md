---
filename: deactivate-sso
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Deactivate single sign-on in Adobe Workfront
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Deactivate single sign-on in `Adobe Workfront`

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

After you deactivate single sign-on (SSO) in `Adobe Workfront`, users need to log in using their `Workfront` credentials. These are the credentials the user originally set up. (If you need to change user credentials, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).)

>[!NOTE]
>
>This is not available if your organization’s `Workfront` instance uses a custom SSO portal>
><!-->
>or is enabled with Adobe IMS>
>-->
>. See your network or IT administrator if you need more information.

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

## Deactivate SSO

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="3">Scroll to the bottom of the page and disable the <span class="bold">Enable</span> option.</li> 
 <li value="4">Click <span class="bold">Save</span>.</li> 
</ol>

