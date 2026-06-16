---
product-area: documents
navigation-topic: approvals
title: Create and manage brands for the Content Reviewer
description: Create and manage brands for the Content Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ezurCOB6dbk6JPL0eY33C9nR8lXVLMHl-SUTfAbVeTg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create and manage brands for the Content Reviewer

The Content Reviewer uses brand guidelines to evaluate content during the review process. You can create brands in Workfront by uploading PDF files that contain your brand guidelines or by manually entering brand elements.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a system administrator.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console permissions*</td> 
   <td> <p>You must be a GenStudio Brand Manager.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requirements

* Your Workfront instance must have Unified Approvals enabled. 

* Your organization must have GenStudio Foundation. 
    * Content Reviewer in Workfront provides the functionality available in GenStudio Foundation for asset review and approval workflows. You do not need to access GenStudio Foundation directly to complete your work. Your access to GenStudio Foundation functionality through Content Reviewer falls under the terms of your Workfront contract.
* Adobe must have a signed Adobe Gen AI agreement on file.
    For more information on signing the agreement, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Prerequisites 

1. You must grant access to brand permissions in the Admin Console and in Workfront access levels before you can create brands. For instructions, see [Grant access to brand permissions](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md).


## Create a brand using a PDF

{{step-1-to-setup}}

1. In the left panel, go to **Review and Approval** > **Brands**.
1. Click **Add brand** in the top-right corner of the screen.
1. Name the brand. 
1. Click **Upload PDFs** to upload brand files.
    ![upload brand pdfs](assets/upload-PDF.png)
1. Click **Continue**.
1. Upload one or more PDF files that contain your brand guidelines, then click **Add brand**. 
1. Once the files are uploaded, review the extracted brand elements to ensure they align with your brand guidelines. 

    >[!IMPORTANT]
    >
    >Guidelines are generated using your files and generative AI technology and may be inaccurate. Review extracted guidelines for missing or incorrect details and edit them before you publish this brand.

1. When finished, click **Publish** to make the brand available for the Content Reviewer.

## Create a brand manually

{{step-1-to-setup}}

1. In the left panel, go to **Review and Approval** > **Brands**.
1. Click **Add brand** in the top-right corner of the screen.
1. Name the brand.
1. Click **Add manually** to create a brand with individual elements.
1. Fill in the brand details as needed. You can add the following elements:

    <table>
    <tr>
        <td>When to use</td>
        <td>Let marketers know when to use this brand.</td>
    </tr>
    <tr>
        <td>Voice guidelines</td>
        <td>Provide guidance on the tone and style of the brand's voice.</td>
    </tr>
    <tr>
        <td>Image guidelines</td>
        <td>Specify the types of images that align with the brand's identity.</td>
    </tr>
    <tr>
        <td>Channel guidelines</td>
        <td>Outline the appropriate channels for brand communication.</td>
    </tr>
    <tr>
        <td>Logos</td>
        <td>Include the official logos associated with the brand.</td>
    </tr>
    <tr>
        <td>Colors</td>
        <td>Specify the brand's color palette.</td>
    </tr>
    </table>

    ![add brand elements manually](assets/brand-elements.png)


1. When finished, click **Publish** to make the brand available for the Content Reviewer.


## Best practices for writing brand guidelines

*  Write brand guidelines that describe measurable criteria. The Content Reviewer evaluates content literally, so objective rules produce more consistent scores than subjective ones.

* Look for words like "avoid," "keep," or "make sure" in your guidelines. These often signal a rule you can tighten. Replace the vague instruction with a specific list of words, formats, or limits. For example, replace "avoid common skiing clichés" with "do not use 'gnar,' 'pow,' or 'shred.'"

* If you can't remove the subjectivity, narrow it. Replace broad adjectives with specific constraints. For example, "Direct and action-oriented" becomes "Direct and action-oriented; omit filler words and hedging language."