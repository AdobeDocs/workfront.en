---
title: 22.2 Integration enhancements
description: 22.2 Integration enhancements
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
---
# 22.2 Integration enhancements

This page describes all Integration enhancements made with the 22.2 release to the Preview environment. These enhancements will be made available in the Production environment 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

the week of April 4, 2022.

For a list of all changes available with the 22.2 release, see [22.2 Release overview](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront with Anaplan integration now available

To give you better flexibility and insight into the financial aspects of your Workfront projects, Workfront can now integrate with your Anaplan account. By linking Workfront objects to Anaplan objects, you can update information between the two accounts automatically, ensuring that the information in both is up-to-date and identical. You can also trigger automated processes in Anaplan based on actions in Workfront (or vice versa).

For example, you can create a campaign in Anaplan, then create a Workfront project or program linked to the campaign. Any costs tracked in Workfront can then be uploaded back to Anaplan to review campaign performance.

Other workflows that you may consider using the Workfront to Anaplan integration for include:

* Creating Anaplan budget requests from new Workfront projects
* Creating Workfront projects from new Anaplan List Items
* Initiating Anaplan supplier requests from Workfront projects

For more information, see [Adobe Workfront with Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront for Experience Manager enhanced connector updates

Workfront for Experience Manager enhanced connector now includes the following updates:

* You can now create linked folders between Adobe Workfront and Adobe Experience Manager Assets as a Cloud Service even if there are multiple project linked folder configurations.
* Added support for event subscription pagination
* Added support for AEM 6.4.x
* Added support for proxy environments
* Several bug fixes based on partner and customer feedback

For more information, see [Workfront for Experience Manager enhanced connector overview](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>Deployment and configuration of this connector requires a certified partner. See [Install Workfront for Experience Manager enhanced connector](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) for more information.

## Adobe Creative Cloud integrations now use OAuth2

For greater security, and to make a more consistent experience across integrations, we've updated the Adobe Creative Cloud integrations to use OAuth2 authentication, an industry-standard way to authenticate users. Now, when your users log in, they can see the specific actions and areas that the integrations have access to, and allow access. After this, they do not need to log in as frequently.

For more information, see [Use the Workfront Extension for Illustrator and InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## See details of the Client Secret for custom OAuth2 or JWT integrations

To provide transparency into the use of your custom OAuth2 and JWT integrations, we've made it possible for you to see details of the Client Secrets your integrations use. Now, you can see the dates that the Client Secret was created and last used. You can also add and view your own notes about the Client Secret.

Previously, these details were unavailable.

For more information on Client Secrets in OAuth2 or JWT custom integrations, see [Create OAuth2 applications for Workfront integrations](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## See type of authentication in list of custom OAuth2 applications

Now, when you view the list of custom OAuth2 applications in your organization, you can see whether each application uses User authentication or Server authentication.

Previously, you could see this information only by going into the edit options on each application.

For more information, see [Create OAuth2 applications for Workfront integrations](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Set expiration for refresh tokens in your custom OAuth2 integrations

To better control access and security for your custom OAuth2 integrations, you can now customize the lifespan of refresh tokens. After a user's refresh token expires, they will need to log in to the integration again.

For more information, see [Create OAuth2 applications for Workfront integrations](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Use public and private keys in your custom OAuth2 integrations for server-to-server apps

You can now set up server-to-server OAuth2 applications in your custom integrations. By setting up public and private keys, you can allow Workfront to communicate with another application without using login credentials.

Previously, all authentication in your custom OAuth2 applications used the user's login credentials.

For more information, see [Create OAuth2 applications for Workfront integrations](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Google Google Workspace integration now uses OAuth2

For greater security, and to make a more consistent experience across integrations, we've updated the Google Google Workspace integration to use OAuth2 authentication, an industry-standard way to authenticate users. Now, when your users log in, they can see the specific actions and areas that the integrations have access to, and allow access. After this, they do not need to log in as frequently.

For more information, see [Log in and out of Adobe Workfront for Google Workspace](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
