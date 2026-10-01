---
title: 21.3 Proofing enhancements
description: 21.3 Proofing enhancements
author: Luke
draft: Probably
feature: Product Announcements, Workfront Proof, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: cad1ebc1-0477-4a05-a8c0-6cdfacbdc976
TQID: 'https://experienceleague.adobe.com/PIgksR1T1k2q9qOd95u2-RZq7kNfEMDuCSy3Gky05cw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# 21.3 Proofing enhancements

This page describes all Proofing enhancements made with the 21.3 release to the Preview environment. These enhancements were made available in the Production environment the week of July 21, 2021.

For a list of all changes available with the 21.3 release, see [21.3 Release overview](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Remove ability to create a new document or proof version in a linked folder

We removed the ability to create a new version of a document or proof within a linked folder. You can still create a new version of a linked document or proof if they are outside of a linked folder.

Previously, this option still displayed for documents and proofs in linked folders, but users were unable to create a new version of a document.

## Users added to a proof automatically granted View access on a document

>[!NOTE]
>
>This feature was released to the Preview environment on May 20, 2021. It was released to the Production environment on June 17, 2021.

Users with Reviewer or Read-only selected as their proof role are automatically granted View access on the document if they had none previously.

Previously, users with the proof roles mentioned above had to request access to documents when they were added to the proof.
