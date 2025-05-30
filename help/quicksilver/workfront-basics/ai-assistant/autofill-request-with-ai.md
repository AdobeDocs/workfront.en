---
title: Auto-fill a request using AI
content-type: reference
description: You can use AI to auto-fill request fields.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
---
# Auto-fill a request using AI

>[!NOTE]
>
>This functionality is currenty part of a closed beta. To  have this functionality enabled, please contact sargism@adobe.com.
>
>To qualify for the closed beta, your organization must meet the requirements to use the Workfront AI Assistant. For details, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

AI can help you auto-fill request fields. It can suggest field values based on previous requests, or parse them from text such as emails ar uploaded documents. 

You can approve or reject these suggestions before submitting the request.

Auto-fill does not overwrite any fields that you have already filled in.

## Get suggestions when filling out form 

Auto-fill can suggest field values while you are filling out the form. As you enter values into the request fields, Workfront compares those values with previous requests. If the entered value closely correlates with other field values in similar contexts in previous requests, Workfront suggests those values.

For example, if a clinic always uses the same billing code, Workfront would suggest that billing code in the appropriate field when the clinic name is entered.

To use suggestions based on previous requests:

1. Begin creating a request.

   For instructions, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Begin filling in fields.

   As you fill in fields, other fields may show suggestions.

1. For each field suggestion, select **Accept** or **Reject** below that field.

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions. 

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
1. For each field suggestion, select **Accept** or **Reject** below that field.

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions.
   
## Get suggestions based on a document you upload

Auto-fill can suggest field values based on a document you upload. 

This type of suggestion also checks previous requests for similar contexts. For example if the prompt mentions that the request is for a certain client, Workfront can locate and enter the billing address for that client automatically, based on previous requests.

### Document upload guardrails

#### Supported file types

The following file types are supported:

   * BMP
   * CSV
   * DOC
   * DOCX
   * GIF
   * JPEG
   * JPG
   * ODP
   * ODS
   * ODT
   * PDF
   * PNG
   * PPT
   * PPTX
   * RTF
   * TIFF
   * TXT
   * XLS
   * XLSX

#### Supported file size

Each file can be up to 100 MB in size

#### Number of files

You can upload up to 50 files (pages, slides, or sheets).

>[!IMPORTANT]
>
>Documents are converted to a series of images, each of which is considered a separate file. 
>
>For example, you can upload one PowerPoint with 50 slides, or 5 Word documents that each have 10 pages.

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
1. For each field suggestion, select **Accept** or **Reject** below that field.

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions.
