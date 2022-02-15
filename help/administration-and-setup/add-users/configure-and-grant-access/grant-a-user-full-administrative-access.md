


# Grant a user full administrative access {#grant-a-user-full-administrative-access}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Adobe Business Platform. If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.
>
>
>For instructions on granting full administrator access in the Adobe Admin Console:
>
>
>
>*  See [Create system administrators in Workfront with the Adobe Admin Console](admin-console.md#create2)
>*  See the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>*  Contact your Adobe Admin Console Administrator.
>
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



As an *`Adobe Workfront administrator`*, you can create another *`Workfront administrator`* by assigning them the System Administrator access level. A user with this access level has full administrative access to everything in *`Workfront`*, including items they did not create themselves. 


>[!NOTE]
>
>This is different from using an access level to grant users administrative access to certain areas of the system. For more information, see the following:
>
>
>
>* [Grant users administrative access to certain areas](grant-users-admin-access-certain-areas.md) 
>* [Access of a Workfront administrator vs. access of a Plan user with administrative rights](#c)in this article
>
>





##  



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="#" class="MCXref xref selected">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Grant full System Administrator access to a single user {#grant-full-system-administrator-access-to-a-single-user}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Users` ![](assets/users-icon-in-main-menu.png).   

1.  Click the name of the user to whom you want to grant administrator rights.
1. Click the More menu ![](assets/more-icon.png), then click `Edit`.  

1. On the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">Edit Person</span> box</MadCap:conditionalText>` that appears, click `Access`.

1.  In the `Access Level` drop-down list, select the `System Administrator`&nbsp;access level.  



   Depending on changes made in your system, the name of this access level might have changed.

1.  Click `Save Changes.`  



   The user now has full System Administrator rights in the system.





## Access of a *`Workfront administrator`* vs. access of a *`Plan`* user with administrative rights  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

The two tables below show the difference between the access rights of a user with a *`Workfront administrator`* access level versus those of a user with a Plan license with some administrative rights.


*`Workfront administrators`* can view all the objects in the system (regardless of who created them), create new ones, and modify or delete existing ones. They have full access to all objects in the system.


Users with a Plan license who can edit functionality in one area have full access to the functionality in that area.


>[!NOTE]
>
>Users with a Plan license who are designated as *`group administrators`* can perform some of the actions allowed for *`Workfront administrators`*. They are allowed to perform these actions only for the groups they administer, their subgroups, and the users in these groups and subgroups. For more information, see [Group administrators](group-administrators.md).





* [Access to the Setup area](#access)<![CDATA[]]>
* [Access to objects](#access2)<![CDATA[     ]]>




### Access to the Setup area {#access-to-the-setup-area}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Area/object</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">User with a Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project Preferences: Projects</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project Preferences: Tasks &amp; Issues</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project Preferences: Statuses</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project Preferences: Priorities</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project Preferences: Severities</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project Preferences: Exchange Rates</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Full access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Processes: Approvals</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Full access</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Full access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Processes: Milestone Paths</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Full access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Custom Forms</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Manage custom forms they created or custom forms shared with them.</p> <p>Attach custom forms they created or custom forms shared with them to objects they have manage or contribute permissions to.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Recycle Bin: Recently Deleted</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Users who are <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can restore projects assigned to Groups they manage, and tasks, issues, or documents associated with those projects.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Recycle Bin: Recently Restored</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Users who are <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can see the items they have recently restored.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Job Roles</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Modify but not delete existing job roles.</p> <p>Add new job roles.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Teams</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to create Teams.</p> <p>Add existing teams to users when creating or editing users.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Groups</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access to create Groups.</p> <p>Only <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can manage group membership, subgroups, and group-level statuses for the groups they manage.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Companies</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Full access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Log in As</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>If their group administrative access is enabled on their Access Level and they are designated as a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span>, they can log in as the users in the group they administer and their subgroups. They cannot log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Schedules</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to edit Schedules.</p> <p>Access to add existing schedules to other users, at the user level.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Timesheet &amp; Hours: Timesheet Profiles</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Access to assign existing Timesheet Profiles to users, at the user level.</p> <p>Users who are <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can create Timesheet Profiles for the groups they administer and their subgroups.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Timesheet &amp; Hours: Hour Types</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Access to assign Hour Types to users, at the user level.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Timesheet &amp; Hours: Preferences</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Email: Notifications: Event Notifications</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Activate/ Deactivate all</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No access</td> 
  </tr> 
  <tr style="height: 16px;" class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Email: Notifications: Reminder Notifications</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Full access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Email: Notifications: Email Templates</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to edit Email Templates.</p> <p>Access to add existing Email Templates to Reminder Notifications.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Email: Automatic Reminders</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Email: Invitations</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to edit Email Invitations.</p> <p>Access to resend email invitations to unregistered users only from the People tab.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Email: Setup</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Scorecards</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Full access</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Expense Types</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Risk Types</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Access Levels</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Full access to modify all access levels.</p> <p>The System Administrator and External User access levels cannot be modified, by default.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access to edit Access Levels.</p> <p>Assign an access level to other users which is lower or equal to theirs at the user level.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Interface: Layout Templates</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Access to assign existing Layout Templates to other users, at the user level. </p> <p>Users designated as&nbsp;<span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can create Layout Templates for groups and subgroups they manage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Interface: Update Feeds</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access to modify Update Feeds.</p> <p>Access to add fields to be tracked in the Update Feeds when editing Custom Forms.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Interface: Filters</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to create Filters in the Setup area.</p> <p>Access to create new filters in a list of objects.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Interface: Views</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access to create Views in the Setup area.</p> <p>Access to create new views in a list of objects.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Interface: Groupings</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to create Groupings in the Setup area.</p> <p>Access to create new groupings in a list of objects.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Interface: List Controls</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Documents: Cloud Providers</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to configure Cloud Providers.</p> <p>Access to link documents to and from Cloud Providers from the Documents tab, after the Cloud Providers have been integrated with <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Documents: Metadata Mapping</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Documents: SharePoint Integration</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No access to configure a SharePoint integration.</p> <p>Access to link documents to and from SharePoint from the Documents tab, after the SharePoint integration with <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> has been configured.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Documents: Custom Integration</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No access to configure a Custom Integration.</p> <p>Access to link&nbsp;documents to and from third-party providers from the Documents tab, after the third-party providers have been integrated with <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">System: Branding</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No access</td> 
  </tr> 
  <tr style="height: 16px;" class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">System: Customer Info</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr style="height: 16px;" class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">System: Single Sign-On (SSO)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No access</td> 
  </tr> 
  <tr style="height: 16px;" class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">System: Update Users for SSO</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr style="height: 16px;" class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">System: Kick-Starts</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No access</td> 
  </tr> 
  <tr style="height: 16px;" class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">System: Diagnostics</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No access</td> 
  </tr> 
  <tr style="height: 16px;" class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">System: Preferences</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">No access</td> 
  </tr> 
 </tbody> 
</table>



### Access to objects {#access-to-objects}


<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Area/object</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">User with a Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Calendars</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Manage calendars they create and calendars shared with them.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Dashboards</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Manage dashboards they create and dashboards shared with them.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Documents</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Manage documents they upload or documents shared with them.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Issues</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Manage issues they create or issues shared with them.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Portfolios</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Manage portfolios they create or portfolios shared with them. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Programs</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Manage programs they create or programs shared with them.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Manage projects they create or projects shared with them.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Reports</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Manage reports they create or reports shared with them. View, copy and edit system reports.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Tasks</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Manage tasks they create or tasks shared with the</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Templates</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Manage templates they create or templates shared with them</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Timesheets</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Full access</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Users</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Full access</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Limited access</p> <p>They cannot assign groups to users for which they are not a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> or groups that are not public.</p> <p>They cannot assign an access level to users which is higher then their own access level.</p> <p>If their group administrative access is enabled on their Access Level and they are designated as a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> on a group, they can reset the password of and log in as the users in the group they administer and their subgroups. They cannot reset the password of or log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

