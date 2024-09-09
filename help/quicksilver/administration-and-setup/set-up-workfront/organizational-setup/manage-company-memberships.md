---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Manage Company Memberships
description: In the [!UICONTROL Companies] area in Setup, you can add and remove a company's members. You can also edit their user profiles, remind them to register in [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] system.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
---
# Manage company memberships

In the [!UICONTROL Companies] area in [!UICONTROL Setup], you can add and remove a company's members. You can also edit their user profiles, remind them to register in [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] system.

For information about creating a new company, see [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td><p>Current: [!UICONTROL Team] or higher</p>
   <p>Or</p>
   <p>New: Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] license</p> </td> 
   <td><p>Current: [!UICONTROL Plan]</p>
   <p>Or</p>
   <p>New: [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations</strong> </td> 
   <td> <p>One of the following:</p> 
    <ul> 
     <li> <p>The [!UICONTROL System Administrator] access level, which allows you to edit any company in the system.</p> </li> 
     <li> <p>Administrative access to manage companies, which allows you to edit any company in the system.</p> </li> 
    </ul> <p><b>NOTE</b>:  
     <ul> 
      <li> <p>You can also manage companies associated with any group where you are assigned as a group administrator.</p> </li> 
      <li> <p>In order to add to and remove users from the [!DNL Workfront] system, you must have one of the following:</p> 
       <ul> 
        <li> <p>The [!UICONTROL System Administrator] access level.</p> </li> 
        <li> <p>In your access level, [!UICONTROL Edit] must be selected for the [!UICONTROL Users] setting. Also, for the [!UICONTROL Users] setting, under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> , the [!UICONTROL Create] option and at least one of the two [!UICONTROL User Admin] options must be enabled. </p> <p> <img src="assets/access-req-users.png"> </p> <p>If you are using the [!UICONTROL User Admin (Group Users)] option, you must be a group administrator of a group where the user is a member.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Manage company memberships

{{step-1-to-setup}}

1. Click **[!UICONTROL Companies]**.
1. Click the name of the company.
1. With the **[!UICONTROL Company Members]** section selected in the left panel, do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Add a member</td> 
      <td> <p>Click <b>[!UICONTROL Add member]</b>, then select one of these options in the drop-down menu that displays:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL New user]</b>: Add a user who has not yet been added to [!DNL Workfront].</p> <p>For information about adding users to [!DNL Workfront], see <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> and <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Add a user already, existing in the system, that you have access to edit.</p> <p><b>IMPORTANT</b>: If the user is already a member of another company, the new assignment overrides the old one. The user loses access to items shared with the previous company and gains access to items shared with this company.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: Import a users by uploading a spreadsheet import file. For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Edit members</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Select at least one user, then click the [!UICONTROL Edit] icon <img src="assets/edit-icon.png"> in the toolbar.</p> </li> 
        <li value="2"> <p>Configure the options in the <b>[!UICONTROL Edit User]</b> box that displays.</p> <p>For information about these options, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copy member</td> 
      <td> <p>You can create a company member by copying an existing one. </p> <p><b>NOTE</b>:  <p>When you create a user this way, all information is copied from the original user to the newly created user except for the following:</p> 
        <ul> 
         <li>The information in the [!UICONTROL Personal Info] section.</li> 
         <li>[!UICONTROL When I log in, show]: The default landing tab for the access level is selected in this box.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Select the user, then click the [!UICONTROL Copy] icon <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>In the <b>[!UICONTROL New User]</b> box that displays, edit the fields available for the new user.</p> <p>For information about all fields associated with a user, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
        <li value="3"> <p>Click <strong>[!UICONTROL Add This User]</strong>.</p> <p>Or</p> <p>Click <strong>[!UICONTROL Add Person User &amp; Start Another]</strong> to save the new user and add another one.</p> </li> 
       </ol> <p>This creates a new account in [!DNL Workfront] for the user.</p> <p>If you selected the option to send an invite to the user, they should receive an email where they can follow a link to create their [!DNL Workfront] password.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remove users</td> 
      <td> 
       <div> 
        <p>Select at least one user, click <b>[!UICONTROL Remove users]</b>, then select one of the following options in the drop-down menu that displays:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remove from company]</b>: Removes the user or users from the company.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: Deletes the user or users from the [!DNL Workfront] system.</p> <p><b>IMPORTANT</b>: Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Send a comment to users and to their [!UICONTROL Updates] areas</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Select at least one user, then click the [!UICONTROL Comment] icon <img src="assets/comment-icon.png"> in the toolbar.</p> </li> 
        <li value="2"> <p>Type the comment you want to send to the users and to the [!UICONTROL Updates] area of their user profiles.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Export the list of company members</td> 
      <td> <p>Click the [!UICONTROL Export] icon <img src="assets/export.png"> in the toolbar, then select the format you want for the exported file.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deactivate members in the system</td> 
      <td> <p>Select at least one user, click the [!UICONTROL More] icon <img src="assets/more-icon.png"> in the toolbar, then select <b>[!UICONTROL Deactivate]</b>.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Remind a user to register in the system</td> 
      <td> <p> In the <b>[!UICONTROL Name]</b> column, <b>[!UICONTROL Unregistered]</b> displays next to the name of each unregistered user. To remind these users to register in the system, select the users, click the [!UICONTROL More] icon <img src="assets/more-icon.png"> in the toolbar, then select <b>[!UICONTROL Remind user to register]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
