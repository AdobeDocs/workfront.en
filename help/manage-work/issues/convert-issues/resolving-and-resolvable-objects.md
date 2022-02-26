---
filename: resolving-and-resolvable-objects
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: Overview of Resolving and Resolvable Objects
description: A Resolvable Object is an issue whose resolution is tied to a Resolving Object. A Resolving Object is a project, task, or another issue.
---

# Overview of Resolving and Resolvable Objects

A Resolvable Object is an issue whose resolution is tied to a Resolving Object. A Resolving Object is a project, task, or another issue.

When you convert an issue to a task or a project, the issue becomes the Resolvable Object of the task or the project.   
You can also manually link an issue to a Resolving Object, which can be a task, project, or issue.&nbsp;For information, see [Manually tie the resolution of an issue to other issues, tasks, or projects](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).   
The original issue becomes the Resolvable Object of the task, project, or issue, in this scenario.

## Set up *Adobe Workfront* to handle Resolvable Objects

As a *Workfront administrator* ` or *group administrator*`, you can decide how you want to handle the Resolvable Objects in your system `or for your group.`

You can select to keep the Resolvable Object as you are converting it to a task or a project, or to delete it once the task or project are created. You can select to allow these settings to be changed in the process of converting issues, which will allow the user converting the issues to select whether to keep or to delete the issue as they are converting it.

>[!NOTE]
>
>Resolvable Objects are always issues whose resolution and status can depend on the resolution and status of the Resolving Object they are associated with. Resolving Objects can be issues, tasks, or projects.

For information about setting up preferences for handling Resolvable Objects, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to <em>Workfront</em> as a <em>Workfront administrator</em> <span>or <em>group administrator</em>.</span></li>
<li value="2"> <p> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
From the main menu, click
<span class="bold">Setup</span>.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
From the main menu, click
<span class="bold">Setup</span>.
</MadCap:conditionalText></p> <p> <draft-comment>
<img src="assets/qs-main-menu-expanded-with-menu-highlight-350x628.png" style="width: 350;height: 628;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/qs-main-menu-expanded-with-menu-highlight-350x628.png" style="width: 350;height: 628;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <span class="bold">Project Preferences</span>.</li>
<li value="4">Click <span class="bold">Tasks & Issues</span>.</li>
<li value="5">Go to the <span class="bold">Issues</span> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><span class="bold">Automatically update Resolvable Issue status when the status of the Resolving Object changes:</span> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <span class="bold">Keep the original issue and tie its resolution to the task</span> or<span class="bold"> project</span> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#syncrhonize-statuses" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><span class="bold">When converting an issue to a TASK...:</span> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><span class="bold">Keep the original issue and tie its resolution to the task:</span> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><span class="bold">Allow Primary Contact to have access to the task:</span> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><span class="bold">Allow these settings to be changed during conversion:</span> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><span class="bold">When converting an issue to a PROJECT...:</span> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><span class="bold">Keep the original issue and tie its resolution to the project:</span> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><span class="bold">Allow Primary Contact to have access to the project:</span> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><span class="bold">Allow these settings to be changed during conversion:</span> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <span class="bold">Save</span>.</li>
</ol>
</div>
-->

To establish the system default for what happens to the issue as it is being converted to a task or a project:

<ol> 
 <li value="1">Log in to <em>Workfront</em> as a <em>Workfront administrator</em> <span>or <em>group administrator</em>.</span></li> 
 <li value="2"> <p> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From the main menu, click 
    <span class="bold">Setup</span>. 
   </MadCap:conditionalText></p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x628.png" style="width: 350;height: 628;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="3">Expand <span class="bold">Project Preferences</span>.</li> 
 <li value="4">Click <span class="bold">Tasks & Issues</span>.</li> 
 <li value="5">Go to the <span class="bold">Issues</span> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings: 
  <ul>
   <li><p><span class="bold">Automatically update Resolvable Issue status when the status of the Resolving Object changes:</span> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <span class="bold">Keep the original issue and tie its resolution to the task</span> or<span class="bold"> project</span> must be selected.</p>
    <ul>
     <li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
     <li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#syncrhonize-statuses" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
       The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
      </note></li>
    </ul></li>
   <li><span class="bold">When converting an issue to a TASK...:</span> The settings in this section determine what happens during the conversion process from issue to task: 
    <ul>
     <li><span class="bold">Keep the original issue and tie its resolution to the task:</span> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
     <li><span class="bold">Allow Primary Contact to have access to the task:</span> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
     <li><span class="bold">Allow these settings to be changed during conversion:</span> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
    </ul></li>
   <li><span class="bold">When converting an issue to a PROJECT...:</span> The settings in this section determine what happens during the conversion process from issue to project: 
    <ul>
     <li><span class="bold">Keep the original issue and tie its resolution to the project:</span> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
     <li><span class="bold">Allow Primary Contact to have access to the project:</span> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
     <li><span class="bold">Allow these settings to be changed during conversion:</span> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
    </ul></li>
  </ul></li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

## Handle the Resolvable Object during the conversion to a project or a task

Depending on the way the *Workfront* or *group administrator* configured the system or group level issue preferences, you might be able to handle the resolvable object during the conversion of an issue to a project or a task.   
The following scenarios exist:

<ul> 
 <li> <p>If the <em>Workfront</em> <span>or <em>group administrator</em></span> has the <span class="bold">Keep the original issue and tie its resolution to the task</span> and the <span class="bold">Keep the original issue and tie its resolution to the project</span> selected and the <span class="bold">Allow these settings to be changed during conversion</span> unselected, you will not be able to change these settings as you are converting issues to tasks or projects.<br><img src="assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png" style="width: 350;height: 217;"><br></p> </li> 
</ul>

<ul> 
 <li> <p>If the <em>Workfront</em> or <em>group administrator</em> has the <span class="bold">Keep the original issue and tie its resolution to the task</span> and the <span class="bold">Keep the original issue and tie its resolution to the project</span> either selected or unselected and the <span class="bold">Allow these settings to be changed during conversion</span> selected, you will be able to change these settings as you are converting issues to tasks or projects.<br><img src="assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png" style="width: 350;height: 113;"><br></p> </li> 
</ul>

For more information about converting issues to tasks and projects, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="tying-the-resolution-of-an-issue-to-task-project-issue"></a>Tie the resolution of an issue to a project, task or issue</h2>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#syncrhonize-statuses" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click the
<span class="bold">Issue Details</span> >
<span class="bold">Overview</span> area.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click the
<span class="bold">Issue Details</span> >
<span class="bold">Overview</span> area.
</MadCap:conditionalText></p> <p> <draft-comment>
<img src="assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png" style="width: 350;height: 462;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png" style="width: 350;height: 462;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit</span> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit</span> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form, <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
click
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
click
</MadCap:conditionalText>in the <span class="bold">Resolved By</span> field, <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
and
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
and
</MadCap:conditionalText>select from the following types of resolving objects:
<ul>
<li><span class="bold">Project</span></li>
<li><span class="bold">Task</span></li>
<li><p><span class="bold">Issue</span></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <span class="bold">Save</span>&nbsp;<draft-comment>
<span class="bold" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Changes</span>
</draft-comment><span class="bold" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Changes</span>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## Tie the resolution of an issue to a project, task or issue

You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue.   
For more information about how the status of the Resolving Object affects the Resolvable Object, see [Synchronize the Status of the Resolvable Object with that of the Resolving Object](#syncrhonize-statuses).

You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this.

To tie the resolution of an issue to the resolution of a project, task, or issue:

<ol> 
 <li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li> 
 <li value="2"> <p> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Issue Details</span> > 
    <span class="bold">Overview</span> area.
   </MadCap:conditionalText></p> <p> <img src="assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png" style="width: 350;height: 462;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit</span> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li> 
 <li value="4">At the bottom of the form, <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   click 
  </MadCap:conditionalText>in the <span class="bold">Resolved By</span> field, <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   and 
  </MadCap:conditionalText>select from the following types of resolving objects: 
  <ul>
   <li><span class="bold">Project</span></li>
   <li><span class="bold">Task</span></li>
   <li><p><span class="bold">Issue</span></p></li>
  </ul><p>The field for the resolving object displays. </p></li> 
 <li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li> 
 <li value="6">Click <span class="bold">Save</span>&nbsp;<span class="bold" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Changes</span>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
    One project, task, or issue may have multiple issues as Resolvable Objects.
  </note></li> 
</ol>

## Synchronize the Status of the Resolvable Object with that of the Resolving Object

* [Synchronize statuses when the Resolving Object is an issue](#syncrhonizing-statuses-for-issues) 
* [Synchronize statuses when the Resolving Object is a task or a project](#synchronizing-statuses-for-projects-and-tasks)

### Synchronize statuses when the Resolving Object is an issue

If an issue is manually tied to another issue, the status of the second issue (Resolving Object) triggers a change in the status of the first issue (Resolvable Object). The status of the first issue matches the status that the second issue is changed to. This applies for both default and custom issue statuses.

### Synchronize statuses when the Resolving Object is a task or a project

When an issue is the Resolvable Object of a task or a project, the changes in the status of the tasks and the projects trigger changes in the status of the issue. Default statuses are triggered differently than Custom statuses, in this case.

* [Synchronize the Default Status of the Resolving Object with the Default Status of the Resolvable Object](#syncrhonizing-default-statuses) 
* [Synchronize the Custom Status of the Resolving Object with the Custom Status of the Resolvable Object](#syncrhonizing-custom-statuses)

#### `Synchronize the Default Status of the Resolving Object with the Default Status of the Resolvable Object`

Regardless of whether the `Automatically set issue statuses to match the resolvable object using the Status keys` `` option is selected or not, every time the default status changes on the Resolving Objects (projects or tasks), the status of the Resolvable Object (issues) changes, accordingly. Only default statuses are already mapped to trigger such a change.

The following default statuses for tasks trigger the following changes in the default statuses for issues, when the issue is set as the resolving object of a task:

| `TASK STATUS`  | `ISSUE STATUS`  |
|---|---|
| New |New |
| In Progress |In Progress |
| Complete |Closed |

The following default statuses for projects trigger the following changes in the default statuses for issues, when the issue is set as a Resolvable Object of a project. Some project statuses do not trigger changes to the status of the issues. The issues remain in the status they were before the project was turned into one of these statuses:

| `PROJECT STATUS`  | `ISSUE STATUS`  |
|---|---|
| Planning |New |
| Current |In Progress |
| On Hold |On Hold |
| Requested |Does not trigger a change to the issue status |
| Approved |Does not trigger a change to the issue status |
| Rejected  |Does not trigger a change to the issue status |
| Idea |Does not trigger a change to the issue status  |
| Dead |Closed |
| Completed |Closed |

>[!NOTE]
>
>After the status of the issue becomes Closed (as a result of closing the task or the project), regardless of what status the task or project changes to after closing them, the issue remains Closed.

#### `Synchronize the Custom Status of the Resolving Object with the Custom Status of the Resolvable Object`

When you change the status of the task or project to a custom status, the status of the issue changes to a custom issue status only if the following two conditions are met:

* The `Automatically` `set issue statuses to match the resolvable object using the Status keys` option is selected. For more information about how to enable this setting, see [Set up Adobe Workfront to handle Resolvable Objects](#system-setup-to-handle-resolving-objects).

* The custom status of the project or task has the same three letter code as the custom status of the issue.

You can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a Resolving Object) are changed to the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.

For example, create a project custom status named "Launched" with the three letter code "LCD" which equates with "Current". Also, create an issue custom status named "Project Launched", also with the letter code "LCD" which equates with "In Progress". When you mark the project as "Launched", the issue will automatically change the status to "Project Launched". If the `Automatically` `set issue statuses to match the resolvable object using the Status keys` setting were not enabled, the issue status would change to "In Progress" instead (the default status).  
For more information about creating a custom status, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Synchronize the percent complete of a Resolving Object with that of the Resolvable Object

If an issue is resolved by a task or a project, the percent complete of the issue updates on the resolvable issue when any of the following things occur:&nbsp;

* When someone saves a change on the task or project. 
* The timeline of the project is recalculated.

If and issue is resolved by another issue, the percent complete updates when either of the issues update.

## Locate the Resolvable Object on a task or a project

Locating the resolving object is identical for tasks and projects.

<ol> 
 <li value="1">Navigate to a project or a task which you created by converting an issue to the project or the task.</li> 
 <li value="2"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
     <span class="bold">Project Details</span> or the 
     <span class="bold">Task Details</span> icon and click to expand it. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Project Details</span> or the 
    <span class="bold">Task Details</span> icon and click to expand it. 
   </MadCap:conditionalText></p> <p> <draft-comment>
    <img src="assets/qs-details-icon-applies-to-all-objects.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-details-icon-applies-to-all-objects.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="3"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Overview</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Overview</span>.
  </MadCap:conditionalText> </li> 
 <li value="4">At the bottom of the tab, locate to <span class="bold">This Resolves</span> field: the issue which is the Resolvable Object of the project or the task is listed in this field.<br><note type="note">
    Issues cannot be converted to other issues, but they can manually be associated with a Resolving Issue. A project, task, or issue can have multiple issues as Resolvable Objects. When the project, task, or issue resolves, the Resolvable Object (issue) also resolves. The Resolvable Issue remains closed even if the project, task, or issue that resolved it re-opens. 
  </note></li> 
</ol>

## Identify an issue with a Resolving Object in a list

In a list of issues, you can identify issues that are labeled as resolving objects via status icons by locating this icon in the `Status Icons` or `Flags` columns:

![](assets/ro1.png)

## View Resolvable and Resolving Object information in a report

You can display information about the Resolvable or Resolving Objects in the view or report for projects, tasks, or issues.  
The following table shows what fields you can display and in which views you can display them:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Field in View</span> </th> 
   <th><span class="bold">Issue View</span> </th> 
   <th><span class="bold">Task View</span> </th> 
   <th><span class="bold">Project View</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><span class="bold">Has Resolvables</span>: Displays a <span class="bold">True</span> value if the project or task has Resolvable Issues associated with them, and a <span class="bold">False</span> value if they do not.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><span class="bold">Original Issue Name, Original Issue Entry Date, Originator Name</span>: Displays the name and entry date of the original issue, as well as the name of the user who created the issue in a text-mode customized view.<br>For more information about building a text mode custom view for a project or task report or list to display information about the original issue, see <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">View: display original issue information on task and project list</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Resolvables:</span> Displays a list of all Resolvable Objects in a text mode custom view for a project or task report or list.</p> <p>For more information about building this view, see <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">View: Resolvable Objects in a task or project report</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><span class="bold">Converted Issue Originator</span>: Displays information about the user who originally logged the issue which was later converted to the task. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Resolve Project</span>: Displays information about the Resolving Project which was either converted from the original issue, or manually designated as the Resolving Object of an issue.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Resolve Task</span>: Displays information about the Resolving Task which was either converted from the original issue, or manually designated as the Resolving Object of an issue.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Resolve Issue</span>: Displays information about the Resolving Issue which was manually designated as the Resolving Object of an issue.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

