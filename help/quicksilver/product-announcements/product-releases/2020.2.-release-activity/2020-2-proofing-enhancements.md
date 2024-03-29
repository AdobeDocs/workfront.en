---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Proofing enhancements
description: This page describes all Proofing enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
---
# 2020.2 Proofing enhancements

This page describes all Proofing enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.

For a list of all changes available with the 2020.2 release, see [2020.2 release overview](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## The proofing domain is changing from proofhq.com to workfront.com.

>[!NOTE]
>
>This feature was originally communicated as part of the 2020.1 release, but was removed from the release prior to its release to Production.

If your firewall or mail server is configured to allow access only to specific vendors, you must add the following additional URL to your allowlist to ensure that users in your organization can view proofs within Workfront in both the browser proofing viewer and the desktop proofing viewer:

&#42;.workfront.com

The &#42;proofhq.com URL is also still required.

For more information about updating your allowlist, see [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

This update applies only to proofing within Workfront; it does not apply when using the Workfront Proof stand-alone application.

## Proofing comments made by guests appear in the Updates area

To streamline collaboration on proofs, guest comments appear in the Updates area.

Previously, Proof comments made by guests were available only in the proof.
