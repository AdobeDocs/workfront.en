---
filename: configure-timesheet-hour-preferences-group
user-type: administrator
product-area: system-administration;user-management
keywords: group,preferences,task,groups,issue,unlock
navigation-topic: create-and-manage-groups
---



# Configure timesheet and hour preferences for a group {#configure-timesheet-and-hour-preferences-for-a-group}

An *`Adobe Workfront administrator`* can unlock the following sections of timesheet and hour preferences at the system level so that *`group administrators`* can configure them independently for their own groups:



* General Preferences
* Pre-Populate timesheets with


If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *`Workfront administrators`* (for any group).


The following sections on the Timesheet and Hours Preferences page are configurable only at the system level and can't be unlocked for groups:



*  Logging Time 
* Project, Task or Issue Deletion Preferences


For information about how a *`Workfront administrator`* unlocks a timesheet and hour preference, see the section [Unlock timesheet and hour preferences for groups](timesheet-and-hour-preferences.md#lock) in the article [Configure timesheet and hour preferences](timesheet-and-hour-preferences.md).


>[!TIP] {type="tip"}
>
>Group-level configuration is also possible for project preferences and for task and issue preferences. For information, see [Configure project preferences for a group](configure-project-preferences-group.md) and [Configure task and issue preferences for a group](configure-task-issue-preferences-group.md).




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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## Group timesheet and hour preferences {#group-timesheet-and-hour-preferences}

Consider the following information about configuring an unlocked timesheet or hour preference for a group:



*  If you are a *`group administrator`* and you configure a timesheet or hour preference for your group, it affects people who use the group as their Home Group.
* Typically, an unlocked preference remains unlocked indefinitely. If the *`Workfront administrator`* re-locks it, the system setting takes effect again and settings for the preference made by the *`group administrators`* are lost.

*  A timesheet inherits the timesheet and hour preferences configured for the timesheet owner’s Home Group.
*  After a *`Workfront administrator`* unlocks a preference at the system level and you configure it for your group, you can then lock it to ensure that everyone in the groups below yours is using the same configuration. This is parallel to the ability that a *`Workfront administrator`* has to configure and lock a preference for everyone in the system. For more information, see [Lock or unlock a group timesheet and hour preference](lock-or-unlock-a-group-timesheet-hour-preference.md).





## Configure an unlocked timesheet or hour preference for a group {#configure-an-unlocked-timesheet-or-hour-preference-for-a-group}



>[!TIP] {type="tip"}
>
>If you are a *`Workfront administrator`*, you can bypass steps 1-4 by going to Setup > Timesheet &&nbsp;Hours > Preferences, then searching for the group’s name in the box at the top of the page.





1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1. Click the name of the group whose timesheet or hour preferences you want to configure.
1. In the left panel, click `Timesheets & Hours`.





1.  On the page that displays, in the `General Preferences` section, configure any of the following options: 


   >[!TIP] {type="tip"}
   >
   >If you hover over a preference and a tool tip displays to tell you that it is locked, you can ask your *`Workfront administrator`* to unlock it for all groups in the organization.



<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Log time for future dates</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Allows users to log time for future dates throughout the system in:</p> 
    <ul> 
     <li>Any projects, tasks, and issues where they have access to log time<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
       , regardless of project’s group
      </MadCap:conditionalText></li> 
     <li>Their timesheets as General Time</li> 
    </ul> <p>This is useful when users plan to be away from the office and want to log that time beforehand.</p> <p>Note: You cannot prevent users from logging time on tasks or issues that are closed or canceled. You can only prevent users from logging time on complete or dead projects. We recommend that you use filters in lists of tasks and issues to exclude&nbsp;the ones that have been completed or canceled from being visible to users.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Add expenses from a timesheet</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Enables users to record both time and expenses in the timesheet.</p> 
    <div data-mc-conditions="SnippetConditions-wf-groups.groups"> 
     <p>When this preference is enabled for a group and the group is set as the home group for certain users, an expense icon displays next to projects and tasks on those users' timesheets. The users can click this icon to add or edit expenses for the project or task.</p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Assign Job Roles to hour entries manually</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Allow users to manually select any Job Role assigned in their user profile or assigned to the object.</p> <p>Important:  
     <ul> 
      <li>If you disable this setting after assigning job roles to hour entries, users must adjust hours logged under various roles on the Hours tab of the project, task, or issue.</li> 
      <li>If the user does not have a job role assigned in their profile and there is a task assigned as the Task Owner in the Advanced Assignments dialog box, that job role appears when the user logs time on the task.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Restrict timesheet editing to owners and admins</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Restrict editing to timesheet owners<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
      , the group's administrators,
     </MadCap:conditionalText> and <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>. When this option is disabled, timesheets can also be edited by:</p> 
    <ul> 
     <li> <p>Users with administrative access to timesheets and hours in their access level</p> </li> 
     <li> <p>Timesheet approvers if “Can edit hours” is enabled on the timesheet</p> </li> 
     <li> <p>The manager of the timesheet owner</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Restrict hour editing to owners and admins</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Restrict editing to the user who input the hours and <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>. This setting applies to the Hours tab in a project or in an Hours report.</td> 
  </tr> 
 </tbody> 
</table>



1.  In the `Pre-Populate timesheets with`section, configure any of the following options: 

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Work that is within &lt;number of weeks&gt; of the timesheet's work range</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Defines the number of weeks before and after the date range&nbsp;of the timesheet that contains dates of tasks and issues assigned to the user. The default setting is 1 week, and you can extend this range to 4 weeks. This means that the timesheet is pre-populated with tasks and issues which have dates anywhere between four weeks before the date range of the timesheet up to four weeks after the date range of the timesheet, if you select 4 weeks for your range. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Tasks &amp; Issues that have been completed</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">If multiple resources are typically assigned to a single task, we recommend this setting. This means when one resource records time against the task and marks it as complete, the other resources assigned to the task can still find the task or the issue in their timesheet, to record their hours.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Tasks &amp; Issues that have Planned Dates in timesheet's date range</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>When selected, the timesheet includes tasks and issues that have either a Planned Start Date or Completion Date that falls within the date range of the timesheet.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"> Tasks that have Projected Dates in timesheet's date range</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>When selected, the timesheet includes tasks that have either a Projected Start Date or Completion Date that falls within the time frame of the project, even if the planned date of the issue or task falls outside of the timesheet date range.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Save`.


