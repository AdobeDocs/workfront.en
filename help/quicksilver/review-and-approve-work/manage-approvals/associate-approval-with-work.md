---
product-area: projects
navigation-topic: approvals
title: Associate a new or existing approval process with work
description: This article describes how you can associate approval processes with work items. For information about associating approvals with proofs or documents, see the following articles.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
---
# Associate a new or existing approval process with work

This article describes how you can associate approval processes with work items. For information about associating approvals with proofs or documents, see the following articles:

* [Create an advanced proof with an Automated workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md) 
* [Request document approvals](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

You can associate a global or single-use approval process with a work item in Adobe Workfront. The following scenarios exist:

* Associate an existing global approval process with a project, task, issue, template, or template task. Some global approval processes are available to all groups in the system. Group-level global approval processes are available only to certain groups.
* Create a single-use approval process and associate it with an existing project, task, issue, template, or template task.

>[!NOTE]
>
>This article uses the term "global approval process" to differentiate from "single-use approval process." A global approval process can be used repeatedly. 
>
>The term "group-level global approval process" refers to an approval process that can be used repeatedly for items and with statuses associated only with a specific group.

For more general information about approval processes, see [Approval process overview](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

For information about creating a global approval process, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access or higher to Projects, Tasks, Issues, or Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project, task, issue, or template</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Considerations about associating approval processes with work items

In addition to the considerations described below, we recommend that you revisit the general considerations about approval processes in&nbsp;Workfront. For more information, see [Approval process overview](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* You must create the project, task, issue, template, or template task before the approval process can be associated with them.
* When you attach an approval process to an item for a status that has passed and in which the item currently is, the approval process will not be triggered and no notifications are sent to the approvers.

  **Example:** If a task is in the status of Complete and you attach an approval process associated with the Complete status, the approval does not trigger. 

* When you attach an approval process to the first status of an item (by using a template for tasks and projects, using the Queue Setup settings for issues, or defining the Task Settings of a project for new tasks), the approval processes are bypassed if the submitted approval is recalled. In this case, the approvers do not receive any notifications.

  For more information about recalling approvals, see [View approvals](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >The first status for a task or issue is New. The first status for a project is the status selected by your Workfront administrator in the Project Preferences in your system. For information, see [Configure system-wide project preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* The association of approval processes with an object is not recorded in the Updates area for the object.
* You cannot associate an approval process with a parent task.
* Adding a user, team, or role as an approver does not automatically give them permissions to the object associated with that approval. They receive permissions to the object when the approval step is triggered. Otherwise, the objects must be shared with them before they can make an approval decision.

The following sections describe the different methods of associating an approval process to a project, task, or issue.

## Associate a global approval process with a work item {#associate-a-global-approval-process-with-a-work-item}

You can associate a global approval process with a work item (project, task, issue, template, template task).

The global approval process must be available to the group associated with the work item or to all groups in the system.

>[!NOTE]
>
>You can attach project approval processes to a template, and task approval processes to a template task. After you do this, when someone uses the template to create a project, the approval process becomes a project or task approval process respectively. A single-use approval process attached to a template or template task remains a single-use approval process for projects and tasks.

For information about how Workfront administrators can configure a global approval process for all groups in the system, and how group administrators can create approvals for a group, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>You can also modify a global approval process to meet your specific needs. For more information, see the section [Modify a global approval process for use on a specific object](#modify-a-global-approval-process-for-use-on-a-specific-object) in this article.

To associate an existing global approval process with a project, task, issue, template, or template task:

1. Go to the work item where you want to associate an approval process.
1. Click **Approvals** in the left panel.

   You might need to click **Show More**, then click **Approvals**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   The approval process selected displays.

1. Expand the **Use existing** drop-down menu and select an existing approval process.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   The approval process selected displays.

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Click **Save**.
1. (Optional) Click Edit Approval Process if you want to modify the existing approval you attached to the item. This changes the global approval process to a single-use approval process. For more information, see the section [Modify a global approval process for use on a specific object](#modify-a-global-approval-process-for-use-on-a-specific-object) in this article.

## Modify a global approval process for use on a specific object {#modify-a-global-approval-process-for-use-on-a-specific-object}

Your Workfront administrator or group administrator creates global approval processes for you to use, as described in [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Modifying a global approval process attached to an item is identical to modifying a single-use approval process.

You can modify a global approval process to suit any specific needs of the project, task, or issue that you associate with it.

>[!IMPORTANT]
>
>When you modify a global approval process, it becomes a single-use approval process that can be used only on the object where you modified it. The global approval process remains unchanged.
>
>Consider the following limitations when modifying a global approval process:
>
>* The approval process is modified only for the project, task, or issue you are associating the approval process with.
>* Any future changes made by an administrator to the original global approval process do not reflect on the global approval process that you modified.
>

To modify a approval process already attached to an item:

1. Add a global approval process to the project, task, or issue.

   For instructions, see the section [Associate a global approval process with a work item](#associate-a-global-approval-process-with-a-work-item) in this article.

   >[!IMPORTANT]
   >
   >Ensure that you click **Save** when adding the approval.

1. After the global approval process is added, click the **Edit**icon ![](assets/edit-icon.png) in the upper-right corner of the approval page. This action turns the global or group-level approval process into a single-use approval process. 
1. Make any changes to the existing approval process. For more information, see the section [Associate a single-use approval process with a project, task, issue, template, or template task](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) in this article. 
1. Click **Save**, then click **Save** again to confirm that you want to convert the global approval process to a single-use approval process that is available only on this object.

## Associate a single-use approval process with a project, task, issue, template, or template task {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

You can create a single-use approval process for use only on a specific project, task, or issue.

You can also associate a single-use approval process with a template or template task so that it is available on projects and tasks that are created from the template.

>[!NOTE]
>
>You can associate a single-use approval process with any system-level or group-level status for a project, task, issue, template, or template task. For information about Workfront statuses, see [Create or edit a status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Creating an approval process in this way enables you to create a custom approval process to meet your needs. However, the approval process cannot be associated with other work items in the future.

Alternatively, you can modify a global approval process for a specific item and that also becomes a single-use approval process. For information, see the section [Modify a global approval process for use on a specific object](#modify-a-global-approval-process-for-use-on-a-specific-object) in this article.

To create a single-use approval process:

1. Go to the project, task, issue, template, or template task where you want to associate an approval process. 
1. Click **Approvals** in the left panel.

   You might need to click **Show More** > **Approvals**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Click **Create single-use**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Complete the steps beginning with step 6 in the section "Create a system-level or group-level global approval process for work items" in the article [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >After you attach the single-use approval process, it displays as "`<Custom>`" in the Approval Process field inside the Edit box of templates and template tasks. For information about editing templates or template tasks, see the following articles:
   >
   >* [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md) 
   >* [Edit a template task](../../manage-work/projects/create-and-manage-templates/edit-template-task.md) 

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Remove or delete an approval process from a work item

You can remove a global or group-level approval process or you can delete a single-use approval process from a project, task, or issue previously associated with it.

The following scenarios exist:&nbsp;

* Removing the global or group-level approval process does not delete the approval. The approval remains available for future use. 
* Deleting a single-user approval process deletes it from Workfront and it cannot be recovered.

To remove or delete an approval process from a work item:

1. Go to the project, task, issue, template, or template task where you want to remove an approval process that you previously added. 
1. Click **Approvals** in the left panel.

   You might need to click **Show More** > **Approvals**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Click one of the following icons in the upper-right corner of the Approvals section, depending on what type of approval is associated with the item:

   * **The Remove**icon ![](assets/remove-icon---x-in-circle.png) for global or group-level approvals.
   * **The Delete**icon ![](assets/delete.png) for single-use approvals.

1. Click **Remove** or **Delete** to confirm.

   The approval process is removed from the work item.

## Automatically associate an approval process with work items

You can associate an approval process automatically with work items using the following workflows:

* For projects and tasks, you can associate an approval process using a template. You can attach an existing approval process to the Template Approvals tab or the Template Task Approvals tab. For information about associating an existing approval with a work item, see [Associate a global approval process with a work item](#associate-a-global-approval-process-with-a-work-item) in this article.
* For new tasks on an existing project, you can associate a global approval process or a group-level global approval process in the Task Settings area of the Edit Project box. For information, see the section "Task Settings"&nbsp;in the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).
* For issues, you can associate an approval with every new issue that is added to a project by associating an existing approval process with a request queue. For information about configuring request queues, see [Create a Request Queue](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
