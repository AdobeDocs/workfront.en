---
filename: manage-email-invitations
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Manage email invitations to new users
description: As an Adobe Workfront administrator, you can add users to Workfront and notify them that they have been added, by using email invitations.
---

# Manage email invitations to new users

As an `Adobe Workfront administrator`, you can add users to `Workfront` and notify them that they have been added, by using email invitations.

The email invitation allows new users to follow a link where they can choose a password for their `Workfront` account. They can then finish setting up their account.

To ensure the security of the new accounts, we recommend that you use email invitations for your new users, so they can choose their own password. Alternatively, you can also select a password for a new user when creating their account. For more information about adding new users to `Workfront`, see [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

You can configure the new user emails for:

* Any new user added to `Workfront`
* Users added to `Workfront` with a Requestor license

All new users see the same email when an email invitation is sent.

For information about receiving email invitations, see [Receive email invitations and create a password for Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

* [Generate email invitations](#generating-email-invitations) 
* [Configure email invitations](#configuring-email-invitations)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Generate email invitations

Email invitations are generated in the following scenarios:

<ul> 
 <li> <p> When you create a new user and you select the <span class="bold">Send an invite email to this person</span> on the <span class="bold">New User</span> form. For more information about creating new users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a>.</p> </li> 
 <li> <p>When you import multiple new users and you select the <span class="bold">Send invite emails to these people</span> option. For more information about importing several new users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a>.</p> </li> 
 <li> <p>After the users are created, you can manually generate the invitations to users who have not yet registered their account with <span>Workfront</span>, and they have not established a <span>Workfront</span> password.<br>Users who have an account created but have not yet registered their account are marked as <span class="bold">Unregistered</span> in <span>Workfront</span>.</p> <note type="note">
    If you deselect the 
   <span class="bold">Send an email invite to this person</span>&nbsp;box when you create the user, the email invitation cannot be generated manually. Resending the email invitations manually is only possible for users who have been sent the original email invitation when their account was created. For more information about creating new users, see 
   <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a>.
  </note> </li> 
</ul>

To manually generate email invitations to existing unregistered users:

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Users . 
 <li value="2"> <p>Select the user who shows the <span class="bold">Unregistered</span> label after their name.</p>  </li> 
 <li value="3"> <p>Click the More icon <img src="assets/more-icon.png">, then click <b>Remind user to register</b>.</p> <p>An email invitation is sent to the new user with a new link they can use to create their <span>Workfront</span> password.</p> </li> 
</ol>

## Configure email invitations

As a `Workfront administrator`, you can configure the message you include with the email invitations for new users.

<ol data-mc-continue="false"> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Setup . 
 <li value="2">In the list on the left, click <span class="bold">Email</span> > <span class="bold">Invitations</span>.</li> 
 <li value="3"> <p>In the <span class="bold">General Options</span> section, make any of the following modifications:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Deactivate invitation links after ... days</span> </td> 
     <td> <p>Choose the amount of time after which the email invitations no longer contain a valid link to <span>Workfront</span>. The default amount of days is 45.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Include a message and/ or term of service</span> </td> 
     <td> <p>Select this option if you want to modify the email invitation for all new users added to <span>Workfront</span>. This does not include users with a Requestor license.</p> 
      <ul> 
       <li><span class="bold">Message</span>: If you select to modify the email invitation for all new users, specify&nbsp;the text that you want to include in your email invitations as the email body.</li> 
       <li><span class="bold">Terms and Conditions</span>: If you select to modify the email invitation for all new users, specify the text that you want to include in your email invitations as the terms and conditions.<br></li> 
       <li><span class="bold">Include a message and/or term of service for helpdesk users</span>:&nbsp;Select this option if you want to modify the email invitation for all new users added to <span>Workfront</span>&nbsp;that have a Requestor license.</li> 
       <li><span class="bold">Message</span>: If you select to modify the email invitation for all new users with a Requestor license, specify the text that you want to include in your email invitations as the email body.</li> 
       <li><span class="bold">Terms and Conditions</span>: If you select to modify the email invitation for all new users with a Requestor license, specify&nbsp;the text that you want to include in your email invitations as the terms and conditions.<br></li> 
       <li> <p>In the <span class="bold">Invitation Preview</span> section, you can see a preview of your email invitation. If you selected to include a customized message in your email invitation, the customized message shows in this area.</p>  </li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">Click <span class="bold">Save</span>.</li> 
</ol>

