---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Install [!DNL Adobe Workfront] for [!DNL Jira]
description: You can use [!DNL Adobe Workfront] for [!DNL Jira] to integrate your [!DNL Jira] and [!DNL Workfront] systems.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
---
# Install [!DNL Adobe Workfront for Jira]

You can use [!DNL Adobe Workfront for Jira] to integrate your [!DNL Jira] and [!DNL Workfront] systems.

After installing the add-on, you can define workflows that create [!DNL Jira] issues automatically when [!DNL Workfront] work items are created. The items in both applications become linked, and some of their information can be automatically updated in both systems. 

All users in [!DNL Workfront] and [!DNL Jira] can benefit from this integration. They only need a license for the system in which they work the most, and not for both systems. 

This add-on is available for the [!UICONTROL Server] and [!UICONTROL OnDemand] (or [!UICONTROL Cloud]) versions of [!DNL Jira] Software. This add-on is not available for the [!DNL Data Center] version of [!DNL Jira] Software.

For a list of [!DNL Jira] versions that [!DNL Workfront for Jira] currently supports, see [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) at the Atlassian Marketplace.

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> 
   <p>New: Any</p>
   <p>Current: [!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licenses overview</td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in [!DNL Jira] and [!DNL Workfront] to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>You must be a [!DNL Workfront] administrator.</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Install [!DNL Workfront] for [!DNL Jira]

Installing [!DNL Workfront] for [!DNL Jira] OnDemand is identical to installing it on a [!DNL Jira] Server instance.

You must be a [!DNL Jira] administrator to install the [!DNL Workfront] add-on.

If you are not a [!DNL Jira] administrator, you can browse for the [!DNL Workfront] add-on and request it to be installed. Your request is sent to the [!DNL Jira] administrator for approval and installation. 

For more information about requesting an add-on to be installed on your [!DNL Jira] application, see [Managing user requests for add-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

To install [!DNL Workfront for Jira]:

1. Log in to [!DNL Jira] as a [!DNL Jira] administrator.
1. Find the **[!DNL Workfront for Jira]** add-on in the [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Click **[!UICONTROL Get it now]** to install it.

   After the installation completes, you can log in to [!DNL Workfront] from [!DNL Jira] and configure your integration.

   For more information, see [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considerations for a [!DNL Jira Server] installation

>[!NOTE]
>
>These requirements do not apply to the [!UICONTROL OnDemand] ([!UICONTROL Cloud]) version of [!DNL Jira] Software.

Although installing the [!DNL Workfront] add-on in the two [!DNL Jira] environments is similar, you must consider the following when working with a [!DNL Jira Server] installation:

* When configuring the add-on in [!DNL Jira], the address specified in the **[!DNL JIRA Base URL]** field may not be the same URL you use to access [!DNL Jira] on your private server. The **[!DNL JIRA Base URL]** must be a publicly-accessible address connected to your private server using NAT or reverse proxy protocols, so [!DNL Workfront] can access it to make requests to your server.  

* You must use SSL encryption to secure the communication between [!DNL Jira] and [!DNL Workfront]. When you enable SSL, you must have a full SSL certificate stack from a certificate authority. We do not support self-signed certificates. 
* You must ensure that the [!DNL jira.workfront.com] domain is accessible from your corporate servers. It serves as a middleware environment between [!DNL Workfront] and [!DNL Jira] and is required for the add-on to operate.

   You must also add the following static IP addresses to the allowlist on your firewall for outbound and inbound connections.

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   For more information about configuring your firewall for optimal functionality with [!DNL Workfront], see [Configuring Your Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
