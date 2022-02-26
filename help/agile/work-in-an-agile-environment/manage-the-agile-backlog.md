---
filename: manage-the-agile-backlog
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Manage the agile backlog
description: The following work items can be assigned to an agile team and added to that team's backlog as stories, depending on the agile methodology the team is using:
---

# Manage the agile backlog

The following work items can be assigned to an agile team and added to that team's backlog as stories, depending on the agile methodology the team is using:

* `Scrum agile teams:` Tasks and issues can be assigned to the agile team and added to the backlog.
* `Kanban agile teams:` Tasks can be assigned to the agile team and added to the backlog. Users can view the backlog directly from the agile story board, as described in [Add the backlog to the Kanban board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). The team uses this backlog to prioritize and manage their work queue.

Tasks or issues can be&nbsp;assigned to the team (and subsequently added to the team backlog) from anywhere in *Adobe Workfront*. For example, a single team might be assigned work assignments from multiple projects.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Worker or higher</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the project the story is on</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create and manage stories on the backlog

* [Reorder stories](#reordering-stories) 
* [Break down stories](#breaking-down-stories) 
* [Edit stories](#editing-stories) 
* [Create new stories on the backlog](#creating-new-stories) 
* [Move stories from the backlog to an iteration or Kanban board](#moving-stories-from-the-backlog)

### Reorder stories

You can reorder stories in the backlog list by using the drag-and-drop method.

<ol> 
 <li value="1">Go to the agile backlog where you want to reorder stories.</li> 
 <li value="2"> <p>In the <span class="bold">View</span> drop-down menu, select the <span class="bold">Backlog</span> view or a custom view that contains the <span class="bold">Order</span> column.</p> <note type="note">
   If a task or issue has an agile team assigned and the project is not in a status that equates with Current, they do not display on the backlog. However, they do still affect the backlog count in the Order column. 
   <br>
  </note> </li> 
 <li value="3">Select one or more stories, then drag the stories to the order where you want them to appear in the backlog.<br><img src="assets/agile-backlog-drag-and-drop-adobe-350x160.png" alt="Agile_backlog_drag-and-drop.png_Adobe" style="width: 350;height: 160;"></li> 
</ol>

### Break down stories

Because stories in a backlog vary in size, users can break them down into workable sizes&nbsp;for an iteration. Breaking a story down creates subtasks on the task that the story represents, and replaces the original task in the backlog. You can have a parent task or its subtasks assigned to an agile team, but you cannot have both assigned to a team simultaneously.

>[!NOTE]
>
>Consider the following limitations when breaking down stories: >
>* Only stories that represent tasks can be broken down. You cannot break down stories that represent issues.
>* Stories can be broken down only if they are associated with a project.
>

To break down a story:

<ol> 
 <li value="1">Go to the backlog that contains the story you want to break down.</li> 
 <li value="2">Select the story you want to break down, then click <span class="bold">Breakdown Story</span>.<br>The Breakdown Story dialog box is displayed.<br><img src="assets/backlog-breakdown-dialog-350x171.png" alt="backlog_breakdown_dialog.png" style="width: 350;height: 171;"></li> 
 <li value="3">Specify a name and estimate for the story, and select whether the story is ready.</li> 
 <li value="4">Click <span class="bold">Add Story</span> to create another story from the original story.</li> 
 <li value="5">Click <span class="bold">Save</span>.&nbsp;</li> 
</ol>

### Edit stories

You can edit stories directly from the Stories or Issues tabs on the Backlog as you would edit any tasks or issues within a project in bulk, as described in [Edit tasks in bulk](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) in [Edit tasks](../../manage-work/tasks/manage-tasks/edit-tasks.md) and&nbsp; [Edit issues](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) in [Edit issues](../../manage-work/issues/manage-issues/edit-issues.md).

## Create new stories on the backlog

You can create new stories on the backlog by creating the story&nbsp;directly from the backlog, or by assigning an existing&nbsp;task or issue to an agile team.

* [Create a story from the backlog](#creating-a-story-from-the-backlog) 
* [Assign a task or issue to an agile team](#assigning-a-task-to-an-agile-team)

### Create a story from the backlog

When you create a story from the backlog, the story is created as a task or issue within a project. You cannot create a story from the backlog as an issue.&nbsp;

To create a story from the backlog:

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Teams</span>.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Teams</span>.</li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <span class="bold">Switch team</span> icon <img src="assets/switch-team-icon.png" alt="Switch team icon">, then either select a new Scrum team from the drop-down menu or search for a team in the search bar.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <span class="bold">Switch team</span> icon <img src="assets/switch-team-icon.png" alt="Switch team icon">, then either select a new Scrum team from the drop-down menu or search for a team in the search bar.</li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select <span class="bold">Backlog</span> from the left panel.</li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select <span class="bold">Backlog</span> from the left panel.</li> 
 <li value="4">Do either of the following, depending on whether you want to create a task or an issue: 
  <ul>
   <li><span class="bold">To create a task:</span> Click the <span class="bold">Stories</span> tab.</li>
   <li><span class="bold">To Create an issue:</span> Click the <span class="bold">Issues</span> tab.</li>
  </ul></li> 
 <li value="5">Click <span class="bold">New Story</span> or <span class="bold">New Issue</span>.</li> 
 <li value="6">Specify the following information:<br>
  <table cellspacing="0">
   <col>
   <col>
   <tbody>
    <tr>
     <td role="rowheader"><span class="bold">Story Name:</span></td>
     <td> Type a name for the story.</td>
    </tr>
    <tr>
     <td role="rowheader"><span class="bold">Description:</span></td>
     <td>(Optional) Type a description for the story.</td>
    </tr>
    <tr>
     <td role="rowheader"><span class="bold">Ready:</span></td>
     <td> Select whether the story is ready to be added to an iteration. This setting is informational only. Stories can be added to an iteration regardless of the status of this setting.</td>
    </tr>
    <tr>
     <td role="rowheader"><span class="bold">Estimate:</span></td>
     <td>Specify a point or hourly estimate for the story. Estimates affect the burndown chart. The burndown&nbsp;chart for an iteration is accurate only if each story contains an accurate estimate.&nbsp;(If you provide a point estimate, you must have already designated in the team settings how many hours each point represents.)</td>
    </tr>
    <tr>
     <td role="rowheader"><span class="bold">Parent Project:</span></td>
     <td>Begin typing the name of the project where this story will be created, then click the name when it appears in the drop-down list.<br>The status of the project must be set to Current. If the status of the project is anything but Current, it is not displayed in the drop-down menu.</td>
    </tr>
    <tr>
     <td role="rowheader"><span class="bold">Parent Task:</span></td>
     <td>(Optional) Begin typing the name of the parent task that this story is subordinate to, then click the name when it appears in the drop-down list.</td>
    </tr>
    <tr>
     <td role="rowheader"><span class="bold">Custom Forms:</span></td>
     <td> (Optional) Select any custom forms that you want to add to this story.</td>
    </tr>
   </tbody>
  </table></li> 
 <li value="7">Click <span class="bold">Save Story</span>.</li> 
</ol>

### `Assign a task or issue to an agile team`

You can assign a task or issue to an agile team. After it is assigned, the task or issue appears as a new story on the team backlog.

To assign a task or issue to an agile team:

1. Go to the Project that contains the task that you want to re-assign. 
1. Select the task or issue in the list. 
1. Click `Edit`. 
1. Click `Assignments`. 
1. (Optional) Delete any existing assignees. 
1. Click `Add Assignee`. 
1. Begin typing the name of the agile team who you want to be assigned to the task or issue, then click the team name when it appears in the drop-down list. 
1. Click `Save Changes`.  
   The task or issue is now available on the team backlog.

## Move stories from the backlog to an iteration or Kanban board

* [Move existing stories to the backlog](#moving-existing-stories) 
* [Export stories from the backlog](#exporting-stories-from-the-backlog)

<ol> 
 <li value="1">Go to the backlog of the agile team.</li> 
 <li value="2">Select the stories you want to move to an iteration or Kanban board, then click <span class="bold">More</span> > <span class="bold">Move to</span>.<br>If moving the story to a Kanban board, the Move Story to the Kanban Board is displayed.<br>If moving the story to an iteration, the Move Story to an Iteration dialog box is displayed.<br><img src="assets/agile-backlog-addtoiteration-350x136.png" alt="agile_backlog_addtoiteration.png" style="width: 350;height: 136;"></li> 
 <li value="3">Do either of the following: 
  <ul>
   <li><span class="bold">For Scrum teams:</span> In the <span class="bold">Select Iteration</span> field, select the iteration where you want to move the stories.</li>
   <li><span class="bold">For Kanban teams:</span> In the <span class="bold">Select Kanban Board</span> field, select your team Kanban board. (Kanban teams can have only one Kanban board.)</li>
  </ul></li> 
 <li value="4">Click <span class="bold">Move Story</span>.</li> 
</ol>

### Move existing stories&nbsp;to the backlog

If you decide that your team is not yet ready to work on a story, you can&nbsp;move the&nbsp;story to the backlog.

For more information, see [Move an agile story](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Export stories from the backlog

You can export one or more stories (including tasks and issues) directly from the backlog.

You export stories from the backlog in the same way that you export other data in *Workfront*, as described in [Export data](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
