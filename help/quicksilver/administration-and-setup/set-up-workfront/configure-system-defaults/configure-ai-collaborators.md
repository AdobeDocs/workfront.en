---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
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

* Task Collaborator: Create a collaborator using Copilot or Writer.ai, then assign the collaborator to a task to complete task-level work.

   For more information, see [Use task collaborators](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


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

* Your organization must have a signed Adobe Gen AI Agreement on file. 

   For more information, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in the article AI Assistant in Workfront.
* You must have configured a brand in Workfront before you can use it for a Reviewer-type AI Collaborator.

   For instructions, see [Create and manage brands for the Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* To use Adobe Brand Intelligence for a Reviewer AI Collaborator, your organization must use the unified review and approval experience in Workfront. </span>

   For more information, see [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md). </span>

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

Task collaborators are MCP agents that you can assign to tasks in Workfront. You configure the task collaborator with a name, access level, and other details, and assign it as you would assign a user. 

Because task collaborators are MCP agents, their actions and abilities are configured where you configure your agents. Currently, agents used as task collaborators can be created in Copilot Studio, Claude, or Writer.ai.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Task agents**, then click **Continue**.
1. In the AI Collaborator Name field, enter a name for the collaborator. This is the name that appears in the list of available assignees on a task.
1. In the AI Collaborator description field, enter a description of the collaborator's purpose or the actions it performs.
1. In the Access Level field, select an access level for this collaborator. This access level controls what the collaborator can do, in the same way an access level controls what a user can do.
1. In the **Choose agent's origin** area, select whether you want to connect an agent created in an common platform such as Copilot or Writer.ai, or use a custom agent.
1. (Conditional) If you are using an agent from a common platform, enter authentication details for the agent's platform:

   |Platform|Required authentication|
   |---|---|
   |Copilot Studio|Web channel secret|
   |Claude Managed Agents|Anthropic API key<br>Agent ID<br>Environment ID|
   |Writer.ai|API key<br>Application ID|

1. (Optional) To test whether the credentials were set up correctly, click **Test connection**.
1. In the **After the Collaborator is finished with its work, it can** area, toggle on the actions that you want the collaborator to take.
1. Click **Save**.

For more information on task collaborators, including how to assign them to tasks, see [Use task collaborators](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

</div>

## Manage AI Collaborators

You can edit, copy, and delete existing AI Collaborators.   

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. (Conditional) To edit a Collaborator, click the name of the Collaborator you want to edit, make any edits in the Edit Collaborator window, and click **Save**.
1. (Conditional) To copy a Collaborator, click the Copy icon ![Copy icon](assets/copy-ai-collaborator.png) in the row of the AI Collaborator you want to copy, click the name of the copy, make any edits in the Edit Collaborator window, and click **Save**.
1. (Conditional) To delete a Collaborator, click the Delete icon ![Delete icon](assets/delete-collaborator-icon.png) in the row of the AI Collaborator you want to delete, then click **Delete**.
