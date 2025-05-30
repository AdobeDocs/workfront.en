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

>[!NOTE]
>
>Microsoft is in the process of disabling support for legacy Exchange Online tokens, which are used by this integration. A new Microsoft Office 365 integration will be available in September 2025, which will not use legacy Exchange Online tokens. 
>
>In the meantime, we highly recommend renewing your legacy Exchange Online token:
>
>* Before June 30, 2025: Your Microsoft administrator can renew your legacy Exchange Online token.
>* After June 30, 2025, you must contact Microsoft Support to renew your legacy Exchange Online token. 


When using Workfront for Outlook, you may see the following error:

```
Unexpected error
Unable to get the outlookIdentityToken
```

To resolve this error, you must enable Microsoft 365 legacy tokens for for your organization. Because this must be done in Microsoft 365, Workfront cannot enable these tokens for your organization.

For instructions on enabling Microsoft 365 legacy tokens, see [Turn legacy Exchange Online tokens on or off](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in the Microsoft documentation.

For more information on legacy tokens, see [Can I turn Exchange Online legacy tokens back on?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in the Microsoft documentation.
