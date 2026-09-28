---
title: Use Work Agents
content-type: reference
description: Learn how to use Work Agents, AI Collaborators that can be assigned to Workfront tasks.
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Use Work Agents

Work Agents are AI Collaborators that can be assigned directly to Workfront tasks, in addition to the existing AI Reviewer used for document and asset reviews. Like other AI Collaborators, Work Agents are configured in the Setup area and assigned to tasks just like a user.

Work Agents connect to agents that you have configured in Copilot Studio, Claude, or Writer.

For information and instructions about creating a Work Agent in Workfront, see [Configure a Work Agent](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) in the article Configure AI Collaborators.

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

* You must configure an agent in Copilot, Claude, or Writer.ai before you can use it as a Work Agent.

## Work Agent overview

Work Agents are a way to assign MCP agents to specific tasks in Workfront. You configure the agent in an app such as Copilot Studio, Claude, or Writer.ai, then connect that agent to Workfront as a Work Agent. You can then assign it to tasks as you would assign a user. 

Some example workflows may include:

* Detecting images uploaded to a task, generating variations based on criteria given to the agent, and uploading the new images to the task.
* Generating copy from a task description, reviewing the copy against guidelines configured in the agent, and posting copy to the update stream.
* Reading details of an event, identifying missing details, and posting questions in the update stream about the missing details.

>[!NOTE]
>
>* Specific details about an agent's responsibilities and abilities are configured in the application where the agent is created, not in Workfront. 
>* The Workfront MCP server does not need to be added to the agent used as a Work Agent, and does not need to be connected for the Work Agent to work.
>* Work Agents currently support agents created in Copilot Studio, Claude, and Writer.ai.
>* When configuring an agent in Copilot Studio, you must set security to **No authentication**.
>* For information and instructions about creating a Work Agent in Workfront, see [Configure a Work Agent](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) in the article Configure AI Collaborators.

## Information a Work Agent reads

When a Work Agent begins work on a task, it automatically reads the following task information as context:

* Task title
* Task description
* Comments in the task's update stream
* Information in any custom form attached to the task

This information is always read and is not configurable as a Workfront setting.

>[!TIP]
>
>For best results, we recommend:
>
>* Including any background information you want the agent to use directly in the task description or a relevant custom form field.
>* Making sure the task matches what your agent is instructed to do. For example, if your agent is instructed to translate text from English to French, include the text you want translated in the task description.

## Work Agent start triggers

When a Work Agent is assigned to a task, it begins work when any of the following situations are met:

* The Work Agent is assigned to a task that is ready to start. (For example, if the task has predecessors, the predecessors are complete.)
* The Work Agent and a user are assigned to a task, and the Work Agent is assigned first.
* A task to which a Work Agent is already assigned as becomes ready to start, and the Work Agent is the only or primary assignee. (For example, if the task has predecessors, the predecessors are complete.)
* A task to which a Work Agent and a user are already assigned becomes ready to start, and the Work Agent was assigned first or is the primary assignee. (For example, if the task has predecessors, the predecessors are complete.)
* A user and a Work Agent are assigned to a task, and the user is removed.
* A user and a Work Agent are assigned to a task, and the Work Agent is set as the Primary Assignee for the task.

The following situations do not cause the Work Agent to begin work on the task:

* A Work Agent is assigned to a task that already has a user assigned.
* A Work Agent is @mentioned in a task.
* A Work Agent is assigned to a task that already has a Work Agent assigned. In this case, the first Work Agent assigned will have already begun the work, and the second Work Agent will do nothing.
* A Work Agent is assigned to a task that is not ready to start. (For example, if the task has predecessors, the predecessors are not yet complete.)

## Assign a Work Agent to a task

Work Agents are assigned to tasks the same way users are assigned.

When you are searching for a Work Agent in the list of available assignees, the name of the Work Agent is a first name only.

For instructions, see [Assign tasks](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

>[!NOTE]
>
>Work Agents cannot be assigned to review or approve a document.

## Troubleshooting Work Agents

If your Work Agent does not return a response or output, please check the following:

* Make sure your agent is published on the AI platform provider side.
* Make sure you have sufficient AI credits with your agent's platform.
* Make sure the the action taken on the task does not require a specific access level.
* If you are using Copilot as the agent provider, ensure you are using the "no authentication" setting.
* If you are using Copilot, make sure that your agent is configured on a global environment. Work Agent functionality does not currently support regional versions of Copilot Studio. 
* Make sure that the Collaborator is the primary assignee on the task.
* Make sure that the task that the Work Agent is assigned to Can Start. For example, check to see that all task predecessors to that task are complete.

>[!TIP]
>
>You can also go to the agent provider platform and ask the agent to perform the task within the platform. If the agent cannot perform the task within the platform, then the Work Agent will also run into issues in Workfront.
