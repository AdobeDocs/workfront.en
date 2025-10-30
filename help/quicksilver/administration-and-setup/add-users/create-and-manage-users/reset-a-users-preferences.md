---
title: Reset a User's Preferences
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: As an Adobe Workfront administrator, you can reset or remove the user preference settings for any user in the Workfront system. Individual users can also reset their own user preference settings.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
---
# Reset a user's preferences

<!-- Audited: 12/2023 -->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>

As an Adobe Workfront administrator, you can reset or remove the user preference settings for any user in the Workfront system.

Individual users can also reset their own user preference settings.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## About affected settings

When you reset user preferences, some preferences are reverted to the system default, and others are cleared or removed:

<!--
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
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
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
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

<div class="preview">

| Preference | Status after the reset |
| --- | --- |
| Views | Reverted to the system default <p>Existing views are not deleted. You can select them again.</p> |
| Filters | Reverted to the system default <p>Existing filters are not deleted. You can select them again.</p> |
| Groupings | Reverted to the system default <p>Existing groupings are not deleted. You can select them again.</p> |
| Recent items list | Cleared |
| Favorites list | Unaffected |
| User Preferences | Reverted to the system default <p>Email notifications revert to the system defaults. The default notifications are listed in [Event notifications available in Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

</div>

## Reset user preferences

{{step-1-to-setup}}

1. Select **Log In As**.
1. Begin typing the name of the user whose preferences you want to reset, then click the name when it appears in the drop-down list.
1. Select  **Log In**.
1. If your organization has not been onboarded to the Adobe Unified Experience, follow this step:
   
   * In the URL field at the top of your web browser, add `/resetUser` after `workfront.com`.

     >[!NOTE]
     >
     >This is case sensitive. The U must be capitalized, and the remaining characters must be lowercase. For example:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. If your organization has been onboarded to the Adobe Unified Experience, follow this step:

   * In the URL field at the top of your web browser, add add `/resetUser` after `workfront`.

     >[!NOTE]
     >
     >This is case sensitive. The U must be capitalized, and the remaining characters must be lowercase. For example:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Press **Enter**.

1. <span class="preview">To reset all user preferences, click **Reset**.</span>

   <span class="preview">Or</span>

   <span class="preview">To reset the user's left navigation to the original layout template configuration, click **Reset Left Navigation**.</span>
