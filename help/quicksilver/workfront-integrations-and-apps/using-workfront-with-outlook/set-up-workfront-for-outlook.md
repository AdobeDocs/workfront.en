---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Set up [!DNL Adobe Workfront] for [!DNL Outlook]
description: The [!DNL Adobe Workfront] [!DNL Outlook] add-in lets you perform the key [!DNL Workfront] tasks directly from Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
---
# Set up [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

The [!DNL Adobe Workfront] [!DNL Outlook] add-in lets you perform the following key [!DNL Workfront] tasks directly from Outlook:

* Update an existing project, task, or issue with information from an email. For more information, see [Update an existing object from an [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Create a [!DNL Workfront] request based on an email within [!DNL Outlook]. For more information, see [Create an Adobe Workfront request from an [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Add an email as a task in your [!UICONTROL My Work] area. For more information, see [Add an [!DNL Outlook] email as a task to your work list](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Reply to comments via the [!DNL Workfront] add-in for [!DNL Outlook]. For information about replying to comments from Workfront for [!DNL Outlook], see [Reply to a comment from [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Create tasks and issues from scratch, or create them from existing emails (using drag-and-drop functionality). For more information , see [Add an [!DNL Outlook] email to a project as a task or an issue](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

You must add the [!DNL Workfront] add-in to your [!DNL Outlook] account before you can use [!DNL Workfront for Outlook].

If you are unable to install the [!DNL Workfront] add-in with your [!DNL Outlook] account, contact your [!DNL Workfront] administrator to ensure that [!DNL Outlook] add-ins are enabled for your organization.

For information about how to enable the [!DNL Outlook] integration for your organization, see [Enable [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>New plan: [!UICONTROL Standard]</p> 
   <p>Current plan:[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

Your [!DNL Workfront] administrator must enable [!DNL Outlook for Office] with [!DNL Workfront] before you can use this integration.

## System requirements

The following applications are available: 

* **[!DNL Outlook] on the Web:** The [!DNL Workfront] add-in is available when using [!DNL Outlook] from a web browser either on a desktop or mobile device. This functionality is also available when using the [!DNL Outlook] Web App.
* **[!DNL Outlook] Desktop Application:** The [!DNL Workfront] add-in is available when using the [!DNL Windows] and [!DNL Mac] desktop versions of [!DNL Outlook] included with the [!DNL Office] package.

The [!DNL Workfront] add-in for [!DNL Outlook] is supported in environments that meet the following requirements:

* [Client requirements](#client-requirements-client-requirements)
* [Mail server requirements](#mail-server-requirements-mail-server-requirements)

### Client requirements {#client-requirements}

Workfront supports the following versions of [!DNL Outlook]: 

* [!DNL Outlook 2013] or later on [!DNL Windows]
*[!DNL  Outlook 2016] or later on [!DNL Windows]
* [!DNL Outlook] on [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] on [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] on the web

You must be connected to an [!DNL Exchange Server] or [!DNL Office 365] using a direct connection.

When configuring the client, the user must select one of the following account types:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;If the client is configured to connect with POP3 or IMAP, the [!DNL Workfront] add-in does not load.

### Mail server requirements {#mail-server-requirements}

The mail server requirements are met by default when you connect to [!DNL Office 365] or [!DNL Outlook.com]. However, if you are connected to an on-premise installation of [!DNL Exchange Server], the following requirements apply:

* Workfront supports all [!DNL Exchange On-Premise] servers
* [!DNL Exchange Web Services] (EWS) must be enabled and must be exposed to the internet. 
* The server must have a valid authentication certificate in order for the server to issue valid identity tokens. New installations of [!DNL Exchange Server] include a default authentication certificate.

   <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* In order to access the [!DNL Workfront] add-in from the [[!DNL Office] Store](https://store.office.com/), your client access servers must be able to communicate with  [https://store.office.com](https://store.office.com/).

For more detailed information about supported environments, see the [[!DNL Microsoft Office 365] home page](https://products.office.com/en-us/office-365-home).

## Install the add-in

You can get the Workfront add-in for Outlook from the [Microsoft store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] for [!DNL Outlook 365] {#workfront-for-outlook-365}

1. In [!DNL Outlook 365], click the **[!UICONTROL Browse Add-ins]** icon ![](assets/outlook-add-in-26x26.png)at the top of the Office 365 interface, then click **[!UICONTROL Manage add-ins]**.

1. In the **[!UICONTROL Search add-ins]** box, search for **[!DNL Workfront]** then press [!UICONTROL Enter]. 

1. Click **[!UICONTROL Add]**.

### [!DNL Workfront] for [!DNL Outlook] on the Web {#workfront-for-outlook-on-the-web}

1. Open [!DNL Microsoft Outlook] in a web browser.
1. Click the **[!UICONTROL Browse] add-ins** icon ![](assets/outlook-add-in-web-version-20x20.png).

   To locate the icon, see [Using add-ins in [!DNL Outlook] on the web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) in the Microsoft documentation.

1. Search for **[!DNL Workfront]** in the **[!UICONTROL Search add-ins]** field, then press **[!UICONTROL Enter]**.

1. When it appears on the list, click **Add**.

### [!DNL Workfront for Outlook] on [!UICONTROL Windows] or [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Click **[!UICONTROL Home]** > **[!UICONTROL Store]** on the ribbon.

1. Search for **[!DNL Workfront]** in the **[!UICONTROL Search]** field, then press **[!UICONTROL Enter]**.

1. Click the toggle to enable the **[!UICONTROL [!DNL Workfront] add-in]**.

## Log in to [!DNL Workfront] from [!DNL Outlook]

1. In [!DNL Outlook], select an email message, then click the **[!DNL Workfront]** icon in the email header.
1. Follow the prompts to log in to [!DNL Workfront] using Enhanced Authentication, OAuth 2.0, or your Security Assertion Markup Language (SAML) URL.

   Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* When you are prompted to enter the domain of your [!DNL Workfront] account, type it using this format: *yourCompany'sDomain.my.workfront.com*. Your company's domain is usually the name of your company.
   >* Enhanced Authentication is not available until a [!DNL Workfront] administrator enables it for this integration.

