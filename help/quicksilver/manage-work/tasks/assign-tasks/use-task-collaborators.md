---
title: Use task collaborators
content-type: reference
description: Learn how to use Task Collaborators, AI Collaborators that can be assigned to Workfront tasks.
author: Becky
feature: Work Management, Tasks

---
# Use task collaborators

Task Collaborators are AI Collaborators that can be assigned directly to Workfront tasks, in addition to the existing Reviewer-type AI Collaborator used for document and asset reviews. Like other AI Collaborators, Task Collaborators are configured in the Setup area and assigned to tasks just like a user.

Task collaborators connect to agents that you have configured, much like an MCP server. 

For information and instructions about creating a Task Collaborator in Workfront, see [Configure a Task Collaborator](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) in the article Configure AI Collaborators.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Standard, Prime, or Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

* You must configure an agent in Copilot, Claude, or Writer.ai before you can use it as a Task Collaborator.

## Task collaborator overview

Task collaborators are a way to assign MCP agents to specific tasks in Workfront. You configure the agent in an app such as Copilot Studio, Claude, or Writer.ai, then connect that agent to Workfront as a Task Collaborator. You can then assign it to tasks as you would assign a user. 

Some example workflows may include:

* Detecting images uploaded to a task, generating variations based on criteria given to the agent, and uploading the new images to the task.
* Generating copy from a task description, reviewing the copy against guidelines configured in the agent, and posting copy to the update stream.
* Reading details of an event, identifying missing details, and posting questions in the update stream about the missing details.

>[!NOTE]
>
>* Specific details about an agent's responsibilities and abilities are configured in the application where the agent is created, not in Workfront. 
>* Task Collaborators currently support agents created in Copilot Studio, Claude, and Writer.ai.
>* For information and instructions about creating a Task Collaborator in Workfront, see [Configure a Task Collaborator](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) in the article Configure AI Collaborators.

## Assign a Task Collaborator to a task

Task collaborators are assigned to tasks the same way users are assigned.

For instructions, see [Assign tasks](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).
