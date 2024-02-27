---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Approval process overview
description: You can create an approval process and attach it to an object to make sure that designated users review certain changes before the object progresses.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
---
# Approval process overview

<!-- Audited: 12/2023 -->

You can create an approval process and attach it to an object to make sure that designated users review certain changes before the object progresses.

This is available for the following types of objects in Adobe Workfront:

* Work item (project, task or issue, template, template task)
* Document
* Proof

This article contains general information about approval processes associated with work items.
 For instructions on creating an approval process, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Types of approval processes for work items

If you are an Adobe Workfront administrator, or a user with administrative access to approval processes, you can create the following approval processes for projects, tasks, and issues:

* **A system-level global approval process**: Users can attach these to any of the following:

   * A project, task, or issue in the Approvals section
   * In the Edit Project box in the Task Default Approval Process area
   * In the Queue Details or Queue Topic section of a project in the Default Approval Process areas. The project must be enabled as a request queue.

* **A group-level global approval process**: Users can attach these to the following:

   * A project, task, or issue belonging to the group that is associated with the approval process in the Approvals section
   * In the Edit Project box in the Task Default Approval Process area for a project belonging to the group associated with the approval process
   * In the Queue Details or Queue Topic section of a project in the Default Approval Process areas. The project must be enabled as a request queue and must belong to the group associated with the approval process.

  For information about creating system-level or group-level approval process, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **A single-use approval process**: For use with a single project, task, issue, template, or template task. This type of approval process affects only the object that is associated with it and is not available to be associated with any other objects.

  For information about creating a single-use approval process, see [Associate a new or existing approval process with work](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>This article uses the term "global approval process" to differentiate from "single-use approval process." A global approval process can be used repeatedly. 
>
>The term "group-level global approval process" refers to an approval process that can be used repeatedly for items and with statuses associated only with a specific group.

For information about creating a system-level approval process or a group-level approval process see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considerations about approval processes

* You must create the project, task, issue, template, or template task before the approval process can be associated with them.
* An approval process is always associated with two essential things:

   * Each approval process corresponds to a certain work item status in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.

     >[!TIP]
     >
     >
     >   
     >   
     >   * You can associate a group-level approval with a global or a group-level status. 
     >   * You cannot change the status of an item using an approval process to a status other than the one associated with the approval process. 
     >   
     >   
     >     For example, if you have a task approval associated with the status of In&nbsp;Progress, the task automatically changes its status to In&nbsp;Progress when the approval is granted. It cannot automatically change its status to Completed or any other status that is not associated with the approval. 
     >   
     >   
     >

   * The entities associated with an approval process can be users, job roles, or teams. Users are ultimately responsible for accepting or rejecting the approval. You can assign approvals to users who fulfill a certain role on the project.&nbsp;For example, you can assign an approval to a Project Owner, or Sponsor.&nbsp;For more information, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     The following scenarios exist:

      * When you assign an approval to job roles, any user on the Project&nbsp;Team who is associated with the job role can make a decision on the approval. The role associated with the approval can be either their Primary&nbsp;Role or any Other Roles.

        For information about the Project Team, see [Project Team overview](../../manage-work/projects/planning-a-project/project-team-overview.md). 
      
      * When you assign an approval to a team, any member of that team can make a decision on the approval. The team associated with the approval can be either their Home Team or any of their Other Teams.

        For information about a user's roles and teams, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* When you create a work item, it does not automatically have an approval process attached. You must attach one manually if you want to use one. For information about attaching an approval process to an item, see [Associate a new or existing approval process with work](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md). 
* The Workfront administrator or a user with administrative access to approval processes can create a system-level global approval processes for use throughout the system. A group administrator with administrative access to approval processes can create a group-level global approval process for use only by a certain group that they manage.
* If you don't want to use a predefined system-level or group-level global approval process for a work item, you can create and attach a single-use approval process to it when you have Manage permissions to the object for which you want to attach the approval process.

  >[!NOTE]
  >
  >You can use a single-use approval process only once for the specific item for which it was created. You can associate global statuses as well as group-level statuses for single-use approval processes for projects, tasks, issues, templates, and template tasks.

* When attaching a group-level approval process to an item using group-level custom statuses, changing the Group of the project might create a conflict between the approval statuses of the previous group and those existing at the system level. Consider removing the group-level approval processes on the project, or its tasks or issues before updating the group. For information about creating group-level approval processes, see [Group-level approval processes](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). For information about creating custom group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). For information about updating the Group of a project, see [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).

## The approval process workflow

This section explains the following about approving work items:

* [How approval processes rely on statuses](#how-approval-processes-rely-on-statuses) 
* [How a typical workflow uses an approval process](#how-a-typical-workflow-uses-an-approval-process)

### How approval processes rely on statuses {#how-approval-processes-rely-on-statuses}

Attaching a status to an approval process ensures that the item moves through departments in the right order.

**Example:** You could attach an approval process to the Marketing Department status that requires approval by the Finance department. Then, when someone changes the status for a work item to "Marketing Department," the item can't move to that department until the Finance department signs off on it.

For more information about statuses for work items, see the following articles:

* [Access the list of system project statuses](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md) 
* [Access the list of system task statuses](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) 
* [Access the list of system issue statuses](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### How a typical workflow uses an approval process {#how-a-typical-workflow-uses-an-approval-process}

The following scenario illustrates how an approval process helps users approve work as a Workfront object progresses through a workflow of several steps in this order:

1. The Workfront administrator or a user with administrative access to Approval Processes creates an approval process for a project, task, or issue.

   >[!NOTE]
   >
   >You can attach project approval processes to a template, and task approval processes to a template task. After you do this, when someone uses the template to create a project, the approval process becomes a project or task approval process respectively. A single-use approval process attached to a template or template task remains a single-use approval process for projects and tasks.

1. A user with Manage permission to the project, task or issue attaches the approval process to the item, or creates a single-use approval for the item. 
1. A user assigned to the work item changes its status to the status that initiates the approval process and the approval process begins. (The person who created the approval process defined the relationship between the status and the approval process.)
1. The designated approvers receive a notification about the pending approval process and they review the work item.
1. The approval process ends after the designated approvers approve all steps of the process. Or, if they reject a step, the status is either reset to a predefined status, or an issue is created. (The person who created the approval process defined which of these automated steps happens after a rejection.)

**Example:** An advertising team has created a status called Ready for Printing and an approval process called Designer/ Copywriter Signoff that they associated with this status. This approval process is configured to:

* Require approval by the team's designer and copywriter
* Initiate whenever someone changes a work item's status to Ready for Printing

A brochure project owner attaches the Designer/ Copywriter Signoff approval process to the brochure project.

When someone on the project changes the status to Ready for Printing, the copywriter and designer receive notifications asking them to approve or reject it. During the approval process, when they are deliberating whether to approve it or not, the status of the projects displays as Ready for Printing - Pending Approval.

After they both approve the brochure in Workfront, the project status changes to Ready for Printing.

## Document approval processes

Document approvals are used for a more general approval. Feedback is captured in chat format on the Updates tab. You can use the approval buttons to approve, reject, or approve with changes.

To add approvers to a document after it's been uploaded to Workfront, see [Request document approvals](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Proof approval processes

Proof approvals are used for a deeper review and generally include more complicated workflows. Feedback is captured with markup tools in the proofing viewer. You can use the approval buttons to approve, reject, or approve with changes.

To add an Automated Workflow to a document proof and designate certain users in the workflow as approvers of the proof, see [Create an advanced proof with an Automated workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Configuring settings for work-item approval processes

As a Workfront administrator, you can configure global settings for work-item approval processes in your system. These settings determine various rules for approval processes, like how long an approval decision should be allowed to stay open or how you manage approval delegation in your system. For more information about approval process settings, see [Configure global approval settings](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
