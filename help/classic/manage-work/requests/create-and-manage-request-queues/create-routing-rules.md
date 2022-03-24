---
filename: create-routing-rules
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create Routing Rules
description: Routing Rules control what Adobe Workfront does with issues when they are submitted to a Request Queue. For more information about creating Request Queues, see Create a Request Queue.
---

# Create Routing Rules

Routing Rules control what Adobe Workfront does with issues when they are submitted to a Request Queue. For more information about creating Request Queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Routing Rules send issues to specific users or job roles best equipped&nbsp;to resolve the submitted issue or request. Routing rules are usually associated with queue topics,&nbsp;which are used to control which routing rule will be applied to the issue or request.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator

## Create a Routing Rule

1. Go to the project which you want to add the routing rules for your requests. 
1. Click **More**, then select **Queue Setup.**

1. Click the&nbsp;**Routing Rules**&nbsp;subtab.&nbsp;
1. Click **New Routing Rules**&nbsp;to add the new rule.&nbsp;

   ![](assets/7-350x75.png)

1. Specify the following information for the Routing Rule:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>&nbsp;</th> 
      <th>&nbsp;</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p>The name of the&nbsp;Routing Rule. You can see the Routing Rule if you have access to see this information on the project.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Add a description for the Routing Rule.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Default Assignee*</strong> </td> 
      <td>Add an active user or an <span data-mc-edit-date="2021-05-27T11:52:45.4165986-04:00" data-mc-editor="alinawilson" data-mc-comment="yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-05-25T13:04:12.7687137-04:00">active</span> job role&nbsp;to whom the new issues should be assigned. You can only have one default assignee in this field. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Default Team*</strong> </td> 
      <td>Add an active team to whom the new issue should be assigned. You can only have one team assigned to the issue. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Route to Project</strong> </td> 
      <td>This is the project where the issue is added.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >&#42;If a user, ```job role```, or team are deactivated after they are associated with a routing rule, the requests continue to be routed to them. You must periodically take an inventory of all routing rules and replace deactivated assignments with active ones.

   When you route an issue to a project, users with permissions on the issue receive the permissions set on that project. For information about setting permissions on projects, see [Share a project in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/8-350x206.png)

1. Select**Save**&nbsp;when done.  
   This process only defines&nbsp;the Routing Rule. To ensure that the issue is routed when it is submitted to the Request Queue, you must&nbsp;select the routing&nbsp;rule&nbsp;on the **Queue Details** tab under&nbsp;**Default Route**. For information about adding a Default Route to a Request Queue, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).  
   If you want to associate multiple routing rules with the Request Queue, you must create multiple Queue Topics and associate each one with a separate Routing Rule. For more information about creating a queue topic, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

