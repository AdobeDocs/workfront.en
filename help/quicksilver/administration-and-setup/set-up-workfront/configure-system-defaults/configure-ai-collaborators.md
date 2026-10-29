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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
---
# Configure AI Collaborators

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>

AI Collaborators are a way to onboard AI agents into your projects, tasks, and issues. You can configure an AI Collaborator, then assign it as you would a user.

For example, you can configure a reviewer-type AI Collaborator with brand guidelines, then assign that collaborator to review a document.

Available AI Collaborator types include:

* AI Reviewer: Create a collaborator using brands or Adobe Brand Intelligence, then assign the collaborator as a reviewer on assets.

   For more information, see [Get started with the Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Work Agent: Create a collaborator <span class="preview">powered by Adobe CX Coworker,</span> or connect an agent from a supported external platform, then assign the collaborator to a task or issue to complete work items.

   For more information, see [Use Work Agents](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

   For more information on Adobe CX Enterprise Coworker, see [Overview of CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

<!-- BECKY CHECK ME: Why this changed: we updated the Work Agent description to include Adobe Native and need product confirmation on any additional package, license, agreement, credit, or administrator restrictions before publishing. -->

Licenses used by AI Collaborators are not billed. If your organization has 200 Workfront licenses and creates an AI Collaborator, 201 licenses are then in use, but only 200 are billed.

<!--
* <span class="preview">Project Coordinator: An out-of-the-box collaborator that monitors project status and follows up on overdue tasks automatically, without needing to configure an external agent.</span>

   <span class="preview">For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>
-->


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
   <td>[!UICONTROL System Administrator] or Group Administrator</span></td> 
  </tr> 
  </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

* [For AI Reviewers](#for-ai-reviewers)
* [For Work Agents](#for-work-agents)

### For AI Reviewers:

* Your organization must have a signed Adobe Gen AI Agreement on file. 

   For more information, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in the article AI Assistant in Workfront.
* You must have configured a brand in Workfront before you can use it for an AI Reviewer.

   For instructions, see [Create and manage brands for the AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* To use Adobe Brand Intelligence for an AI Reviewer, your organization must use the unified review and approval experience in Workfront.

   For more information, see [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

### For Work Agents

<span class="preview">The prerequisites depend on the agent's origin:</span>

* <span class="preview">Adobe Native: Your organization must have Adobe CX Coworker enabled. You do not need to configure an agent in an external platform or provide external-platform credentials.</span>
* External platform or custom agent: Configure the agent in the platform you plan to connect before creating the Work Agent in Workfront.

>[!NOTE]
>
>We aim to connect with any agent provider, so if the provider you are using is not currently compatible with Work Agents, please reach out to your account team for assistance.

<!-- BECKY CHECK ME: Why this changed: we separated Native and external-agent prerequisites to match the draft, and we still need product confirmation on the final setup and entitlement requirements before removing the qualifiers. -->

## Create a new AI Reviewer

AI Reviewers can be configured to use Workfront brands, or Adobe Brand Intelligence.

* **Brands**: Brands are created in Workfront. You can create brands in Workfront by uploading PDF files that contain your brand guidelines or by manually entering brand elements.
* **Adobe Brand Intelligence**: When an AI Collaborator reviews an asset using Adobe Brand Intelligence, you can view comments made by the AI Reviewer in Frame.io.


{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Click **Reviewer**, then click **Continue**.
1. In the Collaborator Name field, enter a name for the collaborator. This is the name that appears in the list of available assignees on a task.
1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.
1. (Conditional) If the AI Collaborator will use a Brand, select the brand and brand guideline that it will use.
1. Click **Save**.

## Configure a Work Agent

<span class="preview">The following setup guidance reflects Adobe Native support and the origin-based setup model that is still in preview.</span>

Work Agents are agents that you can assign to tasks or issues in Workfront. You configure the Work Agent with a name, access level, and other details, and assign it to a task as you would assign a user. 

Because Work Agents are agents, their actions and abilities are configured where you configure your agents. Work Agents can be <span class="preview">Native Work Agents that use Coworker,</span> or can be from a supported external platform such as Copilot Studio, Claude, OpenAI, and IBM.

>Work Agents can be assigned to tasks or issues.

<!-- BECKY CHECK ME: Why this changed: we broadened the origin language to include Adobe Native and want product confirmation on whether the release should describe it as a ready-to-use origin and whether the external-agent setup language still matches production. -->

Licenses used by work agents are not billed. If your organization has 200 Workfront licenses and creates a Work Agent, 201 licenses are then in use, but only 200 are billed.

For a list of best practices when creating an agent to work as a Work Agent, see [Best practices for creating an agent for a Work Agent](#best-practices-for-creating-an-agent-for-a-work-agent).

* [Configure a Work Agent in Workfront](#configure-a-work-agent-in-workfront)
* [Best practices for creating an agent for a Work Agent](#best-practices-for-creating-an-agent-for-a-work-agent)

### Configure a Work Agent in Workfront

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Work agents**, then click **Continue**.
1. In the AI Collaborator Name field, enter a name for the collaborator. This is the name that appears in the list of available assignees on a task.
1. In the AI Collaborator description field, enter a description of the collaborator's purpose or the actions it performs.
1. In the Access Level field, select an access level for this collaborator. This access level controls what the collaborator can do, in the same way an access level controls what a user can do.
1. (Optional) In the Groups field, select the groups that the Work Agent will be associated with.

   >[!NOTE]
   >
   >If you are a group administrator, this field displays only groups that you are an administrator for. Group administrators must select at least one group.

1. In the **Choose agent's origin** area, select whether you want to <span class="preview">use Adobe Native</span>, connect an agent created in a common platform such as Copilot, or use a custom agent.
1. <span class="preview">(Conditional) If you select Adobe Native, confirm that Adobe CX Coworker is enabled for your organization and that you want to use the ready-to-use Adobe Native agent.</span>
1. (Conditional) If you are using an agent from a common platform, enter authentication details for the agent's platform:

   |Platform|Required authentication|
   |---|---|
   |Copilot Studio|Web channel secret|
   |Claude Managed Agents|Anthropic API key<br>Agent ID<br>Environment ID|
   |OpenAI Agents|API key <br>Agent ID|
   |IBM watsonx Orchestrate|Service URL<br>API Key<br> Agent ID|

1. Click **Test connection**. This lets you know whether the connection was set up correctly.
1. In the **After the Collaborator is finished with its work, it can** area, toggle on the actions that you want the collaborator to take. 
   
   * Send notification: The Agent makes a comment in the update stream, tagging the user that requested the work, assigned the Agent, or that owns the project. 
   * Upload text-based documents
   * Mark task complete
   * Write task fields: Select the forms and fields that the Agent can write to. 
   * Write project fields: Select the forms and fields that the Agent can write to. 

1. Click **Save**.

For more information on Work Agents, including how to assign them to tasks, see [Use Work Agents](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

### Best practices for creating an agent for a Work Agent

You may find the following best practices helpful when creating an agent to use as a Work Agent in Workfront. To see best practices, click the section for the application where you are creating the agent.

+++ Claude

1. Navigate to the Claude Console at [platform.claude.com](https://platform.claude.com/).
1. Create an API key.
   1. Under API Keys, click **Create Key** in the upper-right corner.
   1. Provide a name and expiration date.
   1. Copy the key and save it somewhere safe and secure. You will need this key to configure the Work Agent in Workfront.

1. Create an environment.
   1. Under **Managed Agents** > **Environments**, click **Create Environment** in the upper-right corner.
   1. Provide a name and hosting type as applicable.
   1. Configure shared packages and metadata as needed. Environments can be reused across multiple agents and allow for shared packages and metadata.
      The environment ID appears below the environment name in the upper-left corner.

1. Create an agent.
   1. Under Managed Agents > Agents, click **Create Agent** in the upper-right corner.
   1. Provide a name, model, system prompt, skills, and tools as applicable. Be descriptive, because Work Agents pass task context through to this agent, which then executes the work.
     The agent ID appears below the agent name in the upper-left corner.

1. Configure the Work Agent in Workfront.
   1. Enter your API key, environment ID, and agent ID
   1. Click **Test Connection** to verify.

1. Assign the Work Agent to a Workfront task.
   1. The Work Agent fires after all predecessor tasks are complete.

+++
<!--
+++ Copilot Studio


+++
-->
+++ Writer



>[!IMPORTANT]
>
>Writer has deprecated their use of agents. Work Agents configured using Writer agents no longer work after October 9. 2026.
>
>For information on the deprecation, see [Agent Library migration & deprecation](https://support.writer.com/articles/8335689949-migrating-no-code-agents) in the Writer documentation.


<!--

>[!NOTE]
>
> You can use a Writer agent as a Work Agent, but Writer playbooks cannot be used as Work Agents.

When creating an agent for use as a Work Agent in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need them to configure the Work Agent in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Work Agent in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Work Agent to a Workfront task. The Work Agent begins work when all of the task's predecessor tasks are complete.

-->

+++

<div class="preview">

<!--
## Configure a Project Coordinator

The Project Coordinator is an out-of-the-box collaborator that monitors project status and helps keep work on track. Unlike Work Agents, the Project Coordinator does not require you to configure an external agent.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Project Coordinator**.
1. In the **AI Collaborator name** field, enter a name for the Project Coordinator. This is the name that appears as the collaborator in your project.
1. In the **AI Collaborator description** field, enter a description of what the Project Coordinator does or its purpose.
1. In the **Access level** field, select an access level for the Project Coordinator. This access level controls what the collaborator can do on projects.
1. (Optional) In the **Send project updates** section, toggle **Allow** to enable project update notifications, then specify update details.
   * In the **Cadence** field, select whether the Coordinator sends updates daily or weekly.
   * If the Coordinator sends updates weekly, in the **Day of week** field, select the day of the week that updates are sent.
   * In the **Time (MST)** field, select the time to send updates.
   * In the **How to send** field, select whether the Coordinator sends updates as an update on the project, or as an email
   * In the **Who gets the update** field, select whether the update is sent only to the project owner, or to all project stakeholders.
   * (Optional) Check **Send additional update immediately when coordinator is assigned** to notify on assignment.
   * (Optional) Check **Send additional update when a date is missed** to send notifications when dates are missed.
1. (Optional) In the **Notify task assignees** section, toggle **Allow** to enable task notifications, then check the boxes for the situations that you want to notify assignees about.
1. (Optional) In the **Remind reviewers and approvers** section, toggle **Allow** to enable reminders for reviewers, then check the boxes for the situations that you want to remind reviewers and approvers about.
1. (Optional) In the **Update the content of project and task fields** section, toggle **Allow** to enable the coordinator to update project and task field values.
1. Click **Save**.

For more information on the Project Coordinator, including how to assign it to projects, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).
-->

</div>

## Manage AI Collaborators

You can edit, copy, and delete existing AI Collaborators. 

>[!NOTE]
>
>Group administrators can view and interact with only AI Collaborators associated with groups that they are administrators for. If other groups are also associated with a given AI Collaborator, a group administrator can view but not edit it.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. (Conditional) To edit a Collaborator, click the name of the Collaborator you want to edit, make any edits in the Edit Collaborator window, and click **Save**.
1. (Conditional) To delete a Collaborator, click the Delete icon ![Delete icon](assets/delete-collaborator-icon.png) in the row of the AI Collaborator you want to delete, then click **Delete**.
