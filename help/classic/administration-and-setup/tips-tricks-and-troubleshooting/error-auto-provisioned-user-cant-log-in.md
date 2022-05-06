---
filename: error-auto-provisioned-user-cant-log-in
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Error: Auto-provisioned user can't log in
description: When an auto-provisioned user tries to log in for the first time, the receive the following error:
---

# Error: Auto-provisioned user can't log in

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

When an auto-provisioned user tries to log in for the first time, the receive the following error:

## Problem

The system is not assigning&nbsp;the new user an access level.

By default,&nbsp;auto-provisioning uses the Request license type. When no access levels with a Request license&nbsp;exists, the system cannot assign the user an access level.&nbsp;

## Access requirements

You must have the following access to perform the steps in this article: 

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
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Create a basic access level with a Request license:

1. Go to **Setup** > **Access Levels**.

1. Click **New Access Level**.
1. Enter a **Name**.
1. In the **License Type** drop-down menu, select Request.
1. Click **Save Changes**.

After you create an access level with a Request license, have the user log in with their SSO credentials.
