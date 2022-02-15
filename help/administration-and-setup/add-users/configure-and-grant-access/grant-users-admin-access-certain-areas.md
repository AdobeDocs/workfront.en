


# Grant users administrative access to certain areas {#grant-users-administrative-access-to-certain-areas}

As an *`Adobe Workfront administrator`*, you can use an access level to grant users with a *`Plan`* license administrative access to certain areas of the system.


>[!NOTE]
>
>This is different from giving a user full administrative access to *`Workfront`*, which is explained in [Grant a user full administrative access](grant-a-user-full-administrative-access.md).​




## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Grant *`Plan`* users administrative access to certain areas of *`Workfront`* {#grant-plan-users-administrative-access-to-certain-areas-of-workfront}



>[!IMPORTANT] {type="important"}
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users. To customize an access level, copy the default access level and modify the copy. (You can do this for every access level except for System Administrator and External User.)
>
>
>We also recommend that you include the original name of the access level in the name of the copy. For example, at ACME company, a copy of the Planner access level might be named "ACME Planner."






1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Access Levels`.
1. Click the name of the access level you want to use to grant users administrative access to certain areas of *`Workfront`*.
1.  In the `Allow administrative access for` section, check boxes to grant the necessary administrative access.


   These options allow you to grant the following capabilities:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Approval Processes</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Create and manage approval processes for use throughout the system and for specific groups.<br><p>Without this access, users can create only ad-hoc approval processes on items they have access to manage.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Companies</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Add new and edit existing companies in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.<br><p>Without this access, users can only view existing companies.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Custom forms</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Create and edit (add, edit, and delete the fields) custom forms within their group.<br><p>Without this access, users can only attach existing forms to objects where they have access to contribute or manage.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Exchange rates</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Add new currency in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> <p>Without this access, the user can only add an existing currency to a project they create.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Expenses</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">View all expenses on objects in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.<br><p>This does not allow the user to create new Expense Types.<br></p><p>Without this access, the user can only view the following:</p>
    <ul>
     <li>Expenses on projects, tasks or issues they manage</li>
     <li>Their own expenses</li>
     <li>The expenses of their subordinates</li>
    </ul></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Job roles</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>With this access, the user is allowed to do the following:</p> 
    <ul> 
     <li>View and edit existing job roles</li> 
     <li>Add new job roles</li> 
     <li>Edit role billing and cost rates</li> 
    </ul> <p>Important: If you grant a Planner user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Planner user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Milestones in my group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">View all the milestone paths in the system under the Milestone Paths menu in Setup. Users can also edit or&nbsp;delete any milestone paths belonging to any of their&nbsp;groups. Users&nbsp;cannot manage (edit or delete) the milestone paths that are not assigned to any of their of groups.<br><p>Without this access, users can only view existing milestone paths and apply them to projects they have access to manage.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Reminder notifications</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Create and manage reminder notifications in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.<br>Without this access, users are limited to receiving and viewing notifications.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Timesheets &amp; hours</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Allows users to view to all hours and timesheets in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> <p>When this option is disabled, users can view only hours on:</p> 
    <ul> 
     <li>Projects, tasks, or issues they manage</li> 
     <li>Their own timesheet</li> 
     <li>A timesheet of someone that reports to them</li> 
     <li>A timesheet that they approve</li> 
    </ul> <p>Note:  <p>Whether this option is enabled or disabled, <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can create timesheet profiles for the groups and subgroups they manage&gt; and assign them to group members whose user profiles they have access to edit.</p> <p>Enabling this option might provide too much access for some <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> because they can view the timesheets generated by timesheet profiles (and the hours) for all users in the system, not only for those in the groups they administer. You can disable this option for <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> who don’t need this much access.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>


1. When you are finished, click **Save**.
1.  Assign the new access level to a user, as described in [Add users](add-users.md).


   >[!NOTE]
   >
   >You can allow users to have administrative access to users. For more information about giving users administrative access to users so they can manage user accounts, see [Grant access to users](grant-access-other-users.md).





