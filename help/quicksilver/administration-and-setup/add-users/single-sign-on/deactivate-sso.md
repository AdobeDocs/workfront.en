---
filename: deactivate-sso
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Deactivate single sign-on in Adobe Workfront
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Deactivate single sign-on in Adobe Workfront

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

After you deactivate single sign-on (SSO) in Adobe Workfront, users need to log in using their Workfront credentials. These are the credentials the user originally set up. (If you need to change user credentials, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).)

>[!NOTE]
>
>This is not available if your organization's Workfront instance uses a custom SSO portal.>
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>or is enabled with Adobe IMS>
></MadCap:conditionalText>>
>-->
>See your network or IT administrator if you need more information.

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
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
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Deactivate SSO

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **System** > **Single Sign-On (SSO)**.

1. Scroll to the bottom of the page and disable the **Enable** option.
1. Click **Save**.

