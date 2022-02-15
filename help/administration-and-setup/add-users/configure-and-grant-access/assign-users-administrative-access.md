



# Assign users administrative access {#assign-users-administrative-access}

As a `Workfront administrator`, you can assign other users to be `Workfront administrators` by granting them the System Administrator access level.​


By default, a `Workfront administrator` has access to everything in `Workfront`.


For information on how to grant someone full administrator&nbsp;access, see the section [Grant full System Administrator access to users](grant-administrator-access.md#gr) in the article [Grant administrator access](grant-administrator-access.md).


If you want certain users to manage only certain areas of `Workfront`, you can grant them administrative access to those areas. Only users with a Plan license can be assigned administrative access.


## Grant a Planner administrative access to certain areas of `Workfront` {#grant-a-planner-administrative-access-to-certain-areas-of-workfront}



>[!IMPORTANT] {type="important"}
>
>Each of the default access levels that come with `Workfront` contain the settings that we recommend for that level. It's a good idea to leave these unchanged so that you can refer to them after you have set up your users.
>
>
>So, instead of editing a default access level that comes with `Workfront` (Planner, Requestor, Reviewer, and so on) we recommend that you copy it and then modify the copy.
>
>
>We also recommend that you keep the original name of the access level in the name that you create for the copy. For example, at `Workfront`, we might call the access level for users with a Planner license type "Workfront Planner."
>
>
>For instructions on copying an access level, see the section [Create or edit an access level](create-modify-access-levels.md#creating-new-access-from-existing-access) in the article [Create or modify access levels](create-modify-access-levels.md).






1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Click **Access Levels** in the left panel.
1. Click the name of the access level for which you want to grant access to `administrative access`.
1.  In the **Allow administrative access for** section, check boxes to grant the necessary administrative access.


   These options allow you to grant the following capabilities:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Approval Processes</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Create and manage approval processes for use throughout the system and for specific groups.<br><p>Without this access, users can create only ad-hoc approval processes on items they have access to manage.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Companies</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Add new and edit existing Companies in <span class="WFVariablesProdNameWF">Workfront</span>.<br><p>Without this access, users can only view existing Companies.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Custom forms in my group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Manage all custom forms within their group. <br><p>This allows the user to create new custom forms, as well.<br></p><p>Without this access, users can only&nbsp;attach existing forms to the objects they have access to contribute or manage.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Exchange rates</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Add new currency in <span class="WFVariablesProdNameWF">Workfront</span>.<br>Without this access, the user can only add an existing currency to a project they create.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Expenses</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">View all expenses on objects in <span class="WFVariablesProdNameWF">Workfront</span>.<br><p>This does not allow the user to create new Expense Types.<br></p><p>Without this access, the user can only view the following:</p>
    <ul>
     <li value="1">Expenses on projects, tasks or issues they manage</li>
     <li value="2">Their own expenses</li>
     <li value="3">The expenses of their subordinates</li>
    </ul></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Job roles</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>With this access, the user is allowed to do the following:</p> 
    <ul> 
     <li value="1">View and edit existing job roles</li> 
     <li value="2">Add new job roles</li> 
     <li value="3">Edit role billing and cost rates</li> 
    </ul> <p>Important: If you grant a Planner user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Planner user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Milestones in my group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">View all the milestone paths in the system under the Milestone Paths menu in Setup. Users can also edit or&nbsp;delete any milestone paths belonging to any of their&nbsp;groups. Users&nbsp;cannot manage (edit or delete) the milestone paths that are not assigned to any of their&nbsp;of groups.<br><p>Without this access, users can only view existing milestone paths and apply them to projects they have access to manage.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Reminder notifications</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Create and manage reminder&nbsp;notifications in <span class="WFVariablesProdNameWF">Workfront</span>. <br>Without this access, users are limited to receiving and viewing notifications.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Timesheets &amp; hours</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Group administrators can assign Timesheet Profiles to users in the groups and subgroups they manage.</p> <p>Without this option enabled, group administrators cannot assign Timesheet Profiles to other users in the groups and subgroups they manage, although they can create them.</p> <p>All other users with a Plan license can view all hours and timesheets in Workfront.</p> <p>Without this option enabled, all users can only view hours on:</p> 
    <ul> 
     <li value="1">Projects, tasks or issues they manage.</li> 
     <li value="2">Their own timesheet.</li> 
     <li value="3">A timesheet of someone that reports to them.</li> 
     <li value="4">A timesheet they approve.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


1. Click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <b>Save</b></MadCap:conditionalText>`.  

1.  Assign the new access level to a user, as described in [Add users](add-users.md).


   >[!NOTE]
   >
   >You can allow users to have administrative access to users. For more information about giving users administrative access to users so they can manage user accounts, see [Grant access to users](grant-access-other-users.md).





