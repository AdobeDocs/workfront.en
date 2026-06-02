---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Other enhancements
description: This page describes all enhancements made to general areas of Workfront with the 2020.1 release. These enhancements are currently available in the Preview environment and will be made available in the Production environment in late March or early April, 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
TQID: https://experienceleague.adobe.com/I5djuVv0ixHspF6afQaa5-jTkl0uXl26VlKf8BXqhO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
subfeature_v2:
  - id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
    internal-label: Adobe Workfront for Jira
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# 2020.1 Other enhancements

This page describes all enhancements made to general areas of Workfront with the 2020.1 release. These enhancements are currently available in the Preview environment and will be made available in the Production environment in late March or early April, 2020.

For a list of all changes available with the 2020.1 release, see [2020.1 release overview](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Change required for adding proofs to the allowlist

>[!NOTE]
>
>This feature was removed from the 2020.1 release. It will be made available at a later time.

The proofing domain is changing from&nbsp;proofhq.com to workfront.com.

If your firewall or mail server is configured to allow access only to specific vendors, you must add the following additional URL&nbsp;to your allowlist to ensure that users in your organization can view proofs within Workfront in both the browser proofing viewer and the desktop proofing viewer:

&#42;.workfront.com

The &#42;proofhq.com URL is also still required.

For more information about updating your allowlist, see [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>This update applies only to proofing within Workfront; it does not apply when using the Workfront Proof stand-alone application.

## Workfront cookie behavior updated to maintain compatibility with Chrome

To maintain compatibility with an upcoming Google Chrome update (Chrome v80), we've updated the Workfront platform to ensure that cookies are appropriately sent with requests.

This Chrome update changes the default value of the SameSite cookie attribute. If you want to test how your Workfront instance will behave after the Google Chrome update, adjust the flags in Chrome and enable the following options:

* "SameSite by default cookies" 
* "Cookies without SameSite must be secure"

## Workfront comments sync to Jira

The Workfront for Jira integration now syncs your Workfront comments to Jira's native comment stream.

Previously, you could sync comments from Jira to Workfront, but not from Workfront to Jira.

For more information, see [Configure Adobe Workfront for Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## The Flash Portfolio Optimizer has been removed

We have removed the ability to switch between the new and the legacy (based on Flash) Portfolio Optimizer from the Workfront Classic environment for all customers. The Legacy Portfolio Optimizer is a deprecated feature and the new tools provide the same functionality today.

For information about the portfolio optimizer, see https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

For information about deprecating Flash-based tools in Workfront see [Replacement of Flash-based tools in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
