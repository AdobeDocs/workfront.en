---
filename: overview-of-commit-dates
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Commit Date overview
description: The Commit Date is the date by which an user assigned to task or an issue commits to complete the task or the issue. This is different than the Planned Completion Date, as it is a more realistic estimate of the completion date given only by the user in charge of the work. For information about the Planned Completion Date, see Overview of the task Planned Completion Date.
---

# Commit Date overview

The Commit Date is the date by which an user assigned to task or an issue commits to complete the task or the issue. This is different than the Planned Completion Date, as it is a more realistic estimate of the completion date given only by the user in charge of the work. For information about the Planned Completion Date, see [Overview of the task Planned Completion Date](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Commit Date overview

Consider the following when working with commit dates:

* Only tasks and issues have a Commit Date.
* Commit dates are not automatically set by *Adobe Workfront*.  
  When you create a task or issue, there is no commit date assigned to the task or issue.

* If you are assigned to a task or issue, you can set the Commit Date by doing one of the following:

  * Let *Workfront* set the Commit Date to match the existing Planned Completion Date of the task or issue by clicking Work On It, Start Issue, or Start Task on the task or issue. For information about replacing the Work On It button with a Start button, see ` [Replace the Work On It button with a Start button](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)`.
  
  * Manually set the Commit Date yourself according to when you believe the task or issue might be completed. This&nbsp;is your estimation&nbsp;and commitment, as the assignee, to the Project Manager&nbsp;that you will have the task or issue completed by a particular date.

>[!NOTE]
>
>You must be the Task&nbsp;Owner of a task to change the Commit Date. The following users cannot change the Commit Date of a task:
>
>* Project Owner
>* Project Sponsor
>* Resource Manager
>* System Administrator
>* Any other assignee on the task
>* Any other user with permissions to the task.
>
>For more information about the Task Owner, see the section [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) in the article [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Notifications and updates triggered by changing the Commit Date

When a task or issue assignee selects a Commit Date that is different than the Planned Completion Date set by the Project Owner, there are a number of notifications and updates that alert the Project Owner and other users of this change.

>[!NOTE]
>
>Changes made to the Commit Date do not automatically change the planned dates, and changes made to the planned dates do not automatically change the Commit Date.&nbsp;

Setting the Commit Date for a task or issue triggers the following changes:
`<li>  <ul>   <li> <p>The Commit Date populates in the Update Stream of the task or issue.</p> <p> <draft-comment>     <img src="assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png" style="width: 350;height: 73;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">    </draft-comment><img src="assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png" style="width: 350;height: 73;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <note type="tip">    The change of the Commit Date displays in the Updates area of the task or issue when the     <em>Workfront administrator</em> enables this update in the Updates Feeds area in&nbsp;Setup.&nbsp;For information, see     <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md" class="MCXref xref">System-tracked updates</a>.   </note> </li>  </ul> </li>` 

<ul> 
 <li> <p>The Projected Completion Date of the task or issue is set to the same date because the task now has a more accurate indication of when it is likely to be completed.<br>For more information about the Projected Completion Date, see <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Overview of the Projected Completion Date for projects, tasks, and issues</a>.</p> <p> <draft-comment>
    <img src="assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png" style="width: 350;height: 230;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png" style="width: 350;height: 230;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <br> </p> </li> 
 <li> <p>The Project Owner is notified in the notifications area and in the Updates tab of the task whether this change will impact the project timeline. </p> <p> <draft-comment>
    <img src="assets/in-product-notification-commit-date-changed-nwe-350x137.png" style="width: 350;height: 137;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/in-product-notification-commit-date-changed-nwe-350x137.png" style="width: 350;height: 137;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <note type="tip">
   The notification that the Commit Date has changed is sent to the Project&nbsp;Owner only when the 
   <em>Workfront administrator</em> enables displaying the Commit Date in the Updates Feeds area in&nbsp;Setup.&nbsp;For information, see 
   <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md" class="MCXref xref">System-tracked updates</a>.
  </note> <p>If a Project Owner does not want to accept the change, we recommend that they comment back to the user proposing a new date to ask them to change the Commit Date back to the original Planned Date, or select a new date. If a Project Owner accepts the change, they can manually adjust the Planned Completion Date to match the Commit Date offered by the user assigned to the item.</p> <p>The Project Owner can use the Commit Date to reset the Planned Completion Date. You do this by selecting the Set planned date to option in the Updates tab of the task. You must have access to manage the task and the project to accept this change.</p> <note type="note"> 
   <p>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click <span class="bold">Project Timeline</span>. This opens the Gantt Chart where you can evaluate the date changes.</p> 
   <p> <draft-comment>
     <img src="assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png" style="width: 350;height: 139;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </draft-comment><img src="assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png" style="width: 350;height: 139;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> 
  </note> </li> 
</ul>

For information about the additional functionality that is available when updating a work item, see&nbsp; [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).&nbsp;

For information about updating Commit Dates for tasks and issues, see [Update Commit Dates on tasks and issues](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Updating"></a>Update Commit Dates on tasks and issues</h2>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <span class="bold">Task Owner</span>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click <draft-comment>
<MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Work on it
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Work on it
</MadCap:conditionalText> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
in the task or issue header
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
in the task or issue header
</MadCap:conditionalText></p> <p>Or</p> <p>Click <span class="bold">Start Task</span> or <span class="bold">Start Issue</span> if the <draft-comment>
<MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Work on it
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Work on it
</MadCap:conditionalText> button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <span class="bold">Undo</span> in the lower-left corner of the screen. The Commit Date is removed. </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <span class="bold">Undo</span> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<draft-comment>
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>
</draft-comment>
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <span class="bold">This will be done by</span> date picker, and select a new Commit Date.</p>
<div> <draft-comment>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <span class="bold">Updates</span> in the left panel, then click the <span class="bold">Start a new update</span>><span class="bold">Commit Date</span></p>
<p>Or</p>
<p>Click <span class="bold">Task Details</span> or <span class="bold">Issue Details</span> in the left panel, then double click&nbsp;<span class="bold">Commit Date</span> and select a new date from calendar. </p>
</div>
</draft-comment>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <span class="bold">Updates</span> in the left panel, then click the <span class="bold">Start a new update</span>><span class="bold">Commit Date</span></p>
<p>Or</p>
<p>Click <span class="bold">Task Details</span> or <span class="bold">Issue Details</span> in the left panel, then double click&nbsp;<span class="bold">Commit Date</span> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifica" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->

## Update Commit Dates on tasks and issues

Updating the Commit Date is identical for tasks and issues.

<ol> 
 <li value="1"> <p>Go to a task or issue that you are assigned to as the <span class="bold">Task Owner</span>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li> 
 <li value="2"> <p>Click <MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Work on it
   </MadCap:conditionalText> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    in the task or issue header
   </MadCap:conditionalText></p> <p>Or</p> <p>Click <span class="bold">Start Task</span> or <span class="bold">Start Issue</span> if the <MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Work on it
   </MadCap:conditionalText> button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li> 
 <li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <span class="bold">Undo</span> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
   The option to undo your selection to start your work is not available when you click 
   <span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>. 
  </note> </li> 
 <li value="4"> <p> Expand the <span class="bold">This will be done by</span> date picker, and select a new Commit Date.</p> 
  <div> 
   <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <p>Click <span class="bold">Updates</span> in the left panel, then click the <span class="bold">Start a new update</span>><span class="bold">Commit Date</span></p> 
    <p>Or</p> 
    <p>Click <span class="bold">Task Details</span> or <span class="bold">Issue Details</span> in the left panel, then double click&nbsp;<span class="bold">Commit Date</span> and select a new date from calendar. </p> 
   </div> 
   <p>The Commit Date and the Planned Completion date are no longer the same.</p> 
   <p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p> 
   <p>The changes are saved automatically.</p> 
   <p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifica" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p> 
  </div> </li> 
</ol>

