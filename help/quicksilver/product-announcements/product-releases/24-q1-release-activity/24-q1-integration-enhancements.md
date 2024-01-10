---
title: First Quarter 2024 Integration enhancements
description: First Quarter 2024 Integration enhancements
author: Becky
feature: Product Announcements
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
---
# First Quarter 2024 Integration enhancements

This page describes all integration enhancements made with the First Quarter 2024 release to the Preview environment. These enhancements will be made available in the Production environment with the First Quarter 2024 release.

For a list of all changes available at this point in the First Quarter 2024 release cycle, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Mapping metadata in Experience Manager Assets Essentials now uses `xcm:keywords` instead of `dc:subject`

We've updated the Experience Manager Assets Essentials integration to match the experience in the Experience Manager Assets as a Cloud Service integration. Now, when mapping multiple single-line text fields to a single field in Experience Manager Assets, both services use the `xcm:keywords` field.

Previously, these fields would be mapped to the `dc:subject` field in Experience Manager Assets Essentials. The Experience Manager Assets as a Cloud Service functionality is unchanged.

Any Experience Manager Assets Essentials metadata currently mapped to `dc:subject` must be remapped to `xcm:keywords`.

For information on mapping metadata to Experience Manager Assets Essentials, see [AEM Keyword](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Typeahead fields now available in Adobe Experience Manager Integration

To make it easier to link fields between Workfront and Adobe Experience Manager, we've added support for typeahead fields in the metadata mapping. Now, you can map typeahead fields to corresponding fields in Adobe Experience Manager.

If a user selects a different value for a field in Workfront, this change is immediately reflected in Adobe Experience Manager. In addition, if a field value option changes (such as a team changing its name to a new name), this change is also reflected in Adobe Experience Manager.

For information and instructions on metadata mapping in the Adobe Experience Manager integration, see [Set up metadata](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Automatically publish assets in Adobe Experience Manager 

We've added another workflow to the Adobe Experience Manager integration. Now, you can set your assets to automatically publish when sent to Adobe Experience Manager. The integration can be configured to publish to the Adobe Experience Manager publish service, or to an Adobe Experience Manager brand portal.

The Automatic Publish workflow can be enabled and configured in the Adobe Experience Manager integration. When enabled, the workflow can be edited on the project template or project level.

For more information, see [Publishing assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) in [Use workflows in the Experience Manager Assets integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
