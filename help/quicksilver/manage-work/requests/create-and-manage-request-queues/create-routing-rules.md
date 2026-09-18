---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create Routing Rules
description: Routing Rules control what Adobe Workfront does with issues when they are submitted to a Request Queue.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-YFIx4ZtuC3xkzqJzYxbTh3BrumyMI2-w7NmpiTyKpc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create Routing Rules

<!-- Audited: 12/2023 -->

Routing rules control what Adobe Workfront does with issues when they are submitted to a request queue. For more information about creating Request Queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Routing rules send issues to specific users or job roles best equipped to resolve the submitted issue or request. Routing rules are usually associated with queue topics, which are used to control which routing rule will be applied to the issue or request.

Once created, you cannot move routing rules from one project to another.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront packages</p></td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Create a Routing Rule

1. Go to the project in which you want to add routing rules for your requests. 
1. Click **Routing Rules** in the left panel. 
1. Click **New Routing Rule** to add the new rule. The **New Routing Rule** box opens.

    ![New Routing Rule box](assets/new-routing-rule-box.png)
1. Enter the following information for the Routing Rule:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td>The name of the routing rule. You can see the routing rule if you have access to see this information on the project.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Add a description for the routing rule.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Default Assignee*</strong> </td> 
      <td>Add an active user or an active job role to whom the new issues should be assigned. You can only have one default assignee in this field. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Default Team*</strong> </td> 
      <td>Add an active team to whom the new issue should be assigned. You can only have one default team in this field.
      
      <p><b>NOTE</b></p>
      
      After the issue is submitted, you can edit its assignments and assign other users, roles, or teams. For information, see  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Assign issues</a>. 
      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Route to Project</strong> </td> 
      <td>This is the project where the issue is added.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*If a user, job role, or team are deactivated after they are associated with a routing rule, the requests continue to be routed to them. You must periodically take an inventory of all routing rules and replace deactivated assignments with active ones.

   When you route an issue to a project, users with permissions on the issue receive the permissions set on that project. For information about setting permissions on projects, see [Share a project in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

1. Click **Save**.

   This process only defines the Routing Rule. To ensure that the issue is routed when it is submitted to the request queue, you must select the routing rule on the **Queue Details** tab under **Default Route**.
   
   For information about adding a Default Route to a request queue, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   
   If you want to associate multiple routing rules with the request queue, you must create multiple queue topics and associate each one with a separate routing rule. For more information about creating a queue topic, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
