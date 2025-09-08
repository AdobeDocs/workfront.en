---
title: Auto-fill a request using prompts or documents
content-type: reference
description: You can use AI to auto-fill request fields by entering a prompt or supplying a document.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
---
# Auto-fill a request using prompts or documents

>[!NOTE]
>
>* This functionality will be available as an open beta on the following schedule:
>
>   * Monthly release: September 11, 2025
>   * Quarterly release: October 16, 2025
>
>* To use this functionality, your organization must meet the requirements to use the Workfront AI Assistant. For details, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

AI can help you auto-fill request fields based on a prompt you enter. It can also fill fields based on text such as emails ar uploaded documents. You can approve or reject these suggestions before submitting the request.

Auto-fill does not overwrite any fields that you have already filled in.

Users do not receive suggestions of data that they do not otherwise have access to.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p>  </td> 
  </tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

To auto-fill requests using a prompt or document, **all** of the following must apply:

* Your organization must have migrated to Adobe IMS (Identity Management System)
* The Adobe Unified Experience must be enabled
* Your organization must have a Select, Prime, or Ultimate Workfront plan
* Adobe must have a signed Adobe Gen AI agreement on file

   For more information on signing the agreement, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in the article AI Assistant overview.
* AI Assistant must be enabled in your organization's system settings. This is managed by your Workfront administrator.

   For more information on enabling AI Assistant in system settings, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Get suggestions from a text prompt

Auto-fill can suggest field values based on text such as emails. You paste in a text block, and Workfront processes the text to suggest field values based on the text.

For example, If the email includes "This is due on June 1," and the request form has a field for due date, Workfront would suggest June 1 for that field value.

This type of suggestion also checks previous requests for similar contexts. For example if the prompt mentions that the request is for a certain client, Workfront can locate and enter the billing address for that client automatically, based on previous requests.

You can paste in text to be applied to the entire form, or to a single section of the form.

To use suggestions based on a pasted text prompt:

1. Begin creating a request.

   For instructions, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. To apply the text prompt to the entire form, click the AI icon ![AI icon](assets/request-prompt-icon.png) under the form name.

   Or

   To apply the text prompt for a single section, click the AI icon ![AI icon](assets/request-prompt-icon.png) next to the section name.

1. Paste the text into the prompt box.
1. Click **Fill the form**.

   Workfront generates suggestions for the form.
1. For each field suggestion, select **Accept** or **Reject** for that field.

   ![Accept or reject suggestion](assets/accept-reject-suggestion.png)

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions. 

   >[!NOTE]
   >
   >Any unreviewed suggestions will be automatically accepted when you submit the request.

### Text prompt examples

These examples show prompts for various ways that the AI can reference other projects.

* Referencing a past customer campaign

   >[!BEGINSHADEBOX]

   Create a similar campaign request as we did for (Client Company)'s Q2 launch, but this time for their Automotive division. Keep the same deliverable set and audience profile.

   >[!ENDSHADEBOX]

* Building on an existing project

   >[!BEGINSHADEBOX]

   Use the same setup we had in the (Client Company) project kickoff last spring. I want to run a digital ad campaign targeting the same executive audience, but with updated dates for this quarter.

   >[!ENDSHADEBOX]

* Reusing a style from a past deliverable

   >[!BEGINSHADEBOX]

   Prepare a request similar to the (Client Company) summer promotion campaign we ran last year. Focus on social media assets, keep Spanish as the primary language, and adjust the budget to $75,000.

   >[!ENDSHADEBOX]
   
* Expanding on an older campaign type

   >[!BEGINSHADEBOX]

   Take the (Client Company) webinar series campaign from Q1 as a reference. I want the same registration workflow and assets, but this time the topic is 'AI in Financial Planning' and the audience is young professionals.

   >[!ENDSHADEBOX]

* Repeating a request for a different product

   >[!BEGINSHADEBOX]

   Set up a campaign request just like the (Client Company) rebranding project we handled, but replace with (New Client Company) as the client. Keep all deliverables aligned to corporate branding.

   >[!ENDSHADEBOX]

* Narrative style with implicit references

   >[!BEGINSHADEBOX]
 
   We're planning a campaign similar to the holiday social ads we ran last year. Budget should be about 50k, goal is lead generation, and deliverables should include Instagram and TikTok assets.

   >[!ENDSHADEBOX]

   
## Get suggestions based on a document you upload

Auto-fill can suggest field values based on a document you upload. 

This type of suggestion also checks previous requests for similar contexts. For example if the prompt mentions that the request is for a certain client, Workfront can locate and enter the billing address for that client automatically, based on previous requests.

### Document upload guardrails

#### Supported file types

The following file types are supported:

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### Supported file size

Each file can be up to 100 MB in size

#### Number of files

You can upload up to 50 files (pages, slides, or sheets).

>[!IMPORTANT]
>
>Documents are converted to a series of images, each of which is considered a separate file. 
>
>For example, you can upload one PowerPoint with 50 slides, or 5 Word documents that each have 10 pages.

#### Supported field types

Workfront field types affect whether a given field can be auto-filled.

<table>
<tr>
<td><b>Supported </b><br> Auto-fill can fill</td>
<td><b>Unsupported</b> <br>Auto-fill does not fill</td>
</tr>
<tr>
<td>
<ul>
<li>Single line text</li>
<li>Text area or paragraph</li>
<li>Date field</li>
<li>Checkbox</li>
<li>Radio buttons</li>
<li>Single and Multi Select dropdowns</li>
</ul>
</td>
<td><li>Typeahead</li>
<li>External lookup</li>
<li>Internal lookup</li>
<li>Reference</li>
<li>WF Planning embedded fields</li>
</ul>
</td>
</tr>
</table>

#### Other best practices

Consider the following when uploading a document for request auto-fill:

* Auto-fill is currently optimized for the Latin alphabet.
* We recommend using an 8 point or larger text size.
* Auto-fill may have difficulty with images in the document, such as rotated or distorted images, graphs, and counting or using spatial reasons on objects in images.
* As always, we recommend checking results for accuracy before submitting the request.

### Upload a document to auto-fill a request

You can upload a document to be applied to the entire form, or to a single section of the form. 

1. Begin creating a request.

   For instructions, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. To apply the document to the entire form, click the AI icon ![AI icon](assets/request-prompt-icon.png) under the form name.

   Or

   To apply the document for a single section, click the AI icon ![AI icon](assets/request-prompt-icon.png) next to the section name.

1. Click **Upload files**, then select the file from your file manager.

   Or
   
   Drag the document from your file manager to the **Upload files to auto-fill request form** box.
1. Click **Fill the form** of **Fill the section**.

   Workfront generates suggestions for the form.
1. For each field suggestion, select **Accept** or **Reject** for that field.

   ![Accept or reject suggestion](assets/accept-reject-suggestion.png)

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions. 

   >[!NOTE]
   >
   >Any unreviewed suggestions will be automatically accepted when you submit the request.

## Troubleshooting

If you are not getting the expected suggestions, it may be due to one of the following:

* You must have at least one month of request data in the system before it can suggest field values from previous requests.
* You may not have followed the document upload guardrails when uploading a document to pull suggestions from. For more information, see [Document upload guardrails](#document-upload-guardrails) in this article.
