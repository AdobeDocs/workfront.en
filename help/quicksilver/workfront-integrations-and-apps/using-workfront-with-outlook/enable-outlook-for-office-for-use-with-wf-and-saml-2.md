---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Enable Outlook for Office for use with [!DNL Adobe Workfront] and SAML 2.0
description: If your [!DNL Adobe Workfront] system is integrated with SAML 2.0, you must enable SAML 2.0 authentication for Office add-ins in order for users to be able to authenticate using their SAML 2.0 credentials.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 72ffceb3-50f0-486e-92b5-0bea4c9a99c8
---
# Enable [!DNL Outlook for Office] for use with [!DNL Adobe Workfront] and SAML 2.0

>[!IMPORTANT]
>
>[Microsoft is in the process of disabling support for legacy Exchange online tokens](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), which are currently used by the Workfront Outlook add-in for authentication. This change by Microsoft has already started affecting customers and will continue to roll out in phases through October 2025.
>
>* **After Microsoft fully disables these tokens, the Workfront for Microsoft Outlook integration will no longer function.** 
>
>As part of this change, Microsoft has made the decision to change the way tokens are re-enabled. After **June 30, 2025**, admins will no longer be able to re-enable tokens themselves—only Microsoft Support can grant exceptions. **On October 1, 2025, legacy tokens will be turned off for all tenants. Exceptions will not be granted.**  

If your [!DNL Adobe Workfront] system is integrated with SAML 2.0, you must enable SAML 2.0 authentication for [!DNL Office] add-ins in order for users to be able to authenticate using their SAML 2.0 credentials. 

If you experience issues when logging in to [!DNL Workfront] with SAML, contact your [!DNL Workfront] administrator to ensure that SAML is configured correctly.

For information about how to enable Office add-ins to authenticate using a SAML 2.0 solution, see the section in the [Configure Adobe Workfront with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md) article.
