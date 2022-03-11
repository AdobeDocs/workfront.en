---
filename: manage-company-memberships
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Manage company memberships
description: In the Companies area in Setup, you can add and remove a company's members. You can also edit their user profiles, remind them to register in Workfront, deactivate them in Workfront, and remove them from the Workfront system.
---

# Manage company memberships

In the Companies area in Setup, you can add and remove a company's members. You can also edit their user profiles, remind them to register in Workfront, deactivate them in `Workfront`, and remove them from the `Workfront` system.

For information about creating a new company, see [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Access requirements

You must have the following in order to manage companies in `Workfront`:

<table cellspacing="0">   
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront plan*</p> </td> 
   <td><span>Team</span> or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span>Adobe Workfront</span> license*</p> </td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> Access level configurations* One of the following: The System Administrator access level, which allows you to edit any company in the system. For more information, see Grant a user full administrative access. Administrative access to manage companies, which allows you to edit any company in the system. For more information, see Grant users administrative access to certain areas. Note: You can also manage companies associated with any group where you are assigned as a group administrator. In order to add to and remove users from the Workfront system, you must have one of the following: The System Administrator access level. For information about this access level, see Grant a user full administrative access. In your access level, Edit must be selected for the Users setting. And, for the Users setting, under Fine-tune your settings , the Create option and at least one of the two User Admin options must be enabled. If you are using the User Admin (Group Users) option, you must be a group administrator of a group where the user is a member. For information about the Users setting in an access level, see Grant access to users. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your `Workfront administrator`.

## Manage company memberships

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> Click <span class="bold">Companies</span>.</li> 
 <li value="3"> <p>Click the name of the company.</p> </li> 
 <li value="4"> <p>With the <b>Company Members</b> section selected in the left panel, do any of the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> Add a member Click Add member, then select one of these options in the drop-down menu that displays: New user: Add a user who has not yet been added to Workfront. For information about adding users to Workfront, see Add users and Edit a user's profile. Existing user: Add a user already, existing in the system, that you have access to edit. Important: If the user is already a member of another company, the new assignment overrides the old one. The user loses access to items shared with the previous company and gains access to items shared with this company. Import Users: Import a users by uploading a spreadsheet import file. For more information, see Import users. 
    <tr> 
     <td role="rowheader">Edit members</td> 
     <td> 
      <ol> 
       <li value="1"> <p>Select at least one user, then click the Edit icon <img src="assets/edit-icon.png"> in the toolbar.</p> </li> 
       <li value="2"> <p>Configure the options in the <b>Edit User</b> box that displays.</p> <p>For information about these options, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
      </ol> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Remove users</td> 
     <td> 
      <div> 
       <p>Select at least one user, click <b>Remove users</b>, then select one of the following options in the drop-down menu that displays:</p> 
       <ul> 
        <li> <p><b>Remove from company</b>: Removes the user or users from the company.</p> </li> 
        <li> <p><b>Delete</b>: Deletes the user or users from the <span>Workfront</span> system.</p> <note type="important">
          Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see 
          <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate a user</a>.
         </note> </li> 
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
     <td> <p>Select at least one user, click the More icon <img src="assets/more-icon.png"> in the toolbar, then select <b>Deactivate</b>.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate a user</a>.</p> </td> 
    </tr> Remind a user to register in the system In the Name column, Unregistered displays next to the name of each unregistered user. To remind these users to register in the system, select the users, click the More icon in the toolbar, then select Remind user to register. 
   </tbody> 
  </table> </li> 
</ol>

