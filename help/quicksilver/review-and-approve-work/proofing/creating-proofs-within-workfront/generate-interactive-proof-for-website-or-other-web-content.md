---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Create an interactive proof for a website or other web content
description: You can generate a new interactive proof or a new version of an existing interactive proof for web content. This can be a website or other kinds of interactive content such as ads with streaming video or audio, HTML animations, and interactive banners.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
TQID: https://experienceleague.adobe.com/HrCGRaJ6jTF97KxhLe65Fy6I8ahbMy4hAgPUDJFvr2I
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create an interactive proof for a website or other web content

You can generate a new interactive proof or a new version of an existing interactive proof for web content. This can be a website or other kinds of interactive content such as&nbsp;ads with streaming video or audio, HTML animations, and interactive banners.

In an interactive proof, reviewers can navigate and interact as they normally would with the website or other web content.

>[!IMPORTANT]
>
>Make sure that the website or interactive content is accessible to the people who are going to review it. They can access it in the proofing process only if they can also access it on the internet.

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
   <td> 
   <p>Standard</p>
   <p>Work or Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Documents</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Create an interactive proof for a website or other web content

1. Go to the project, task, or issue where you want to create a new website proof or a new version of an existing one.
1. Click **Documents** in the left panel.
1. (Conditional) If you are creating a new proof, click **Add New**, then click **Proof** in the menu that appears.

1. (Conditional) On the **New proof** page appears, if you are creating a new version of an existing proof:

   1. Hover over the URL proof for which you want to create a new version, then select it by clicking in the light blue background surrounding it.

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. In the **Add new** drop-down, click **Version** > **Proof**.

1. In the **Add files** section, type the URL of the website you want to proof, then press **Enter**.  You can repeat this process to add multiple websites to be proofed.

   ![proof_website.png](assets/proof-website-350x65.png)

  
   >[!NOTE]
   >
   > The URL must be less than 1,000 characters.

1. Click the URL you have added.

   ![Click URL](assets/click-url-350x137.png)

1. (Optional) If you want to change the name of the proof from the website URL to something else, type a **Proof name**.
1. Select **Interactive**, then click **Done**.

   >[!NOTE]
   >
   >If you are adding a new version to an existing URL proof, any options that were configured on the original proof or previous version are maintained in this version.

1. Click **Create proof** to create a simple proof with no review process.  
   or  
   Continue by configuring an advanced proof:

   * [Create an advanced proof with a Basic workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Create an advanced proof with an Automated workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
