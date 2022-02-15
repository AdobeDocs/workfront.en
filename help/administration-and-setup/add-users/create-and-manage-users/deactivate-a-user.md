---
filename: deactivate-a-user
title: Deactivate a user
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
---



# Deactivate a user {#deactivate-a-user}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Adobe Business Platform. If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.
>
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



Your users might leave the organization and you might need to remove them from *`Adobe Workfront`*. They should not remain active in the system because this would create confusion for other users when adding them to updates or assigning them work.


>[!IMPORTANT] {type="important"}
>
>We recommend that you deactivate users who have left the organization rather than deleting them. If a user is deleted, all history in *`Workfront`* associated with that user is lost. This includes their work assignments, their association with notes, hours, documents, and all other objects they have once created.
>
>
>Deactivating a user in *`Workfront`* removes the user's licenses to both *`Workfront`* and digital *`proofing`*. Additionally, the user can no longer be assigned work. When a user is deactivated, that user's *`Workfront`* license and *`proofing`* license become available to be used by another user; all other information in the deactivated user's profile remains as-is.
>
>
>For more information about the impact of deleting and that of deactivating users, see [Delete users](delete-a-user.md).





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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p data-mc-conditions="SnippetConditions.HIDE">Users with a <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> license can deactivate any direct reports who are not <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>. They can also deactivate themselves.<br></p> <p data-mc-conditions="SnippetConditions.HIDE">Users with a System Administrator access level can deactivate any user except for the main administrator.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings </b><img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Deactivate a user immediately {#deactivate-a-user-immediately}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Users` ![](assets/users-icon-in-main-menu.png). 

1. Select a user, then do one of the following, depending on the environment you are using:
    
    
    * In the Production environment, click `More` > `Deactivate`.
    
    * In the Preview environment, click the More icon ![](assets/more-icon.png), then click **Deactivate**.
    
    
    
1.  Click `Deactivate` in the box that appears.  





## Schedule users for deactivation {#schedule-users-for-deactivation}

As a manager, you might want to mark users for deactivation before their actual leaving your organization. For example, if you are working with a user who is contractually bound, they are in your system for a limited period of time and you know their termination date. You can schedule them to become deactivated on that date.


*`Workfront administrators`* and *`Plan`* license users can see the deactivation date in their user profile.


To schedule a user for deactivation: 



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Users` ![](assets/users-icon-in-main-menu.png). 

1.  Select the user's name.


   Or


   (Optional) Select multiple users to schedule them for deactivation in bulk.

1. Click `Edit`.
1.  In the `Resource Planning` area of the user profile box, click the `Schedule Deactivation` box to select it.  

1.  In the calendar that displays, specify the date and the time for the `Scheduled Deactivation Date`.


   >[!NOTE]
   >
   >
   >    
   >    
   >    *  In the time box, you can select only whole hour increments, not minutes.
   >    * If you select a time for the current day which has passed, *`Workfront`* will schedule the deactivation for the following day at 12:00 AM. The time selected matches the computer timezone of the user who is scheduling the deactivation. 
   >    
   >    




1.  Click `Save Changes`.  



   The user is deactivated on the selected day sometimes after the selected time. If you selected multiple users to deactivate in bulk, all selected users are deactivated on the selected day sometimes after the selected time.



We recommend that you build a report for users that you have scheduled for deactivation, to keep informed about what users are coming up to be deactivated. There is no confirmation that the deactivation happened once the users become deactivated. 


## About deactivating *`Workfront administrators`* and *`Plan`* license users {#about-deactivating-workfront-administrators-and-plan-license-users}

Before you deactivate a *`Workfront administrator`* or a user with a *`Plan`* license, it's important to check for *`Workfront`* objects and activities involving that person, then associate them with another *`Workfront administrator`* or *`Plan`* license user as necessary.


These objects and activities might include the following:



* Tasks or issues assigned to the user
* Projects owned by the user
* Reports set up to run with the access rights of the user
* Templates owned by the user
* Projects and templates on which the user was set as a resource manager
* Request queue routing rules on which the *`Workfront administrator`* or Plan license user is the Default Assignee
* Approval processes that have a stage including the user (especially if they were the only approver on the stage)
* Timesheets that list the user as an approver
* Timesheet profiles that list the user as an approver
* Proofing Automated Workflows that include the user




## Resource planning impact when you schedule a user for deactivation {#resource-planning-impact-when-you-schedule-a-user-for-deactivation}

When you schedule a user for deactivation, they no longer appear in the Resource Planner as being available for budgeting hours. If they remain part of the Resource Pools, they appear in the Resource Planner, but their availability will be set to zero hours starting with the date of their scheduled deactivation. 


The Resource Planner takes into account all the job roles of the users and Planned Completion Dates of the tasks and calculates resources accordingly. 


For more information about the Resource Planner, see [Resource Planner overview](get-started-resource-planner.md).
