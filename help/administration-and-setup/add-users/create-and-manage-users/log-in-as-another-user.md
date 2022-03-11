---
filename: log-in-as-another-user
title: Log in as another user
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Log in as another user
description: The procedure described on this page applies only to organizations that have not yet been onboarded to the Adobe Admin Console. If your organization has been onboarded to the Adobe Admin Console, this action is not available.
---

# Log in as another user

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Adobe Admin Console. If your organization has been onboarded to the Adobe Admin Console, this action is not available.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

As the Adobe Workfront administrator, sometimes you might need to access Workfront on behalf of another user.

Or, as a group administrator, you might need to access Workfront on behalf of a user who is a member of a group you manage.

For example, if a task can’t progress until a user on vacation performs a certain action, you can log in as that user and perform the action instead.

<!--
Note: Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user’s groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see Access in Configure My Settings. [Add a note about this being only for the Enterprise package if they decide to do it that way]
-->

>[!NOTE]
>
>Since a document integration may connect to private personal files, administrators can't access document integrations while logged in as another user.
>
>For more information on document integrations, see [Configure document integrations](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

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
   <td> <p>With the System Administrator access level, you can log in as anyone. For information about this level of access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> <p>With a Planner access level, you can log in as a user with a lower license level if the <b>Users</b> setting in the access level is configured to <b>Edit</b> access, with <b>Create</b> and at least 1 of the 2 <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Note: Of these 2 options, if User <b>Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Log in and perform actions as another user

<ol> 
 <li value="1"> <p>Log in to Workfront as a Workfront administrator or a group administrator.</p> <note type="note"> 
   <ul> 
    <li> <p>If you are a group administrator, you can log in only as users in the groups you manage. Also, the User Admin (Group Users) permission must be enabled in your access level:</p> <p> <img src="assets/group-admin-user-350x165.png" style="width: 350;height: 165;"> </p> <p>This setting is disabled by default. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
    <li> <p>You cannot reset the password of a Workfront administrator.<br></p> </li> 
   </ul> 
  </note> </li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="3">In the left panel, click <span class="bold">Log in As</span>.<br></li> 
 <li value="4"> <p>In the <span class="bold">Users</span> box on the <span class="bold">Log In As</span> tab, begin typing the name of the user, then click the name when it appears in the drop-down list.</p> <p>The user must have an access level defined in Workfront. You cannot log in to the Workfront system as a user who does not have rights to log in.</p> <note type="note">
   Group administrators can log in only as the users who are members of the groups they manage. They cannot log in as a Workfront administrator.
   <br>
  </note> </li> 
 <li value="5"> <p>Click <span class="bold">Log in.</span></p> <!--
   Or [specify somewhere here that this is only for the Enterprise package if they decide on that]
  --> <!--
   If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.
  --> <!--
   The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period.
  --> <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see Event notifications.
  --> <p>When you are logged in as another user, a notification displays at the top of the screen to indicate this.</p> </li> 
 <li value="6">After you have performed the necessary actions as the user, click <span class="bold">Log Out.</span></li> 
</ol>

## Tracking and auditing activity while an administrator is logged in as another user

Workfront provides mechanisms for tracking and auditing activity that takes place while the administrator is logged in as another user.

When you log in as another user, the last login date is modified for that user to the date when the system or group administrator logs in as that user.

* [View indicators on items](#vieing-indicators-on-items) 
* [View audit information](#viewing-audit-information)

### View indicators on items

When you log in to Workfront as another user and perform an action, Workfront clearly indicates that any action you perform is made by you on behalf of the user who you are logged in as.

For example, if you comment on an item while logged in as another user, a statement indicates that the comment was made by you on behalf of the user.

### View audit information

<ol> 
 <li value="1">Log in to Workfront as a Workfront administrator or group administrator.</li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="3"> <p>Click <span class="bold">Log in As,</span> then click the <span class="bold">Access Log</span> tab.</p> <p>Any time a system or group administrator logs in to Workfront as another user, the event is logged in the audit trail. In addition, any auditable actions that take place while the administrator is logged in as another user are logged in the audit trail.</p> </li> 
 <li value="4">(Optional) You can filter the results that are displayed in the audit trail in the following ways: 
  <ul>
   <li>By user who has logged in</li>
   <li>By user who has been logged in as</li>
   <li>By date </li>
  </ul></li> 
</ol>

