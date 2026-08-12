---
title: Use Task Collaborators
content-type: reference
description: Learn how to use Task Collaborators, AI Collaborators that can be assigned to Workfront tasks.
author: Becky
feature: Work Management, Tasks

---
# Use Task Collaborators

{{highlighted-preview-article-level}}

Task Collaborators are AI Collaborators that can be assigned directly to Workfront tasks, in addition to the existing Reviewer-type AI Collaborator used for document and asset reviews. Like other AI Collaborators, Task Collaborators are configured in the Setup area and assigned to tasks just like a user.

Task Collaborators connect to agents that you have configured, much like an MCP server. 

For information and instructions about creating a Task Collaborator in Workfront, see [Configure a Task Collaborator](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) in the article Configure AI Collaborators.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Select, Prime, or Ultimate</p></td> 
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

## Task Collaborator overview

Task Collaborators are a way to assign MCP agents to specific tasks in Workfront. You configure the agent in an app such as Copilot Studio, Claude, or Writer.ai, then connect that agent to Workfront as a Task Collaborator. You can then assign it to tasks as you would assign a user. 

Some example workflows may include:

* Detecting images uploaded to a task, generating variations based on criteria given to the agent, and uploading the new images to the task.
* Generating copy from a task description, reviewing the copy against guidelines configured in the agent, and posting copy to the update stream.
* Reading details of an event, identifying missing details, and posting questions in the update stream about the missing details.

>[!NOTE]
>
>* Specific details about an agent's responsibilities and abilities are configured in the application where the agent is created, not in Workfront. 
>* Task Collaborators currently support agents created in Copilot Studio, Claude, and Writer.ai.
>* When configuring an agent in Copilot Studio, you must set security to **No authentication**.
>* For information and instructions about creating a Task Collaborator in Workfront, see [Configure a Task Collaborator](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) in the article Configure AI Collaborators.

## Task Collaborator start triggers

When a Task Collaborator is assigned to a task, it begins work when any of the following situations are met:

* The Task Collaborator is assigned to a task that is ready to start. (For example, if the task has predecessors, the predecessors are complete.)
* The Task Collaborator and a user are assigned to a task, and the Task Collaborator is assigned first.
* A task to which a Task Collaborator is already assigned as becomes ready to start, and the Task Collaborator is the only or primary assignee. (For example, if the task has predecessors, the predecessors are complete.)
* A task to which a Task Collaborator and a user are already assigned becomes ready to start, and the Task Collaborator was assigned first or is the primary assignee. (For example, if the task has predecessors, the predecessors are complete.)
* A user and a Task Collaborator are assigned to a task, and the user is removed.
* A user and a Task Collaborator are assigned to a task, and the Task Collaborator is set as the Primary Assignee for the task.

The following situations do not cause the Task Collaborator to begin work on the task:

* A Task Collaborator is assigned to a task that already has a user assigned.
* A Task Collaborator is @mentioned in a task.
* A Task Collaborator is assigned to a task that already has a Task Collaborator assigned. In this case, the first Task Collaborator assigned will have already begun the work, and the second Task Collaborator will do nothing.
* A Task Collaborator is assigned to a task that is not ready to start. (For example, if the task has predecessors, the predecessors are not yet complete.)

## Assign a Task Collaborator to a task

Task Collaborators are assigned to tasks the same way users are assigned.

When you are searching for a Task Collaborator in the list of available assignees, the name of the Task Collaborator is a first name only.

For instructions, see [Assign tasks](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

## Troubleshooting Task Collaborators

If your Task Collaborator does not return a response or output, please check the following:

* Make sure your agent is published on the AI platform provider side.
* Make sure you have sufficient AI credits with your agent's platform.
* Make sure the the action taken on the task does not require a specific access level.
* If you are using Copilot as the agent provider, ensure you are using the "no authentication" setting.
* If you are using Copilot, make sure that your agent is configured on a global environment. Task Collaborator functionality does not currently support regional versions of Copilot Studio. 
* Make sure that the Collaborator is the primary assignee on the task.
* Make sure that the task that the Task Collaborator is assigned to Can Start. For example, check to see that all task predecessors to that task are complete.

>[!TIP]
>
>You can also go to the agent provider platform and ask the agent to perform the task within the platform. If the agent cannot perform the task within the platform, then the Task Collaborator will also run into issues in Workfront.
