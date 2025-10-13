---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Proof a linked asset with the enhanced connector
description: After you've linked an asset from Experience Manager Assets, you can create a proof and assign users to review and add comments to the asset.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
---
# Proof a linked asset with the enhanced connector

After you've linked an asset from Experience Manager Assets, you can create a proof and assign users to review and add comments to the asset. Proofs created from linked assets count towards your proof storage quota.

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
   <p>Work or higher</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Additional products</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access or higher on a Document</p> </td> 
  </tr> 
 </tbody> 
</table>


For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you begin, you must

* Install the Workfront for Experience Manager enhanced connector

## Create a proof

You can create static, video, or interactive proofs.

To create a proof:

1. Go to the project, task, or issue where you want the proof, then click the **Documents** section.
1. Hover over the document, then click the **Create Proof** link that appears below the document name.

   >[!NOTE]
   >
   >If you have **Automatically generate proofs when uploading documents** enabled in your user profile, the system automatically creates a simple proof.

1. Choose one of the following:  

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Simple Proof</td> 
      <td>This option creates a proof with no workflow attached and applies the default proof settings. You can update the default proofsettings or add a workflow after you've created the proof. For more information on proof settings, see <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Edit proof settings</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Advanced Proof</td> 
      <td> <p>This option allows you to configure a Basic or Advanced workflow and modify proof settings for the proof you create. For more information, see </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Create an advanced proof with a Basic workflow</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Create an advanced proof with an Automated workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Manage an existing proof

Once you've created a proof, you can do things like

* View current stage activity
* Update reviewers and deadlines
* Edit the workflow

For more information about how to manage an existing proof, see [Manage proofs within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Review a proof

Assigned reviewers can do things like

* View the asset and make comments
* Add actions to comments
* Compare versions
* Approve or reject the proof

For more information about what you can do with the proofing tool, see [Review proofs within Adobe Workfront](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
