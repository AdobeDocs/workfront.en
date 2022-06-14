---
product-area: projects
navigation-topic: use-the-home-area
title: Mark an item as Done in the Home area
description: You can mark a task or issue as Done if you are the task or issue assignee. When you mark a task or issue as Done, the status of the task or issue is changed to Complete.
feature: "Get Started with Workfront, Work Management"
---

# Mark an item as Done in the Home area

You can mark a task or issue as Done if you are the task or issue assignee. When you mark a task or issue as Done, the status of the task or issue is changed to Complete.

>[!NOTE]
>
>You do not see the Done button unless you are one of the resources assigned to the task or the issue.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>Edit access to Tasks and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the tasks and issues you need to work on</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Mark a task or issue as Done

Only the user assigned to the task or issue can mark it as Done.

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner, then click&nbsp;**Home**. 
1. In the **Work List**, locate any of the items waiting to be worked on.
1. Do either of the following:

* Click&nbsp;**Done**&nbsp;on the work item.  
  See [Understand the options of the Done button](#understand-the-options-of-the-done-button) for more detailed information about how this button might appear.

* Select the item you want to mark as done, then in the right panel, click&nbsp;**Update Status**, then change the status of the item to a status that equates with Complete or Closed.&nbsp;

## Understand the options of the Done button {#understand-the-options-of-the-done-button}

By default, clicking the Done button on a work item changes the status of that item to Complete (for tasks) or Resolved (for issues).&nbsp;

Your Adobe Workfront administrator can customize what statuses are associated with the Done button, and apply those customizations to your Home Team.

Depending on how many statuses are associated with the Done button or how many resources are assigned to the task or the issue, the look of the Done button can change.&nbsp;

* [Done button associated with one status](#done-button-associated-with-one-status) 
* [Done button associated with multiple statuses](#done-button-associated-with-multiple-statuses) 
* [Done button for items assigned to multiple resources](#done-button-for-items-assigned-to-multiple-resources)

### Done button associated with one status {#done-button-associated-with-one-status}

When the Done button is associated with one status and the work item is assigned to you only, the button reads **Done**. When you click it, the status of the task or the issue is changed to the status associated with the Done button.

![Done button](assets/Done.png)

To understand which status is associated with the Done button, check the Team Settings of your Home Team for the Done Button section, as described in [Edit team settings](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

If you are not assigned to a Home Team,&nbsp;the default status is chosen when clicking Done, as described above in [Understand the options of the Done button](#understand-the-options-of-the-done-button).

### Done button associated with multiple statuses {#done-button-associated-with-multiple-statuses}

When the Done button is associated with more than one status, the button shows the word **Done** which is followed by a drop-down menu. In this scenario, you cannot simply click Done. You must select a status from the drop-down menu. Select the status that best fits the completion of the work item. By doing this, you are changing the status of the work item.

To understand how you can associate multiple statuses with the Done button, see [Configure the Done button for tasks](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) and [Configure the Done button for issues](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### Done button for items&nbsp;assigned to multiple resources {#done-button-for-items-assigned-to-multiple-resources}

When the task or the issue is assigned to more than one resource, the button shows the word **Done** which is followed by a drop-down menu. In the drop-down menu, you have the option to chose between **Done with my part** (which lets team members know you are complete with your portion of the task), or the status associated with the Done button (which&nbsp;completes the item). After you select **Done with my part**, the work item is removed from your Work List, but remains in the Work List of those still assigned to the work item.  
If the Done button is associated with multiple statuses, they are listed under **Done with my part**.

>[!NOTE]
>
>On a task or issue with multiple assignees, each user is responsible for indicating that their own assignment on the task or issue has actually been completed. For this reason, each assignee must click Done to show they have completed the work assigned to them on the item.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)

