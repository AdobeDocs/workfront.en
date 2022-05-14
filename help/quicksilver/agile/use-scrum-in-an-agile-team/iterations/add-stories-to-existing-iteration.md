---
filename: add-stories-to-existing-iteration
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Add stories to an existing iteration
description: You can add stories to an iteration in any of the following ways - EDIT ME.
---

# Add stories to an existing iteration

You can add stories to an iteration in any of the following ways:

* From the backlog after the iteration is created, as described in the [Move stories from the backlog to an iteration or Kanban board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) section in [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* From the Details page of the individual task or issue
* From a task or issue list
* From a report
* From a dashboard

## Access requirements

You must have the following access to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Worker or higher</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the project the story is on</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Understand how adding stories affects task dates

By default, when you add an existing task to an iteration, the task's Planned Start Date and Planned Completion Date are set as follows:

### **Task Planned Start Date**

* The task uses the iteration's Start Date when:

   * The project does not have a Planned Start Date set.
   * The project's Planned Start Date is *before* or *on* the iteration's start date.

* The task uses the project's Planned Start Date when:

   * The project's Planned Start Date is *after* the iteration's start date.

### **Task Planned Completion Date**

* The task uses the iteration's End Date when:

   * The project does not have a Planned Completion Date set.
   * The project's Planned Start Date is *before or on&nbsp;*the iteration's Start Date or the Project's Planned Completion Date is *before or on*&nbsp;the iteration's End Date.

* The task uses the project's Planned Completion Date when:

   * The project's Planned Start Date is&nbsp;*after*&nbsp;the iteration's Start Date&nbsp;and&nbsp;the project's Planned Completion Date is&nbsp;*after*&nbsp;the iteration's End Date.

You can configure individual Scrum teams to use the project dates by default, rather than the iteration dates. For information, see the section [Configure how dates are applied when adding work items to an iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in the article [Configure Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Add a story to an existing iteration

To add stories to an iteration directly from the task or issue:

>[!IMPORTANT]
>
>After the task moves to the iteration, you cannot update the Duration Type or Task Constraint. Duration Type is set to Simple and Task Constraint is set to Fixed Dates to keep the task timeline consistent with the iteration's timeline.

### **From the tasks or issues tab**

You can add any task or issue to any iteration if&nbsp;you have Manage access to the project. Keep the following in mind when moving a task or issue to an iteration:

* If the task or issue is assigned to an agile team and moved to another team's iteration, the team assignment does not change.&nbsp;
* If the task or issue is not assigned to a team, the task or issue is assigned to the team who owns the iteration.
* You can't add parent tasks to the iteration. If you add any child tasks, the parent task appears on the Scrum board as a swimlane.

1. Go to the project, report, or dashboard that contains the task or issue you want to add to an iteration.
1. Select one or more tasks or issues.
1. Click **More** ![](assets/more-icon.png) > **Add to Iteration**.  
   You cannot assign tasks or issues assigned to non-agile teams.

1. In the **Add Stories** box, type the name of the iteration.

   >[!NOTE]
   >
   >You can move a story from an existing iteration to a new iteration.

1. If you are adding tasks, click **Add Stories**.  
   Or  
   If you are adding issues, click **Add Issues**.

