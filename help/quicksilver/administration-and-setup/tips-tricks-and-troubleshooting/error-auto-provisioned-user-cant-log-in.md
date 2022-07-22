---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error: Auto-provisioned user can't log in"
description: If an auto-provisioned user tries to log in for the first time and receives an error saying that the system is not assigning them an access level, this might be because your system lacks access levels that are associated with the Request license. Auto-provisioning uses the Request license type, so you can fix this problem by creating an access level that is associated with a Request license.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Error: Auto-provisioned user can't log in

When an auto-provisioned user tries to log in for the first time, they receive the following error:

## Problem

The system is not assigning the new user an access level.

By default, auto-provisioning uses the Request license type. When no access levels with a Request license exists, the system cannot assign the user an access level. 

## Access requirements

You must have the following access to perform the steps in this article: 

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
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
