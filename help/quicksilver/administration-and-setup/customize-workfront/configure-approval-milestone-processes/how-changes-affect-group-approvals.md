---
filename: how-changes-affect-group-approvals
title: How approval process and group changes affect assigned approval processes
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: How group and approval process changes affect assigned approval processes
description: This article explains what happens when an approval process is already associated with tasks, issues, projects, templates, or template tasks and a Workfront administrator (or a user with administrative access to approval processes) does one of the following:
---

# How group and approval process changes affect assigned approval processes

This article explains what happens when an approval process is already associated with tasks, issues, projects, templates, or template tasks and a Workfront administrator (or a user with administrative access to approval processes) does one of the following:

* Changes the approval process (group-level) from one group to another
* Changes the group associated with the project
* Changes the approval process from group-level to system-level
* Changes the approval process from system-level to group-level

For information about the 3 types of approval processes you can use in Workfront, see [Approval process overview](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Changing a group-specific approval process from one group to another

The following scenarios occur when a group-specific approval process is already being used on an object and someone reassigns it to a different group:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area or object where the approval process was attached</th> 
   <th>Approval object</th> 
   <th>Change in the approval process for the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project or template approval </td> 
   <td>Project</td> 
   <td>Becomes a single-use approval process</td> 
  </tr> 
  <tr> 
   <td>Task or template task approval </td> 
   <td>Task</td> 
   <td>Becomes a single-use approval process </td> 
  </tr> 
  <tr> 
   <td>Issue approval</td> 
   <td>Issue</td> 
   <td>Becomes a single-use approval process</td> 
  </tr> 
  <tr> 
   <td>Tasks area in the Edit Project or Edit Template box</td> 
   <td>Task</td> 
   <td> <p>The Task Default Approval Process field is reset to N/A.</p> <p>By default, no approval processes are associated with new tasks on the project.</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Details section of a project or template</td> 
   <td>Issue</td> 
   <td> <p>The Default Approval field is reset to N/A.</p> <p>By default, no approval processes are associated with new issues or requests on the project.</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section of a project or template</td> 
   <td>Issue</td> 
   <td> <p>The Default Approval field is reset to N/A.</p> <p>No approval processes are associated with new issues or requests on the project by default.</p> </td> 
  </tr> 
 </tbody> 
</table>

##

## Changing the group associated with a project

When someone changes the group associated with a project to different group, the following occurs:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area or object that has the approval process already attached</th> 
   <th>Approval object</th> 
   <th>Change in the approval process of the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project or template approval </td> 
   <td>Project</td> 
   <td>Becomes a single-use approval process and the status associated with it updates to match a similar status for the new group.</td> 
  </tr> 
  <tr> 
   <td>Task or template task approval </td> 
   <td>Task</td> 
   <td>Becomes a single-use approval process and the status associated with it updates to match a similar status for the new group.</td> 
  </tr> 
  <tr> 
   <td>Issue approval</td> 
   <td>Issue</td> 
   <td>Becomes a single-use approval process and the status associated with it updates to match a similar status for the new group.</td> 
  </tr> 
  <tr> 
   <td>Tasks area in the Edit Project or Edit Template box</td> 
   <td>Task</td> 
   <td> <p>The Task Default Approval Process field is reset to N/A</p> <p>By default, no approval processes are associated with new tasks on the project</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Details section of a project or template</td> 
   <td>Issue</td> 
   <td> <p>The Default Approval Process field is reset to N/A</p> <p>By default, no approval processes are associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section of a project or template</td> 
   <td>Issue</td> 
   <td> <p>The Default Approval Process field is reset to N/A</p> <p>By default, no approval processes are associated with new issues or requests on the project</p> </td> 
  </tr> 
 </tbody> 
</table>

## Changing an approval process from group-level to system-level

When someone changes the Group option in a group-specific approval process to "All groups," the approval process becomes system-wide and the following occurs:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area or object where the approval process was attached</th> 
   <th>Approval object</th> 
   <th>Change in the approval process of the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project or template approval </td> 
   <td>Project</td> 
   <td>No change</td> 
  </tr> 
  <tr> 
   <td>Task or template task approval </td> 
   <td>Task</td> 
   <td>No change</td> 
  </tr> 
  <tr> 
   <td>Issue approval</td> 
   <td>Issue</td> 
   <td>No change</td> 
  </tr> 
  <tr> 
   <td>Tasks area in the Edit Project or Edit Template box</td> 
   <td>Task</td> 
   <td> <p>No change to the approval process but, by default, it is associated with new tasks on the project</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Details section of a project or template</td> 
   <td>Issue</td> 
   <td> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section of a project or template</td> 
   <td>Issue</td> 
   <td> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
 </tbody> 
</table>

## Changing an approval process from system-level to group-level

When someone changes the availability of a system-wide approval process from "All groups" to a specific group, the approval process becomes group-specific and the following occurs:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area or object where the approval process was attached</th> 
   <th>Approval object</th> 
   <th>Change in the approval process of the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project, task, issue, template, or template task that belongs to the group of the approval process</td> 
   <td> <p>Project, task, or issue</p> </td> 
   <td>No change</td> 
  </tr> 
  <tr> 
   <td>Tasks area in the Edit Project or Edit Template box for a project or template that belongs to the group of the approval process</td> 
   <td>Task</td> 
   <td> <p>No change to the approval process but, by default, it is associated with new tasks on the project</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Details section for a project or template that belongs to the group of the approval process</td> 
   <td>Issue</td> 
   <td> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section for a project or template that belongs to the group of the approval process</td> 
   <td>Issue</td> 
   <td> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr> 
   <td>Project, task, issue, template, or template task that belongs to a group other than the group of the approval process</td> 
   <td> <p>Projects</p> <p>Tasks</p> <p>Issues</p> </td> 
   <td>Becomes a single-use approval process</td> 
  </tr> 
  <tr> 
   <td>Tasks area in the Edit Project or Edit Template box for a project or template that belongs to a group other than the group of the approval process</td> 
   <td>Tasks</td> 
   <td> <p>The Task Default Approval Process field is reset to N/A.</p> <p>By default, no approval processes are associated with new tasks on the project.</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Details section for a project or template that belongs to a group other than the group of the approval process</td> 
   <td>Issues</td> 
   <td> <p>The Default Approval field is reset to N/A.</p> <p>By default, no approval processes are associated with new issues or requests on the project.</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section for a project or template that belongs to a group other than the group of the approval process</td> 
   <td>Issues</td> 
   <td> <p>The Default Approval field is reset to N/A.</p> <p>By default, no approval processes are associated with new issues or requests on the project.</p> </td> 
  </tr> 
 </tbody> 
</table>

##

<!--
Moving a task or an issue to a project with a different group than that of the approval process Drafted out until this postponed story is completed Moving a task or an issue from a project to another might affect existing approval processes on the task or the issue depending on the groups of the two projects. The following table illustrates the scenarios that might exist: Original task or issue approval process Groups of the two projects Changes in the approval process after the task or issue is moved to another project Single-use approval process associated with a system-wide status Projects are in the same or different groups No change Single-use approval process associated with a group-specific status Projects are in different groups The approval remains a single-use approval process and the status associated with the approval updates to match a similar status for the new group. System-wide approval process Projects are in the same or different groups No change Group-specific approval process Projects are in the same group No change Group-specific approval process Projects are in different groups and the groups have different group-specific statuses The approval becomes a single-use approval process and the status associated with the approval updates to match a similar status for the new group. Group-specific approval process Projects are in different groups and there is a status with the same key in the new group as the status associated with the approval process from the first group No change
-->

