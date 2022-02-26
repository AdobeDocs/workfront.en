---
filename: prevent-duplicate-users
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Prevent duplicate users
description: When creating a new user in Adobe Workfront, you can no longer use an email address that is already being used by another user, even if the email address varies by case (for example, JohnDoe@example.com and johndoe@example.com). In addition, to prepare for future authentication enhancements, ensure that all users have unique email addresses in a Workfront instance.
---

# Prevent duplicate users

When creating a new user in *Adobe Workfront*, you can no longer use an email address that is already being used by another user, even if the email address varies by case (for example, JohnDoe@example.com and johndoe@example.com). In addition, to prepare for future authentication enhancements, ensure that all users have unique email addresses in a *Workfront* instance.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Walkthrough

`<iframe class="vimeo-player_0" src="assets/371505632?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>`

[View this video in full-screen mode.](https://vimeo.com/371505632/2e6938ce06)

## Create users with unique email addresses

Beginning with the 2019.4 release, when creating a new user in *Workfront*, you can no longer use an email address that is already being used by another user, even if the email address varies by case. For example, you cannot create one user with the email address of JohnDoe@example.com if another user has the email address of johndoe@example.com.

## Update email addresses of existing users in your Workfront instance

As the *Workfront administrator*, you must update existing users who have matching email addresses that differ only by case. This is required for the future enhancements described in [Enhanced Authentication overview](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

To fix duplicate email addresses within a *Workfront* instance:

<ol> 
 <li value="1">&nbsp;Examine any duplicate users and decide which user is no longer needed.
  <ol>
   <draft-comment>
    <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Workfront</em>, then click <span class="bold">Users</span>.<img src="assets/users-icon-in-main-menu.png"></li>
   </draft-comment>
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Workfront</em>, then click <span class="bold">Users</span>.<img src="assets/users-icon-in-main-menu.png"></li>
   <li value="2">In the <span class="bold">Filter</span> menu, select <span class="bold">All</span>.</li>
   <li value="3">In the <span class="bold">View</span> menu, select <span class="bold">User Login</span>.</li>
   <li value="4">In the <span class="bold">Grouping</span> menu, select <span class="bold">Nothing</span>.</li>
   <li value="5">Customize the User Login view.
    <ol>
     <li value="1">Click <span class="bold">View</span> >&nbsp;<span class="bold">Customize View</span>.</li>
     <li value="2">Replace the <span class="bold">ID</span>&nbsp;column with the <span class="bold">Email Address</span> column.</li>
     <li value="3">Rename the View and save it.</li>
    </ol></li>
   <li value="6">Create a new Grouping.
    <ol>
     <li value="1">Click <span class="bold">Grouping</span> >&nbsp;<span class="bold">New Grouping</span>.</li>
     <li value="2">Click <span class="bold">Switch to Text Mode</span> in the upper-right corner of the page.</li>
     <li value="3">Paste the following Text Mode code:</li>
    </ol><pre>group.0.linkedname=direct</pre><pre>group.0.namekey=emailAddr</pre><pre>group.0.valueexpression=LOWER({emailAddr})</pre><pre>group.0.valueformat=string</pre><pre>textmode=true</pre></li>
   <li value="7">Rename the Grouping and save it.</li>
  </ol></li> 
 <li value="2">&nbsp;Do any of the following:<br>
  <ul>
   <li><p>(Preferred method) Add a + address to the user's email address for each additional account. </p><p>Choose this option if a single user in your organization needs access to more than 1 user account. If plus addressing is not supported by your email provider you must provide a separate email account for each Workfront account.</p><p>For example, John Doe can have one user account for his daily-use account and one to use for testing purposes:&nbsp;</p>
    <ul>
     <li>johndoe@workfront.com</li>
     <li>johndoe+reviewer@workfront.com</li>
    </ul></li>
   <li><p>Change the domain to use a fake domain by appending the following text to the email address:</p><pre>.inactive</pre><p>For example,John Doe could have the following domains: (These must be unique.)</p>
    <ul>
     <li>johndoe@workfront.inactive</li>
     <li>johndoe@workfront.inactive2</li>
    </ul><p>You can no longer log in to these accounts because password resets require a valid email address. These accounts can be accessed only by using the Login As feature.</p></li>
   <li><p>Delete unneeded users</p><note type="important">
     Choose this option only for accounts that were created by mistake or for test accounts. This option is usually performed only for accounts with zero or 1 mistaken login. Accounts that have been regularly used should never be deleted.
    </note></li>
  </ul></li> 
</ol>

If you have users in a *Workfront* instance with matching email addresses that differ only by case, *Workfront* will contact you with additional information and a timeline when these need to be updated.
