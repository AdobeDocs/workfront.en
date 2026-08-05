---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: Configure AI Collaborators
description: As an Adobe Workfront administrator, you can configure AI Collaborators and assign them to projects and tasks.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
---
# Configure AI Collaborators


<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>


AI Collaborators are a way to onboard AI agents into your projects and tasks. You can configure an AI Collaborator, then assign it as you would a user.

For example, you can configure a reviewer-type AI Collaborator with brand guidelines, then assign that collaborator to review a document.

Available AI Collaborator types include:

* Reviewer: Create a collaborator using brands or Adobe Brand Intelligence, then assign the collaborator as a reviewer on assets.

   For more information, see [Get started with the Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Task Collaborator: Create a collaborator using Copilot or Writer, then assign the collaborator to a task to complete task-level work.

   For more information, see [Use Task Collaborators](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


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

### For AI Reviewers:

* Your organization must have a signed Adobe Gen AI Agreement on file. 

   For more information, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in the article AI Assistant in Workfront.
* You must have configured a brand in Workfront before you can use it for a Reviewer-type AI Collaborator.

   For instructions, see [Create and manage brands for the Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* To use Adobe Brand Intelligence for a Reviewer AI Collaborator, your organization must use the unified review and approval experience in Workfront. </span>

   For more information, see [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md). </span>

<div class="preview">

### For Task Collaborators

You must configure an agent in Claude, Copilot Studio, or Writer before you can use it as a Task Collaborator. 

</div>

## Create a new Reviewer-type AI Collaborator

Reviewer AI Collaborators can be configured to use Workfront brands, or Adobe Brand Intelligence.

* **Brands**: Brands are created in Workfront. You can create brands in Workfront by uploading PDF files that contain your brand guidelines or by manually entering brand elements.
* **Adobe Brand Intelligence**: When an AI Collaborator reviews an asset using Adobe Brand Intelligence, you can view comments made by the Reviewer in Frame.io.  </span>


{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Click **Reviewer**, then click **Continue**.
1. In the Collaborator Name field, enter a name for the collaborator. This is the name that appears in the list of available assignees on a task.
1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.
1. (Conditional) If the AI Collaborator will use a Brand, select the brand and brand guideline that it will use.
1. Click **Save**.

<div class="preview">

## Configure a Task Collaborator

Task Collaborators are MCP agents that you can assign to tasks in Workfront. You configure the Task Collaborator with a name, access level, and other details, and assign it as you would assign a user. 

Because Task Collaborators are MCP agents, their actions and abilities are configured where you configure your agents. Currently, agents used as Task Collaborators can be created in Copilot Studio, Claude, or Writer.

For a list of best practices when creating an agent to work as a Task Collaborator, see [Best practices for creating an agent for a Task Collaborator](#best-practices-for-creating-an-agent-for-a-task-collaborator).

### Configure a task collaborator in Workfront

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Task agents**, then click **Continue**.
1. In the AI Collaborator Name field, enter a name for the collaborator. This is the name that appears in the list of available assignees on a task.
1. In the AI Collaborator description field, enter a description of the collaborator's purpose or the actions it performs.
1. In the Access Level field, select an access level for this collaborator. This access level controls what the collaborator can do, in the same way an access level controls what a user can do.
1. In the **Choose agent's origin** area, select whether you want to connect an agent created in an common platform such as Copilot or Writer, or use a custom agent.
1. (Conditional) If you are using an agent from a common platform, enter authentication details for the agent's platform:

   |Platform|Required authentication|
   |---|---|
   |Copilot Studio|Web channel secret|
   |Claude Managed Agents|Anthropic API key<br>Agent ID<br>Environment ID|
   |Writer|API key<br>Application ID|

1. Click **Test connection**. This lets you know whether the connection was set up correctly.
1. In the **After the Collaborator is finished with its work, it can** area, toggle on the actions that you want the collaborator to take.
1. Click **Save**.

For more information on Task Collaborators, including how to assign them to tasks, see [Use Task Collaborators](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


### Best practices for creating an agent for a Task Collaborator

You may find the following best practices helpful when creating an agent to use as a Task Collaborator in Workfront. To see best practices, click the section for the application where you are creating the agent.

+++ Claude

1. Navigate to the Claude Console at [platform.claude.com](https://platform.claude.com/).
1. Create an API key.
   1. Under API Keys, click **Create Key** in the upper-right corner.
   1. Provide a name and expiration date.
   1. Copy the key and save it somewhere safe and secure. You will need this key to configure the Task Collaborator in Workfront.

1. Create an environment.
   1. Under **Managed Agents** > **Environments**, click **Create Environment** in the upper-right corner.
   1. Provide a name and hosting type as applicable.
   1. Configure shared packages and metadata as needed. Environments can be reused across multiple agents and allow for shared packages and metadata.
      The environment ID appears below the environment name in the upper-left corner.

1. Create an agent.
   1. Under Managed Agents > Agents, click **Create Agent** in the upper-right corner.
   1. Provide a name, model, system prompt, skills, and tools as applicable. Be descriptive, because Task Collaborators pass task context through to this agent, which then executes the work.
     The agent ID appears below the agent name in the upper-left corner.

1. Configure the Task Collaborator in Workfront.
   1. Enter your API key, environment ID, and agent ID
   1. Click **Test Connection** to verify.

1. Assign the Task Collaborator to a Workfront task.
   1. The Task Collaborator fires after all predecessor tasks are complete.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Writer

>[!NOTE]
>
> You can use a Writer agent as a Task Collaborator, but Writer playbooks cannot be used as Task Collaborators.

When creating an agent for use as a Task Collaborator in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need Task Collaborator to configure the Task Collaborator in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Task Collaborator in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Task Collaborator to a Workfront task. The Collaborator begins work when all of the task's predecessor tasks are complete.

+++

</div>

## Manage AI Collaborators

You can edit, copy, and delete existing AI Collaborators.   

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. (Conditional) To edit a Collaborator, click the name of the Collaborator you want to edit, make any edits in the Edit Collaborator window, and click **Save**.
1. (Conditional) To copy a Collaborator, click the Copy icon ![Copy icon](assets/copy-ai-collaborator.png) in the row of the AI Collaborator you want to copy, click the name of the copy, make any edits in the Edit Collaborator window, and click **Save**.
1. (Conditional) To delete a Collaborator, click the Delete icon ![Delete icon](assets/delete-collaborator-icon.png) in the row of the AI Collaborator you want to delete, then click **Delete**.
