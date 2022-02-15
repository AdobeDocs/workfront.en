---
filename: set-task-issue-preferences
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
---



# Configure system-wide task and issue preferences {#configure-system-wide-task-and-issue-preferences}

As an *`Adobe Workfront administrator`*, you can configure system-wide preferences for tasks and issues. These preferences impact the way that your users create tasks and issues in *`Workfront`*.


By default, these preferences are locked and *`group administrators`* cannot modify them at the group level unless you unlock them for all groups throughout the system. For more information, see the section [Lock task and issue preferences for groups](#lock) in this article.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Configure task and issues preferences for everyone in *`Workfront`* {#configure-task-and-issues-preferences-for-everyone-in-workfront}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).  

1. In the left panel, click `Project Preferences` > `Tasks & Issues.`

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> On the page that appears</MadCap:conditionalText>`, continue with one of the 5 sections listed below to configure settings for New Task Defaults, Issues, Deletion, Actual Dates, and Access.
1.  Click `Save`.





* [New Task Defaults](#new-task-defaults) 
* [Issues](#issues) 
* [Deletion](#deletion) 
* [Actual Dates](#actual-dates) 
* [Access](#access) 




### New Task Defaults {#new-task-defaults}


<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Start Date on New Tasks</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Determines the default start date for new tasks for project managers. The start date for new tasks can either be the planned start date of the project or the day the task is created on.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Duration Type </p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Determines the relationship between the number of resources (and their allocation percent) and the duration or the total effort for the task. For more information, see <a href="_task-duration-duration-type.md" class="MCXref xref">Task Duration and Duration Types</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Revenue Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Calculates planned and actual revenue estimates for a task. When the <span class="bold">Revenue Type </span>is set to<span class="bold"> Not Billable</span>, the hours planned and the actual hours recorded do not generate a revenue estimate for the task, and the work on the task does not contribute to project-level revenue.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Cost Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Calculates planned and actual cost estimates for a task. When set to <span class="bold">No Cost</span>, the hours planned and the actual hours recorded do not generate a planned or an actual cost estimate for the task, and the work on the task does not contribute to project-level costs.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Issues {#issues}


<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Automatically update Resolvable Issue status when the status of the Resolving Object changes</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>When someone converts an issue into a project or task, both the original issue and the converted project or task become resolving objects. This setting lets you correlate the resolution of the original issue to the resolution of its resolvable object. For more information on resolving objects, see <a href="resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> <p>In order for this setting to have any effect, the option to <span class="bold">Keep the original issue and tie its resolution to the task</span> must be selected.</p> 
    <ul> 
     <li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li> 
     <li>When this setting is disabled, resolving&nbsp;object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="issue-statuses.md" class="MCXref xref">Issue statuses</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">When converting an issue to a task</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The settings in this section determine what happens during the conversion process from issue to task:</p> 
    <ul> 
     <li> <p><span class="bold">Keep the original issue and tie its resolution to the task</span>: When you are converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes. When this is deselected, the issue is deleted.</p> <p>Note:  <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
       <ul> 
        <li> <p><a href="grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
        <li> <p><a href="share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a> </p> </li> 
       </ul> </p> </li> 
     <li><span class="bold">Allow Primary Contact to have access to the task</span>: Gives the primary contact (issue creator)&nbsp;access to the task to review the task, make updates, and stay informed of its progress</li> 
     <li> <p><span class="bold">Allow these settings to be changed during conversion</span>: Allows the user who is converting the issue to change these options during the conversion of an issue to a task.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">When converting an issue to a project</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>The settings in this section determine what happens during the conversion process from issue to project:</p> 
    <ul> 
     <li> <p><span class="bold">Keep the original issue and tie its resolution to the project</span>: When you are converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project&nbsp;completes. When this is deselected, the issue is deleted. </p> <p>Note:  <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
       <ul> 
        <li> <p><a href="grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
        <li> <p><a href="share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a> </p> </li> 
       </ul> </p> </li> 
     <li><span class="bold">Allow Primary Contact to have access to the project</span>: Gives the primary contact (issue creator)&nbsp;access to the project to review the project, make updates, and stay informed of its progress.</li> 
     <li><span class="bold">Allow these settings to be changed during conversion</span>: Allows the user who is converting the issue to change the listed options during the conversion of an issue to a project.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



### Deletion {#deletion}


`Allow users to delete tasks & issues with logged hours`: Lets you determine whether you allow the deletion of tasks or issues where hours are logged. This option is selected by default.


>[!TIP] {type="tip"}
>
>`This setting also applies to deleting projects that have tasks or issues with hours logged on them. This setting does not apply to deleting projects where time is logged directly for the project.` 





*  When it is selected, you receive an informational warning when you delete a task or issue. The warning reminds you that if the task or issue has logged hours, they will either be moved to the project or deleted. You can configure whether the hours are deleted or moved to the project in the Timesheet & Hours Preferences area of the Setup. After you confirm that you have seen the warning, the task or issue is deleted. For more information about configuring Timesheet & Hours Preferences, see [Configure timesheet and hour preferences](timesheet-and-hour-preferences.md). 


  >[!TIP] {type="tip"}
  >
  >`When you delete a project with tasks and issues that have logged hours, the logged hours are either deleted or they are preserved according to the settings in the Timesheet & Hours Preferences area of Setup. The warning message does not display when deleting a project`. 



* `When you deselect this option, you receive a prohibitive warning when you delete a task or issue with logged hours` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span><span>, or when you delete a project with hours logged for its tasks or </span><span data-mc-edit-date="2021-03-23T15:49:41.0077566-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted and it will replace the first sentence with 21.2 preview" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-03-23T15:49:13.9738997-04:00">issues</span></span> </MadCap:conditionalText>` `.` The warning specifies that the administrator does not allow for tasks or issues with logged hours to be deleted. `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> The tasks, issues <span>, or projects that have hours logged for tasks and issues</span> cannot be deleted.</MadCap:conditionalText>`





### Actual Dates {#actual-dates}


<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">When a task or issue goes from "New" to "In Progress," set the Actual Start Date to</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select one of the following options for when the Actual Start Date is recorded in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> when a task or issue goes from <span class="bold">New</span> to <span class="bold">In Progress</span>:</p> 
    <ul> 
     <li><span class="bold">Now:</span> The Actual Start Date is set to the current date.</li> 
     <li><span class="bold">The Planned Start Date:</span> The Actual Start Date is set to the Planned Start Date of the task or issue.</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">When a task or issue is completed, set the Actual Completion Date to</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select one of the following options for when the Actual Completion Date is&nbsp;recorded in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> when a task or issue is completed:</p> 
    <ul> 
     <li><span class="bold">Now:</span> The Actual Completion Date is set to the current date.</li> 
     <li> <p><span class="bold">The Planned Completion Date:</span> The Actual Completion Date is set to&nbsp;the Planned Completion Date of the task or issue.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



### Access {#access}


<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">When someone is assigned to a task</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <ul> 
     <li><span class="bold">Give them ... access to a task</span>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see<a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</li> 
     <li> <p><span class="bold">Also grant them ... access to the project</span>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">When someone is assigned to an issue</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ul> 
     <li><span class="bold">Give them ... access to a task</span>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see<a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</li> 
     <li> <p><span class="bold">Also grant them ... access to the project</span>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">When someone submits a request</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> 
    <ul> 
     <li><span class="bold">Give them ... access to the issue</span>: Defines the default permission a user has on a request they submitted. For more information, see <a href="share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a>.</li> 
     <li> <p><span class="bold">People from the same company will inherit the same permissions for all requests</span>: Allows users to see requests submitted by other users from the same company as them. They have the same permissions on those requests as they have on their own submitted requests.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Lock task and issue preferences for groups {#lock-task-and-issue-preferences-for-groups}

If groups in your organization need a task or issue preference configured differently for their unique workflows, you can unlock the preference for all groups throughout the organization so that they can configure it on their own. When a preference is unlocked and the *`group administrator`* modifies it, the tasks or issues associated with the group are affected by the group-level setting for the preference instead of the system-level setting.


For information about how a *`group administrator`* configures task and issue preferences for a group, see [Configure task and issue preferences for a group](configure-task-issue-preferences-group.md).


>[!NOTE]
>
>After a *`Workfront administrator`* unlocks a preference at the system level, any *`group administrator`* can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a *`Workfront administrator`* has to configure and lock a preference for everyone in the system. For more information, see [Configure project preferences for a group](configure-project-preferences-group.md) and [Lock or unlock a project, task, or issue preference for subgroups](lock-or-unlock-a-group-preference.md).


To lock or unlock a task or issue preference so that groups can configure it



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Project Preferences` > `Tasks & Issues`.

1.  Do any of the following:

    
    
    *  If you want administrators of groups below your group to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
    *  If you want your group and all groups below it to use your configuration for a preference, make sure that it is locked (this is the default).
    
    
      >[!IMPORTANT] {type="important"}
      >
      >We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that *`group administrators`* might have made.
    
    
    
    
    

1. Click `Save`.


