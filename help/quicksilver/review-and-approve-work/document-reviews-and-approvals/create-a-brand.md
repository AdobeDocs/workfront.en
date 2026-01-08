---
product-area: documents
navigation-topic: approvals
title: Set up brands for the AI Reviewer
description: Set up brands for the AI Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog

---
# Set up brands for the AI Reviewer

>[!IMPORTANT]
>
>This feature is currently in beta. 

The AI Reviewer uses brand guidelines to evaluate content during the review process. You can create brands in Workfront by uploading PDF files that contain your brand guidelines or by manually entering brand elements.

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
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Prerequisites 

* Your organization must have migrated to Adobe IMS (Identity Management System).
* Your Workfront instance must have Unified Approvals enabled. 
* Your organization must have GenStudio Foundation.
* Adobe must have a signed Adobe Gen AI agreement on file.
    For more information on signing the agreement, see [Sign the Adobe Gen AI agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## Create a brand using a PDF

{{step-1-to-setup}}

1. In the left panel, go to **Review and Approval** > **Brands**.
1. Click **Add brand** in the top-right corner of the screen.
1. Name the brand. 
1. Click Upload PDFs to upload brand files. 
1. Upload one or more PDF files that contain your brand guidelines. 
1. Click **Add brand**. 
1. Once the files are uploaded, review the extracted brand elements to ensure they align with your brand guidelines. 

    >[!IMPORTANT]
    >
    >Guidelines are generated using your file(s) and generative AI technology and may be inaccurate. Review extracted guidelines for missing or incorrect details and edit them before you publish this brand.

1. When finished, click **Publish** to make the brand available for the AI Reviewer.





## Create a brand manually

{{step-1-to-setup}}

1. In the left panel, go to **Review and Approval** > **Brands**.
1. Click **Add brand** in the top-right corner of the screen.
1. Name the brand.
1. Click **Add manually** to create a brand with individual elements.

When to use
Voice guidelines
Image guidelines
Channel guidelines
logos
Colors

Publish brand


customer questions:

Lilly has some questions on this - Yes
1- Do brands update directly to GS Brands when updated in WF?
2- Is there a way to block this aspect in WF for users so they have to use brands in GS?


It's the same brands in both places, its just reflected in WF so they dont have to go back and forth. Brands created in GS show here and vice versa
Yes (once enabled)