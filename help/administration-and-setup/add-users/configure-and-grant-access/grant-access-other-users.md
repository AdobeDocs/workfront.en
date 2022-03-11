

# Grant access to users

As an Adobe Workfront administrator, you can use an access level to define a user’s access to other users in Workfront, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuring access to users

You can manage what information users can view and edit for other users using a default access level or a custom access level that you create. Users with the default Plan and Work licenses can view the contact information of other users. Any of the following users can create and edit other users:

* A Workfront administrator.

  For more information, see [Grant a user full administrative access](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* A user with a default Plan license who also has access to users, as explained in this article.

  Users that are restricted to see only users from their company or the primary company have access to edit only the users they can see. For more information, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* A user with a default Plan license who is also specified as the manager of another user.

  Users who are granted Edit access to users in their access level can manage users who report to them. For information about managing a user, see [View the organizational chart](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* A user with a default Plan license who created a user can deactivate, delete, or edit the user they created. For information about creating new users, see [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configure users’ access to edit users using a custom access level

<ol> 
 <li value="1">Begin creating or editing the access level, as explained in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</li> 
 <li value="2">To change the ability of users with a Plan or Work license to view the profiles of other users:
  <ol>
   <li value="1">Click the gear icon <img src="assets/gear-icon-settings.png"> on the <span class="bold">View</span> button to the right of <span class="bold">Users</span>.</li>
   <li value="2">Disable <span class="bold">View Contact info</span>, then click the X to close the <span class="bold">Fine-tune your settings</span> box.</li>
  </ol></li> 
 <li value="3"> <p>To modify the ability of users with a Plan license access to edit other users, click the gear icon <img src="assets/gear-icon-settings.png"> on the <span class="bold">Edit</span> button to the right of <span class="bold">Users</span>, then select the abilities you want to grant:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Create</span> </td> 
     <td> <p>Allows users to create users.<br>This option is enabled by default.</p> <!--
       Make sure this change is being made before undrafting these 2 notes. On 3/29, the req doc says that this depends on investigation results.
      --> <note type="note">
       This is not available if your organization’s Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Delete</span> </td> 
     <td> <p> Allows users to delete the users they have created themselves.<br>This option is enabled by default.</p> <note type="note">
       This is not available if your organization’s Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">User Admin (All Users)</span> </td> 
     <td> <p>Allows users to do the following for any user in Workfront:</p> 
      <ul> 
       <li>Edit, delete, or deactivate the user</li> 
       <li>Log in as the user</li> 
       <li>Reset the user's password</li> 
      </ul> <p>This option is disabled by default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">User Admin (Group Users)</span> </td> 
     <td> <p>Allows users to do the following for any user in a group they administer: 
       <ul>
        <li><p>Edit, delete, or deactivate the user</p></li>
        <li>Log in as the user</li>
        <li><p>Reset the user's password</p><note type="note">
           A group administrator cannot log in as or reset the password of a Workfront administrator.
          <br>
         </note></li>
       </ul><p>This option is disabled by default.</p></p> </td> 
    </tr> 
   </tbody> 
  </table> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>If you don’t want to grant group administrators access to all members of the groups they administer, disable both of the User Admin options above. Group administrators will still be able to access group members whom they add to Workfront, or who report to them in Workfront.</p> 
  </div> </li> 
 <li value="4"> <p>(Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref" data-mc-variable-override="">Configure access to Adobe Workfront</a>, such as <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref" data-mc-variable-override="">Grant access to tasks</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref" data-mc-variable-override="">Grant access to financial data</a>.</p> </li> 
 <li value="5">When you are finished, click Save.</li> 
</ol>

## Access to users by license type

For information about what users in each access level can do with users, see the section [Users](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).  

