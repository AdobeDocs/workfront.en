---
filename: simple-duration-type
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Duration Type overview: Simple
description: The Simple Duration Type is a Duration Type that you can set for a task in Adobe Workfront. For general information about Duration Types in Workfront, see Overview of Task Duration and Duration Type.
---

# Duration Type overview: Simple

The Simple Duration Type is a Duration Type that you can set for a task in *Adobe Workfront*. For general information about Duration Types in *Workfront*, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overview of the Simple Duration Type

Your *Workfront* `or a *group administrator*` can set the default Duration&nbsp;Type of your system or group as Simple.&nbsp;In this case, all new tasks will be created with this Duration Type. For information about changing your task and issue preferences as part of your system-level or group-level project preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

The following things occur when a task has a Duration Type of Simple:

<ul> 
 <li> <p>Project managers can modify the both the Duration and the Planned Hours of a task when modifying how those hours should be distributed among assignees. </p> <p>For information, see <a href="../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md" class="MCXref xref" xrefformat="{para}">Update the Planned Hours and Duration of a task with a Simple Duration Type</a>.</p> <note type="important">
   When you first create a task and assign the Simple Duration&nbsp;Type to it and do not specify a Duration, 
   <em>Workfront</em> calculates the Duration of the task based on the amount of Planned Hours you specify for the task. If you manually modify the Duration of a Simple Duration task, 
   <em>Workfront</em> stops matching the Planned Hours to the Duration because it assumes you want to define them manually yourself. 
  </note> </li> 
 <li>Allocation percent is hidden and allocation hours are available to be edited, instead.</li> 
 <li>All new customers have the system-level Duration Type set to Simple. <a name="editing-planned-hours-for-simple-duration-tasks"></a></li> 
</ul>

## Change the Duration Type of a task to Simple

For information about changing the Duration Type of a task, see [Update the Duration Type of a task](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Task Details</span> in the left panel, then in the Overview area double click <span class="bold">Duration Type</span>. </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Task Details</span> in the left panel, then in the Overview area double click <span class="bold">Duration Type</span>. </p> </li>
<li value="3"> <p>Select <span class="bold">Simple</span> from the drop-down menu.</p> </li>
<li value="4">Click <span class="bold">Save</span><draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<span class="bold">Changes</span>
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<span class="bold">Changes</span>
</MadCap:conditionalText><span class="bold">.</span></li>
</ol>
-->

1. Go to a task for which you want to change the Duration Type.
1. Click `Task Details` in the left panel, then in the Overview area double click `Duration Type`. 
1. Select `Simple` from the drop-down menu.
1. Click `Save``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  <span class="bold">Changes</span></MadCap:conditionalText>` `.`

