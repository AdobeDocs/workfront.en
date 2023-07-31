---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Troubleshoot the Adobe Experience Manager integration
description: Connect your work with your content in Experience Manager Assets Essentials - EDIT ME.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
---
# Troubleshoot the Adobe Experience Manager Integration

## Problem: Assets are not saved to Adobe Experience Manager

When a user selects an asset or folder to export to Experience Manager Assets and clicks Select, the selector window closes but the assets are not saved to Experience Manager Assets. There is no indication in Workfront that the assets did not saved to Experience Manager Assets.

### Cause

This may occur because of the allowlist in Adobe Cloud Manager. If the Adobe Cloud Manager allowlist for an organization is empty, then IP addresses are not limited, and Workfront can access the organization's folders and assets in Adobe Experience Manager. However, if even a single IP address is added to the Cloud Manager allowlist, then the allowlist assumes that any IP address not on the list is not allowed. Therefore, if the Cloud Manager allowlist includes any IP addresses, the Workfront IP addresses must also be added to the allowlist to enable Workfront to send assets to Experience Manager Assets.

### Solution:

Add the Workfront IP addresses to the Adobe Cloud Manager allowlist.

* For instructions on adding IP addresses to your Adobe Cloud Manager, see [Introduction to IP Allow Lists](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) in the Adobe Experience Manager documentation.
* For a list of Workfront IP addresses to add to the allowlist, see [Configure your firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

