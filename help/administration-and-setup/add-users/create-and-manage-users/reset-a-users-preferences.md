---
filename: reset-a-users-preferences
title: Reset a user's preferences
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Reset a user's preferences
description: As the Adobe Workfront administrator, you can reset or remove the user preference settings for any user in the Workfront system.
---

# Reset a user's preferences

As the Adobe Workfront administrator, you can reset or remove the user preference settings for any user in the Workfront system.

Individual users can also reset their own user preference settings.

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

## About affected settings

When you reset user preferences, some preferences are reverted to the system default, and others are cleared or removed:

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Preference</span> </th> 
   <th><span class="bold">Status after the reset</span> </th> 
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
   <td> <p>Reverted to the system default</p> <p>Existing Groupings&nbsp;are not&nbsp;deleted. You can select them again.</p> </td> 
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

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"><span class="bold">Log In As</span>.</li> 
 <li value="3">Begin typing the name of the user whose preferences you want to reset, then click the name when it appears in the drop-down list.</li> 
 <li value="4">Click <span class="bold">Log In</span>.</li> 
 <li value="5"> <p>In the URL field at the top of your web browser, add the following to the end of <code>workfront.com</code> in the current URL:</p> <p><code>/resetUser</code> <br> </p> <note type="note">
   This is case sensitive. The U must be capitalized, and the remaining characters must be lowercase. For example: 
   <code>https://company_domain.my.workfront.com/resetUser</code>
   <br>
  </note> </li> 
 <li value="6"> <p>Press <span class="bold">Enter</span>.</p> </li> 
 <li value="7"> <p>To reset all user preferences, click <span class="bold">Reset</span>.</p> <p>Or</p> <p>To reset only custom tabs, click <span class="bold">Reset Tabs</span>.</p> </li> 
</ol>

