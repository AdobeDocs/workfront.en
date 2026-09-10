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
TQID: https://experienceleague.adobe.com/rcmVwp5wZgG0cmtmUclkBUnTcOT9OaW7LDHIt373AjM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Reset a user's preferences

<!-- Audited: 12/2023 -->

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

| Preference | Status after the reset |
| --- | --- |
| Views | Reverted to the system default <p>Existing views are not deleted. You can select them again.</p> |
| Filters | Reverted to the system default <p>Existing filters are not deleted. You can select them again.</p> |
| Groupings | Reverted to the system default <p>Existing groupings are not deleted. You can select them again.</p> |
| Recent items list | Cleared |
| Favorites list | Unaffected |
| User Preferences | Reverted to the system default <p>Email notifications revert to the system defaults. The default notifications are listed in [Event notifications available in Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

## Reset user preferences

{{step-1-to-setup}}

1. Select **Log In As**.
1. Begin typing the name of the user whose preferences you want to reset, then click the name when it appears in the drop-down list.
1. Select  **Log In**.
1. In the URL field at the top of your web browser, add add `/resetUser` after `workfront`.

     >[!NOTE]
     >
     >This is case sensitive. The U must be capitalized, and the remaining characters must be lowercase. For example:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Press **Enter**.

1. To reset all user preferences, click **Reset**.

   Or

   To reset the user's left navigation to the original layout template configuration, click **Reset Left Navigation**.
