

# Create and customize priorities

You can control the priorities for&nbsp;projects, tasks, and issues in the Setup area of *Workfront*. Priorities give importance to your projects, tasks, or issues in *Adobe Workfront*.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customizing existing priorities

As a *Workfront administrator*, you can&nbsp;make the following modifications to the default priorities provided in *Workfront*:

* Rename priorities.
* Reorder the priorities.

  For more information on how to reorder priorities, see [Create a priority for a project task, or issue](#creating-new-priorities).&nbsp;

* Change the default priority.

  For more information on the functionality of changing the default priority, see [Create a priority for a project task, or issue](#creating-new-priorities).

* Edit the description for the priorities.&nbsp;
* Set a color for each priority.

  The color of the priority is used in chart reports, when you group your results by `Priority`.

  For more information on chart reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Delete priorities.

  When you delete an existing priority, you must select a replacement one.

* Hide priorities.

  For more information on the functionality of hiding priorities, see [Create a priority for a project task, or issue](#creating-new-priorities).

>[!NOTE]
>
>You must have at least one priority in your *Workfront* account for each object.

The priorities provided by default for each object type (project, task, and issue) are identical:

* None
* Low
* Normal
* High
* Urgent

## Create a priority for a project task, or issue

In addition to the default priorities provided in&nbsp;*Workfront*, you can add your own priorities to reflect the needs of your organization.

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span> > <span class="bold">Priorities</span>.</li> 
 <li value="3"> <p>Click the tab for the object type you want to create a priority for (<span class="bold">Project</span>, <span class="bold">Task</span>, or <span class="bold">Issue</span>).</p> </li> 
 <li value="4">Click <span class="bold">Add a New Priority</span>.</li> 
 <li value="5"> <p>Specify&nbsp;the following information for the new priority:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Priority Name</td> 
     <td>Type a name for your priority.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Importance</td> 
     <td> <p>When adding a new priority, a number is assigned to it&nbsp;by default. Edit this number, if it does not match your needs.</p> <p>The <span class="bold">Importance</span> number for each priority must be unique for the object you selected.<br>The number of the priority&nbsp;reflects the importance&nbsp;of the project, task or issue: the highest number corresponds to the highest priority.</p> <note type="note">
       &nbsp;You cannot edit the Importance number, after you save the priority.&nbsp;
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Color</td> 
     <td> <p>Choose a color for your priority.</p> <p>The color of the priority is used in chart reports and Agile Team Settings.&nbsp;For more information on chart reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.</p> <p>For more information on Agile Team Settings, see in&nbsp;.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Default Priority</td> 
     <td> <p>Decide whether this should be a default priority&nbsp;or not, by selecting the radio button.</p> <p>If a priority is designated as the <span class="bold">Default Priority</span>, it is automatically picked&nbsp;for all the projects, tasks, or issues in <em>Workfront</em>. <span class="bold">Normal</span> is the default priority for all objects in <em>Workfront</em>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>Add a description for your priority&nbsp;to explain its function.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Hide</td> 
     <td> <p>Select this box if you want to hide&nbsp;the priority.<br>When you select&nbsp;the <span class="bold">Hide</span> option, the priority does not display anywhere in <em>Workfront</em> and users are not able to choose it for their projects, tasks, and issues.</p> <note type="important">
       &nbsp;We recommend that you hide the priorities that you no longer want to use, rather than deleting them.&nbsp;By hiding them, you still keep all your historic data, of objects that have been completed with this priority, while preventing people from choosing this priority&nbsp;in the future.&nbsp;
      </note>(Optional) You can change the listing order of your priorities by&nbsp;dragging and dropping them in your desired order. This changes the order in which they display&nbsp;for projects, tasks, and issues. This does not change the <span class="bold">Importance</span> number.&nbsp;</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

1. Click `Save`.

For instructions on applying priorities to projects, tasks and issues, see the following articles:

* [Understand and update project priorities](../../../manage-work/projects/planning-a-project/project-priority.md) 
* [Update Task Priority](../../../manage-work/tasks/task-information/task-priority.md) 
* [Update issue Priority](../../../manage-work/issues/issue-information/update-issue-priority.md)

