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

>[!IMPORTANT]
>
>Currently, Content Reviewer is the only available AI Collaborator type. More AI Collaborator capabilities will be available in the future.

AI Collaborators are a way to onboard AI agents into your projects and tasks. You can configure an AI Collaborator, then assign it as you would a user.

For example, you can configure a reviewer-type AI Collaborator with brand guidelines, then assign that collaborator to review a document.

Available AI Collaborator types include:

* Reviewer: Create a collaborator using brands or Adobe Brand Intelligence, then assign the collaborator as a reviewer on assets.

   For more information, see [Get started with the Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).


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
* <span class="preview">To use Adobe Brand Intelligence for a Reviewer AI Collaborator, your organization must use the unified review and approval experience in Workfront. </span>

   <span class="preview">For more information, see [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md). </span>

## Create a new Reviewer-type AI Collaborator

Reviewer AI Collaborators can be configured to use Workfront brands, or Adobe Brand Intelligence.

* **Brands**: Brands are created in Workfront. You can create brands in Workfront by uploading PDF files that contain your brand guidelines or by manually entering brand elements.
* <span class="preview">**Adobe Brand Intelligence**: When an AI Collaborator reviews an asset using Adobe Brand Intelligence, you can view comments made by the Reviewer in Frame.io.  </span>

>[!NOTE]
>
>Content Reviewer is not available in Sandbox environments.


{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Click **Reviewer**, then click **Continue**.

   >[!NOTE]
   >
   >Currently, only the Reviewer type is available. More AI Collaborator types will be available in the future.

1. In the Collaborator Name field, enter a name for the collaborator. This is the name that appears in the list of available assignees on a task.
1. <span class="preview">Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.</span>
1. (Conditional) If the AI Collaborator will use a Brand, select the brand and brand guideline that it will use.
1. Click **Save**.

## Manage AI Collaborators

You can edit, copy, and delete existing AI Collaborators.   

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. (Conditional) To edit a Collaborator, click the name of the Collaborator you want to edit, make any edits in the Edit Collaborator window, and click **Save**.
1. (Conditional) To copy a Collaborator, click the Copy icon ![Copy icon](assets/copy-ai-collaborator.png) in the row of the AI Collaborator you want to copy, click the name of the copy, make any edits in the Edit Collaborator window, and click **Save**.
1. (Conditional) To delete a Collaborator, click the Delete icon ![Delete icon](assets/delete-collaborator-icon.png) in the row of the AI Collaborator you want to delete, then click **Delete**.
