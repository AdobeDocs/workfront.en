---
title: 'AI Assistant overview'
content-type: reference
description: AI Assistant overview
author: Becky
feature: Get Started with Workfront
---
# AI Assistant overview

>[!IMPORTANT]
>
>The Workfront AI Assistant has been temporarily removed and it will be available at a later date.

Workfront's AI Assistant helps you accomplish your work by offering in-app information and suggestions in a natural-language conversation. AI Assistant can give you a smoother work experience by

* Summarizing work items or documents
* Finding instructions or reference material for work processes
* Generating or checking formulas for calculated fields  

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>New: Any</p>
       <p>or</p>
       <p>Current: Not available</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>or</p>
       <p>Current: Not available</p></td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).## Prerequisites to AI Assistant

To enable AI Assistant for your organization, **all** of the following must apply:

* Your organization must have migrated to Adobe IMS (Identity Management System)
* The Adobe Unified Experience must be enabled
* Your organization must have a Select, Prime, or Ultimate Workfront plan
* Adobe must have a signed Adobe Gen AI agreement on file

   For more information on signing the agreement, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in this article.

## Considerations about AI Assistant

* AI Assistant is context sensitive to the page that you have open. For example, entering "Summarize this project" into AI Assistant on a project page returns a summary of that specific project.
* The Workfront administrator must enable AI Assistant for users in your organization. AI Assistant is enabled through access levels.

   For more information, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Workfront Planning AI Assistant has different features than Workfront AI Assistant. 

   For more information about AI Assistant in Workfront Planning, see [Adobe Workfront Planning AI Assistant overview](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).


## Functionality available in AI Assistant

AI Assistant currently offers the following functionality:

* Summarizing projects, tasks, issues, or documents.

   For more information, see [Summarize using AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Providing instructions or reference information pulled from the Workfront documentation on Adobe Experience League.

   For more information, see [Get help from AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Generate or refine formulas for calculated custom fields.

   >[!NOTE]
   >
   >This functionality is available only to organizations on the Prime or Ultimate Workfront plans.

   For more information, see [Generate or revise calculated field formulas with AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

## Access AI Assistant

1. At the top of any Workfront page, click the AI Assistant icon ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Type your question or prompt into the panel at the right of the screen.

   If you cannot type into this panel, your organization does not have a signed Adobe Gen AI agreement on file.

1. If AI assistant does not provide the answer you need, refine your prompt and try again.

## Sign the Adobe Gen AI agreement

If your organization does not have a signed Adobe Gen AI agreement on file, AI Assistant can not be enabled for your organization.

If a user attempts to use AI Assistant when the Adobe Gen AI agreement has not been signed, they will see a message:

* Users: Users are informed that AI Assistant has not been enabled for their organization, and that they can contact their Workfront administrator to request it for their organization.
* Administrators: Administrators are informed that there is not a signed Adobe Gen AI agreement, and can request that a copy of the agreement be sent for signing.

To request the Adobe Gen AI agreement:

1. As a Workfront Administrator, click the AI Assistant icon ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Begin typing in the AI Assistant panel.
1. When the Adobe Gen AI agreement message appears, click **Review agreement**.
1. Enter the name and email address of the individual at your organization who will sign the Adobe Gen AI agreement.

   The agreement will be sent to this individual for signing. After it is signed and returned, AI Assistant is enabled for your organization.

