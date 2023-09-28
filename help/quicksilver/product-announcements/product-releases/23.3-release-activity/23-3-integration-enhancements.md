---
title: 23.3 Integration enhancements
description: 23.3 Integration enhancements
author: Lisa
feature: Product Announcements
exl-id: 95c42acd-f7c4-432d-b2da-1ff27b5a6098
---
# 23.3 Integration enhancements

This page describes all integration enhancements made with the 23.3 release. These enhancements were made available in the Production environment with the 23.3 release on July 20 and 21, 2023.

For a list of all changes available at this point in the 23.3 release cycle, see [23.3 Release overview](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## New G Suite integration now available

A new G Suite integration is now available in the Google Marketplace. The new integration authenticates using OAuth2, and replaces the previous integration.

The previous G Suite integration is now deprecated, and will be automatically uninstalled.

For instructions on how to install the new integration, see [Install [!DNL Adobe Workfront for G Suite]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

For more information on Workfront for G Suite, see [Workfront for G Suite](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Adobe Creative Cloud integrations now support multiple assigned users

The Adobe Creative Cloud integration now supports the ability to choose between "Done with my part" and "Complete" (or "Resolved") when a task or issue has multiple assigned users.

Previously, the integration allowed users to mark a task as done, without specifying "Done with my part" Or "Complete"/"Resolved."

To take advantage of this functionality, download and install the newest Workfront for Creative Cloud plugins.

For more information on the functionality, see [Mark work items complete using the Adobe Workfront plugin](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

For information on installing the Workfront for Creative Cloud plugins, see [Install the Adobe Workfront plugin for Creative Cloud Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## View and manage Workfront notifications from the Workfront for Creative Cloud plugins

To make it easier for you to receive the notifications you need, we've made it possible to view and manage Workfront notifications without leaving the Adobe Creative Cloud. Now, you can view notifications, as well as access the work items and comments related to those notifications, directly from the Workfront plugin window within the Creative Cloud application.

Previously, notifications were only available within Workfront and through email.

To take advantage of this functionality, download and install the newest Workfront for Creative Cloud plugins.

For more information, see [View and Manage [!DNL Adobe Workfront] notifications from Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

For information on installing the Workfront for Creative Cloud plugins, see [Install the Adobe Workfront plugin for Creative Cloud Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Automatically create linked folders to Adobe Experience Manager Assets when creating a project

With the new Create linked folder workflow for the Adobe Experience Manager integration, you can configure the integration with a path to an Adobe Experience Manager Assets folder. When the integration is added to a project template, any projects created from the template will automatically create a linked subfolder in Experience Manager Assets in the specified folder.

Previously, creating linked folders required action on the part of the user.

This functionality is available only with an Adobe Experience Manager as a Cloud Service integration within Workfront. This is not available in the Adobe Experience Manager enhanced connector.

For more information, see [Use workflows in the Experience Manager Assets integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Map Workfront field values to tags in Experience Manager Assets

Now, you can categorize and quickly find assets based on data from Workfront. You can map this data as part of your metadata configuration in the Workfront for Experience Manager Assets integration.

Previously, mapping Workfront data to Experience Manager Assets tags was unavailable.

For more information on this functionality in Experience Manager Assets as a Cloud Service, see [Configure the [!UICONTROL Experience Manager Assets as a Cloud Service] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
For more information on this functionality in Experience Manager Assets Essentials, see [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Map Workfront fields to custom Experience Manager Assets metadata fields

With the native integration, you can now map both native and built-in Workfront fields to custom metadata schema fields in Experience Manager Assets as a Cloud Service.

For more information on this functionality in Experience Manager Assets as a Cloud Service, see [Configure the [!UICONTROL Experience Manager Assets as a Cloud Service] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
For more information on this functionality in Experience Manager Assets Essentials, see [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Adjust automated proof workflow template settings using Adobe Workfront for Creative Cloud

You can now adjust existing automated workflow template settings directly in the Creative Cloud. Once you choose an existing automated workflow template, you can:

* Disable stages
* Add additional recipients
* Change proof roles
* Adjust the deadline
* Update email notifications 
* And more!

For more information, see [Upload documents and proofs with the [!DNL Adobe Workfront] plugin for [!DNL Creative Cloud] Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

These enhancements are available for the following Creative Cloud apps:

* Photoshop
* XD
* InDesign
* Illustrator
