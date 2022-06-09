---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Manage company memberships
description: In the Companies area in Setup, you can add and remove a company's members. You can also edit their user profiles, remind them to register in Workfront, deactivate them in Workfront, and remove them from the Workfront system.
feature: System Setup and Administration
role: Administrator
---

# Manage company memberships

In the Companies area in Setup, you can add and remove a company's members. You can also edit their user profiles, remind them to register in Workfront, deactivate them in Workfront, and remove them from the Workfront system.

For information about creating a new company, see [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Access requirements

You must have the following in order to manage companies in Workfront:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>One of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level, which allows you to edit any company in the system. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p>Administrative access to manage companies, which allows you to edit any company in the system. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </li> 
    </ul> <p><b>NOTE</b>:  
     <ul> 
      <li> <p>You can also manage companies associated with any group where you are assigned as a group administrator.</p> </li> 
      <li> <p>In order to add to and remove users from the Workfront system, you must have one of the following:</p> 
       <ul> 
        <li> <p>The System Administrator access level. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
        <li> <p>In your access level, Edit must be selected for the Users setting. Also, for the Users setting, under Fine-tune your settings <img src="assets/gear-icon-in-access-levels.png"> , the Create option and at least one of the two User Admin options must be enabled. </p> <p> <img src="assets/access-req-users.png"> </p> <p>If you are using the User Admin (Group Users) option, you must be a group administrator of a group where the user is a member.</p> </li> 
       </ul> <p>For information about the Users setting in an access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Manage company memberships

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Companies**.
1. Click the name of the company.
1. With the **Company Members** section selected in the left panel, do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Add a member</td> 
      <td> <p>Click <b>Add member</b>, then select one of these options in the drop-down menu that displays:</p> 
       <ul> 
        <li> <p><b>New user</b>: Add a user who has not yet been added to Workfront.</p> <p>For information about adding users to Workfront, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> and <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
        <li> <p><b>Existing user</b>: Add a user already, existing in the system, that you have access to edit.</p> <p><b>IMPORTANT</b>: If the user is already a member of another company, the new assignment overrides the old one. The user loses access to items shared with the previous company and gains access to items shared with this company.</p> </li> 
        <li> <p><b>Import Users</b>: Import a users by uploading a spreadsheet import file. For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Edit members</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Select at least one user, then click the Edit icon <img src="assets/edit-icon.png"> in the toolbar.</p> </li> 
        <li value="2"> <p>Configure the options in the <b>Edit User</b> box that displays.</p> <p>For information about these options, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copy member</td> 
      <td> <p>You can create a company member by copying an existing one. </p> <p><b>NOTE</b>:  <p>When you create a user this way, all information is copied from the original user to the newly created user except for the following:</p> 
        <ul> 
         <li>The information in the Personal Info section.</li> 
         <li>When I log in, show: The default landing tab for the access level is selected in this box.</li> 
         <li>Direct Reports</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Select the user, then click the Copy icon <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>In the <b>New User</b> box that displays, edit the fields available for the new user.<br></p> <p>For information about all fields associated with a user, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
        <li value="3"> <p>Click <strong>Add This User</strong>.</p> <p>Or</p> <p>Click <strong>Add Person User &amp; Start Another</strong> to save the new user and add another one.</p> </li> 
       </ol> <p>This creates a new account in Workfront for the user.</p> <p>If you selected the option to send an invite to the user, they should receive an email where they can follow a link to create their Workfront password.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remove users</td> 
      <td> 
       <div> 
        <p>Select at least one user, click <b>Remove users</b>, then select one of the following options in the drop-down menu that displays:</p> 
        <ul> 
         <li> <p><b>Remove from company</b>: Removes the user or users from the company.</p> </li> 
         <li> <p><b>Delete</b>: Deletes the user or users from the Workfront system.</p> <p><b>IMPORTANT</b>: Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Send a comment to users and to their Updates areas</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Select at least one user, then click the Comment icon <img src="assets/comment-icon.png"> in the toolbar.</p> </li> 
        <li value="2"> <p>Type the comment you want to send to the users and to the Updates area of their user profiles.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Export the list of company members</td> 
      <td> <p>Click the Export icon <img src="assets/export.png"> in the toolbar, then select the format you want for the exported file.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deactivate members in the system</td> 
      <td> <p>Select at least one user, click the More icon <img src="assets/more-icon.png"> in the toolbar, then select <b>Deactivate</b>.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Remind a user to register in the system</td> 
      <td> <p> In the <b>Name</b> column, <b>Unregistered</b> displays next to the name of each unregistered user. To remind these users to register in the system, select the users, click the More icon <img src="assets/more-icon.png"> in the toolbar, then select <b>Remind user to register</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

