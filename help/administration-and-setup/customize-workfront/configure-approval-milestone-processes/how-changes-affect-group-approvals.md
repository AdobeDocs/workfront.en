---
filename: how-changes-affect-group-approvals
title: How approval process and group changes affect assigned approval processes
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
---



# How group and approval process changes affect assigned approval processes {#how-group-and-approval-process-changes-affect-assigned-approval-processes}

This article explains what happens when an approval process is already associated with tasks, issues, projects, templates, or template tasks and a *`Workfront administrator`* (or a user with administrative access to approval processes) does one of the following:



* Changes the approval process (group-level) from one group to another
* Changes the group associated with the project
* Changes the approval process from group-level to system-level
* Changes the approval process from system-level to group-level


For information about the 3 types of approval processes you can use in *`Workfront`*, see [Approval process overview](approval-process-in-workfront.md).


## Changing a group-specific approval process from one group to another {#changing-a-group-specific-approval-process-from-one-group-to-another}

The following scenarios occur when a group-specific approval process is already being used on an object and someone reassigns it to a different group:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Area or object where the approval process was attached</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Approval object</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Change in the approval process for the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project or template approval </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Becomes a single-use approval process</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task or template task approval </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Becomes a single-use approval process </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue approval</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Becomes a single-use approval process</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Tasks area in the Edit Project or Edit Template box</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The Task Default Approval Process field is reset to N/A.</p> <p>By default, no approval processes are associated with new tasks on the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Queue Details section of a project or template</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The Default Approval field is reset to N/A.</p> <p>By default, no approval processes are associated with new issues or requests on the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Queue Topic section of a project or template</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The Default Approval field is reset to N/A.</p> <p>No approval processes are associated with new issues or requests on the project by default.</p> </td> 
  </tr> 
 </tbody> 
</table>



##  



## Changing the group associated with a project {#changing-the-group-associated-with-a-project}

When someone changes the group associated with a project to different group, the following occurs:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Area or object that has the approval process already attached</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Approval object</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Change in the approval process of the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project or template approval </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Becomes a single-use approval process and the status associated with it updates to match a similar status for the new group.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task or template task approval </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Becomes a single-use approval process and the status associated with it updates to match a similar status for the new group.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue approval</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Becomes a single-use approval process and the status associated with it updates to match a similar status for the new group.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Tasks area in the Edit Project or Edit Template box</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The Task Default Approval Process field is reset to N/A</p> <p>By default, no approval processes are associated with new tasks on the project</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Queue Details section of a project or template</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The Default Approval Process field is reset to N/A</p> <p>By default, no approval processes are associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Queue Topic section of a project or template</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The Default Approval Process field is reset to N/A</p> <p>By default, no approval processes are associated with new issues or requests on the project</p> </td> 
  </tr> 
 </tbody> 
</table>



## Changing an approval process from group-level to system-level {#changing-an-approval-process-from-group-level-to-system-level}

When someone changes the Group option in a group-specific approval process to "All groups," the approval process becomes system-wide and the following occurs:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Area or object where the approval process was attached</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Approval object</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Change in the approval process of the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project or template approval </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No change</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task or template task approval </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">No change</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue approval</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No change</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Tasks area in the Edit Project or Edit Template box</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No change to the approval process but, by default, it is associated with new tasks on the project</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Queue Details section of a project or template</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Queue Topic section of a project or template</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
 </tbody> 
</table>



## Changing an approval process from system-level to group-level {#changing-an-approval-process-from-system-level-to-group-level}

When someone changes the availability of a system-wide approval process from "All groups" to a specific group, the approval process becomes group-specific and the following occurs:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Area or object where the approval process was attached</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Approval object</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Change in the approval process of the object or area</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project, task, issue, template, or template task that belongs to the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Project, task, or issue</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">No change</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Tasks area in the Edit Project or Edit Template box for a project or template that belongs to the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No change to the approval process but, by default, it is associated with new tasks on the project</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Queue Details section for a project or template that belongs to the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Queue Topic section for a project or template that belongs to the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>No change to the approval process but, by default, it is associated with new issues or requests on the project</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Project, task, issue, template, or template task that belongs to a group other than the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Projects</p> <p>Tasks</p> <p>Issues</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Becomes a single-use approval process</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Tasks area in the Edit Project or Edit Template box for a project or template that belongs to a group other than the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Tasks</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The Task Default Approval Process field is reset to N/A.</p> <p>By default, no approval processes are associated with new tasks on the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Queue Details section for a project or template that belongs to a group other than the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issues</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The Default Approval field is reset to N/A.</p> <p>By default, no approval processes are associated with new issues or requests on the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Queue Topic section for a project or template that belongs to a group other than the group of the approval process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Issues</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The Default Approval field is reset to N/A.</p> <p>By default, no approval processes are associated with new issues or requests on the project.</p> </td> 
  </tr> 
 </tbody> 
</table>



##  

