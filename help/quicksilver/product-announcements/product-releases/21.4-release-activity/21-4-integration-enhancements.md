---
title: 21.4 Integration enhancements
description: 21.4 Integration enhancements
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
---
# 21.4 Integration enhancements

This page describes all Integration enhancements made with the 21.4 release to the Preview environment. These enhancements will be made available in the Production environment the week of October 4, 2021.

For a list of all changes available with the 21.4 release, see [21.4 Release overview](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Link documents from Dropbox Business

We've added Dropbox Business as an available document integration. Now, you can access documents you have stored in Dropbox Business directly from inside Workfront.

Dropbox Business allows you to link shared documents and upload documents to shared folders. Dropbox (not Dropbox Business) allows only the owner of the documents to view the document in Workfront.

Your Workfront administrator can enable this integration for your organization.

For more information see [Link documents from external applications](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

For information about how a Workfront administrator can enable this option, see [Configure document integrations](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Updates to Workfront for Slack

The following updates are now visible in the Workfront for Slack integration:

* Workfront for Slack has a new look and feel. 
* Now you receive your Workfront for Slack notifications in real time.

  For example, if you are assigned to a task, you receive that notification as soon as you are assigned. Previously, there could be a delay before the notification appeared in Slack.

This update requires that you reauthorize your Workfront for Slack integration. For information on authorizing the integration, see [Configure Adobe Workfront for Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

For more information on Workfront for Slack notifications, see [Receive Adobe Workfront notifications in Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## More clearly see details of account access when giving consent to Adobe Workfront integrations

The consent screens for Adobe Workfront integrations are now updated. Now, you can see the specific actions and areas that the integrations has access to, so that you can better understand what you are allowing the integration or application to access.

This new consent screen applies to any Adobe Workfront integration that uses OAuth 2.0.

For details on specific integrations, see that integration's documentation.

## API key authentication no longer necessary for integrations

Workfront integrations have recently begun using OAuth2 for greater security and usability. As part of this move, Workfront no longer requires API keys for integrations authentication.
