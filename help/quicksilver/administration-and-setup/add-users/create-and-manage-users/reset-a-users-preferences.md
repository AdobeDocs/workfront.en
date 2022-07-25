---
title: Reset a user's preferences
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: As an Adobe Workfront administrator, you can reset or remove the user preference settings for any user in the Workfront system. Individual users can also reset their own user preference settings.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Reset a user's preferences

As an Adobe Workfront administrator, you can reset or remove the user preference settings for any user in the Workfront system.

Individual users can also reset their own user preference settings.

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
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## About affected settings

When you reset user preferences, some preferences are reverted to the system default, and others are cleared or removed:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing Views are not deleted. You can select them again.<br></p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing Filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing Groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>

## Reset user preferences

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Select **Log In As**.
1. Begin typing the name of the user whose preferences you want to reset, then click the name when it appears in the drop-down list.
1. Select  **Log In**.
1. In the URL field at the top of your web browser, add `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >This is case sensitive. The U must be capitalized, and the remaining characters must be lowercase. For example:
   >
   >```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Press **Enter**.
1. To reset all user preferences, select **Reset**.

   Or

   To reset only custom tabs, select **Reset Tabs**.

