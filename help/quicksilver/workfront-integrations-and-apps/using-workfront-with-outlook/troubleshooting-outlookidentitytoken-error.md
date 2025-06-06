---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Troubleshooting: outlookIdentityToken error when using Workfront for Outlook'
description: If you get an outlookIdentityToken error when using Workfront for Outlook, you must enable Microsoft 365 legacy tokens for your organization.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
---
# Troubleshooting: outlookIdentityToken error when using Workfront for Outlook

>[!IMPORTANT]
>
>[Microsoft is in the process of disabling support for legacy Exchange online tokens](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), which are currently used by the Workfront Outlook add-in for authentication. This change by Microsoft has already started affecting customers and will continue to roll out in phases through October 2025.
>
>* **After Microsoft fully disables these tokens, the Workfront for Microsoft Outlook integration will no longer function.** 
>
>As part of this change, Microsoft has made the decision to change the way tokens are re-enabled. After **June 30, 2025**, admins will no longer be able to re-enable tokens themselves—only Microsoft Support can grant exceptions. **On October 1, 2025, legacy tokens will be turned off for all tenants. Exceptions will not be granted.**  


When using Workfront for Outlook, you may see the following error:

```
Unexpected error
Unable to get the outlookIdentityToken
```

To resolve this error, you must enable Microsoft 365 legacy tokens for for your organization. Because this must be done in Microsoft 365, Workfront cannot enable these tokens for your organization.

For instructions on enabling Microsoft 365 legacy tokens, see [Turn legacy Exchange Online tokens on or off](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in the Microsoft documentation.

For more information on legacy tokens, see [Can I turn Exchange Online legacy tokens back on?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in the Microsoft documentation.
