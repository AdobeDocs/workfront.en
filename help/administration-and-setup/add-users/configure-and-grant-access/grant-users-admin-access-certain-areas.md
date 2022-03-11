

# Grant users administrative access to certain areas

As an `Adobe Workfront administrator`, you can use an access level to grant users with a `Plan` license administrative access to certain areas of the system.

>[!NOTE]
>
>This is different from giving a user full administrative access to `Workfront`, which is explained in [Grant a user full administrative access](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).​

## Access requirements

You must have the following to perform the steps in this article:

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
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Grant `Plan` users administrative access to certain areas of `Workfront`

>[!IMPORTANT]
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users. To customize an access level, copy the default access level and modify the copy. (You can do this for every access level except for System Administrator and External User.)

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Access Levels</span>.</li> 
 <li value="3">Click the name of the access level you want to use to grant users administrative access to certain areas of <span>Workfront</span>.</li> 
 <li value="4"> <p>In the <span class="bold">Allow administrative access for</span> section, check boxes to grant the necessary administrative access.</p> <p>These options allow you to grant the following capabilities:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Approval Processes</td> 
     <td>Create and manage approval processes for use throughout the system and for specific groups.<br><p>Without this access, users can create only ad-hoc approval processes on items they have access to manage.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Companies</td> 
     <td>Add new and edit existing companies in <span>Workfront</span>.<br><p>Without this access, users can only view existing companies.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Custom forms</td> 
     <td>Create and edit (add, edit, and delete the fields) custom forms within their group.<br><p>Without this access, users can only attach existing forms to objects where they have access to contribute or manage.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Exchange rates</td> 
     <td> <p>Add new currency in <span>Workfront</span>.</p> <p>Without this access, the user can only add an existing currency to a project they create.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Expenses</td> 
     <td>View all expenses on objects in <span>Workfront</span>.<br><p>This does not allow the user to create new Expense Types.<br></p><p>Without this access, the user can only view the following:</p>
      <ul>
       <li>Expenses on projects, tasks or issues they manage</li>
       <li>Their own expenses</li>
       <li>The expenses of their subordinates</li>
      </ul></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Job roles</td> 
     <td> <p>With this access, the user is allowed to do the following:</p> 
      <ul> 
       <li>View and edit existing job roles</li> 
       <li>Add new job roles</li> 
       <li>Edit role billing and cost rates</li> 
      </ul> <note type="important">
       If you grant a Planner user administrative access to job roles, the Financial Data access setting Edit Role Billing & Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Planner user, job roles are still visible to the user because the Edit Role Billing & Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing & Cost Rates permission setting. For instructions, see 
       <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Milestones in my group</td> 
     <td>View all the milestone paths in the system under the Milestone Paths menu in Setup. Users can also edit or&nbsp;delete any milestone paths belonging to any of their&nbsp;groups. Users&nbsp;cannot manage (edit or delete) the milestone paths that are not assigned to any of their of groups.<br><p>Without this access, users can only view existing milestone paths and apply them to projects they have access to manage.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Reminder notifications</td> 
     <td>Create and manage reminder notifications in <span>Workfront</span>.<br>Without this access, users are limited to receiving and viewing notifications.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Timesheets & hours</td> 
     <td> <p>Allows users to view to all hours and timesheets in <span>Workfront</span>.</p> <p>When this option is disabled, users can view only hours on:</p> 
      <ul> 
       <li>Projects, tasks, or issues they manage</li> 
       <li>Their own timesheet</li> 
       <li>A timesheet of someone that reports to them</li> 
       <li>A timesheet that they approve</li> 
      </ul> <note type="note"> 
       <p>Whether this option is enabled or disabled, <span>group administrators</span> can create timesheet profiles for the groups and subgroups they manage> and assign them to group members whose user profiles they have access to edit.</p> 
       <p>Enabling this option might provide too much access for some <span>group administrators</span> because they can view the timesheets generated by timesheet profiles (and the hours) for all users in the system, not only for those in the groups they administer. You can disable this option for <span>group administrators</span> who don’t need this much access.</p> 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">When you are finished, click Save.</li> 
 <li value="6"> <p>Assign the new access level to a user, as described in <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a>.</p> <note type="note">
    You can allow users to have administrative access to users. For more information about giving users administrative access to users so they can manage user accounts, see 
   <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.
  </note> </li> 
</ol>

