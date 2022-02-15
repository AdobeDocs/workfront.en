---
filename: manage-a-group
user-type: administrator
product-area: system-administration;user-management
keywords: manage,group,edit,
navigation-topic: create-and-manage-groups
---



# Manage a group {#manage-a-group}

As a *`group administrator`*, you can manage a group that you administer`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  from the Groups area in Setup</MadCap:conditionalText>`. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *`Workfront administrators`* (for any group).


>[!NOTE]
>
>When you are assigned as the administrator for a group, you inherit the *`group administrator`* role for any subgroups that are below it. The only users who can manage a subgroup are the *`group administrators`* for the top group above it and any *`group administrators`* who are assigned to the subgroup.




## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
      s
     </MadCap:conditionalText> or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## Manage a group’s memberships {#manage-a-group-s-memberships}

You can add to and remove users and other groups from a group you administer. You can also assign group members as administrators for the group and manage the user profile information of group members.


For instructions, see [View and manage a group’s memberships](view-and-manage-a-groups-memberships.md).


## Manage a group’s details {#manage-a-group-s-details}

You can view and edit the Group Details page for a group or subgroup that you manage. This page includes a description of the group, the names of the Business Leader and *`group administrators`*, and an option that allows you to make the group and all of its subgroups public or private.`<MadCap:conditionalText class="preview" data-mc-conditions="">  And, if your access level allows you to manage custom forms, you can attach a custom form to a group.</MadCap:conditionalText>`


For instructions, see [View and manage a group’s details](view-and-manage-a-groups-details.md).


## Edit, copy, or delete a group`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  from its main page</MadCap:conditionalText>` {#edit-copy-or-delete-a-group-from-its-main-page}

Without leaving the main page of a group you are viewing, you can quickly edit, copy, or delete the group.



1. Click `Setup` near the upper-right corner of *`Adobe Workfront`* on the Global Navigation Bar.

1.  Click `Groups`.


   In the list of groups that displays, *`group administrators`* can see the groups they manage, as well as any subgroups of those groups. *`Adobe Workfront administrators`* can see all groups.

1.  Select the group, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the Edit  <img src="assets/edit-icon.png">, Copy  <img src="assets/copy-icon.png">, or Delete  <img src="assets/delete.png"> icon</MadCap:conditionalText>`.


   If you need information about using the box that displays, see one of the following:

    
    
    * `Edit`: [View and manage a group’s memberships](view-and-manage-a-groups-memberships.md)
    
    * `Copy`: [Create a top-level group by copying an existing group or subgroup](create-a-group.md#copying-an-existing-group-and-sub-group) in the article [Create a group](create-a-group.md)
    
    * `Delete`: [Delete a group](delete-a-group.md)
    
    
    





## Configure project, task, and issue preferences for a group {#configure-project-task-and-issue-preferences-for-a-group}

If you are a *`group administrator`* and your group needs different project, task, and issue preference settings from those that are set on the system level, you can ask the *`Workfront administrator`* to unlock a preference for all groups throughout the organization. After it is unlocked, you (and *`group administrators`* for all other groups) can configure it for the groups you manage.


For instructions, see [Configure project preferences for a group](configure-project-preferences-group.md) and ` [Configure task and issue preferences for a group](configure-task-issue-preferences-group.md)` `.`


## List, add, and configure subgroups {#list-add-and-configure-subgroups}

You can create, view, edit, copy, rename, export, and delete subgroups beneath a group you administer.


## Configure event notifications for a group {#configure-event-notifications-for-a-group}

If a *`Workfront administrator`* unlocks the ability to configure event notifications for the groups in your organization, you can configure them for a group you administer. For instructions, see [View and configure event notifications for a group](view-and-configure-event-notifications-group.md).


## Create and customize statuses for a group {#create-and-customize-statuses-for-a-group}

As a *`group administrator`*, you can create custom statuses for a top-level group that you manage. This gives your group autonomy and helps to eliminate the need for dozens of company-wide custom statuses. (A *`Workfront administrator`* can also do this, for any group.)


You can also customize system statuses for a top-level group if a *`Workfront administrator`* has configured them to allow customization.


For instructions, see [Create or edit a group status](create-or-edit-a-group-status.md).



## Work with a group’s projects {#work-with-a-group-s-projects}

In the Groups area in Setup, when you are viewing the main page of a group you administer, you can do the following with projects:



* List and work with (edit, copy, delete, and export) the projects that are associated with the group and its subgroups and that have been shared with you
*  Create a new project for the group


For instructions, see [Create and modify a group’s projects](create-and-modify-a-groups-projects.md).



## View and manage a group’s approval processes {#view-and-manage-a-group-s-approval-processes}

When you are viewing a group that you manage in the Groups area, you can view and work with the *`approval processes`* for which the administrators of the group, or one of its subgroups, have administrative access. 


For instructions, see [Group-level approval processes](create-and-modify-groups-approval-processes.md).


## View and manage a group’s layout templates {#view-and-manage-a-group-s-layout-templates}

When you are viewing a group that you manage in the Groups area, you can view and work with the *`Layout Template`* for which the administrators of the group, or one of its subgroups, have administrative access. 


For instructions, see [Create and modify a group’s layout templates](create-and-modify-a-groups-layout-templates.md).



## View and manage group members’ schedules {#view-and-manage-group-members-schedules}

A *`group administrator`* creating a schedule for a group has to specify the group whose administrators will manage the schedule. Typically, this is the group for which the schedule is being created, but it could be a different group if the *`group administrator`* manages multiple groups and specifies one of the others instead.


When you are viewing the main page of a group you manage, if the group is designated as the one whose administrators can edit a schedule, you can view and manage the schedule from the group’s page.


For instructions, see [Create and modify a group’s schedules](create-and-modify-a-groups-schedules.md).



## View and manage group members’ timesheet profiles {#view-and-manage-group-members-timesheet-profiles}

When you are viewing the main page of a group you administer, you can manage the timesheet profiles that you and the other administers of the group—or one of its subgroups—have permission to edit. For instructions, see [Create and manage a group’s timesheet profiles](create-and-modify-a-groups-timesheet-profiles.md).



## View and manage a group’s subgroup members {#view-and-manage-a-group-s-subgroup-members}

When you are viewing the main page of a group you administer, you can view and manage all of the users in the group’s subgroups. For instructions, see [View and manage subgroup members](view-and-manage-subgroup-members.md).


## View and manage a group’s teams {#view-and-manage-a-group-s-teams}

When you are viewing a group that you manage in the Groups area, you can view and work with teams associated with the group or any of its subgroups.


For instructions, see [Create and modify a group’s teams](create-and-modify-a-groups-teams.md).


## View and manage a group’s companies {#view-and-manage-a-group-s-companies}

When you are viewing a group that you manage in the Groups area, you can view and work with companies associated with the group or any of its subgroups. For instructions, see [Create and modify a group’s companies](create-and-modify-a-groups-companies.md).


## View and manage a group’s portfolios and programs {#view-and-manage-a-group-s-portfolios-and-programs}

When you are viewing a group that you manage in the Groups area, you can view and work with portfolios and programs when both of the following are true:



* They are associated with the group you are viewing or any of its subgroups
* You have permissions to view them because you created them or they were shared with you


For instructions, see [Create and modify a group’s projects](create-and-modify-a-groups-portfolios.md) and [Create, modify, and view a group’s programs](create-and-modify-a-groups-programs.md).
