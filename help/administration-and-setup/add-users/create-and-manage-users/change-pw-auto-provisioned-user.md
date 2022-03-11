---
filename: change-pw-auto-provisioned-user
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Change the password for an auto-provisioned user
description: When you create users through auto provisioning, Adobe Workfront assigns them a GUID (Globally Unique Identifier) for a user name. A GUID is a unique string of random numbers and letters, for example, 5489cb430012526e1ea635e8c29f377f.
---

# Change the password for an auto-provisioned user

When you create users through auto provisioning, Adobe Workfront assigns them a GUID (Globally Unique Identifier) for a user name. A GUID is a unique string of random numbers and letters, for example, *5489cb430012526e1ea635e8c29f377f*.

Often, when a new user attempts to change their temporary password, they enter their email address for their user name and receive an error for an incorrect user name. In order for the user to change their password, they must enter their system-assigned user name, which is a GUID.

Because GUID user names can be difficult to use, we recommend you first change a user's user name to their Workfront mail address, then allow them to change their password.

>[!NOTE]
>
>The only way to find a user's GUID is through a query of the Workfront API.

##  

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

## Change the password for an auto-provisioned user

<ol> 
 <li value="1"> <p>Determine a user's GUID user name by passing an API request, as shown in the following example:</p><pre><a href="https://domain.my.workfront.com/attask/api/v10/USER/search?fields=Username&ID=">https://<domain>.my.workfront.com/attask/api/v14.0/USER/search?fields=username&ID=<ID of User></a></pre> <p>Where <i><domain></i> is your company's domain and <i><ID of User></i> is the user's Workfront ID. </p> <p>You receive a response similar to the following:</p> <p> <img src="assets/getguid-350x105.png" style="width: 350;height: 105;"> </p> <p>The return for "username" is the user's GUID.</p> </li> 
 <li value="2"> <p>Using their GUID as their user name, change the user's password.</p> <p>For more information on changing your password, see <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Reset your password</a>.</p> <p>If your organization uses a SSO system, only a Workfront system administrator can change a user's password. For more information, see <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overview of single sign-on in Adobe Workfront</a></p> </li> 
 <li value="3"> <p>With the user logged in to Workfront, navigate to:</p> <p>https://<your domain>.my.workfront.com/login/convertUsername</p> </li> 
 <li value="4"> <p>In the <span class="bold">Your login email address</span> box, verify that user's email address is correct, then click <span class="bold">Update Account</span>.</p> <p> <img src="assets/guidusername-350x272.png" style="width: 350;height: 272;"> </p> <p>The user's user name is changed to their Workfront email address.</p> </li> 
</ol>

` `**Tip: **`` To find a user's ID:

1. Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Users . `<li value="2"> <p>Select the user.</p> <p>The user's profile page opens and their user ID displays in the URL.</p> </li>`

