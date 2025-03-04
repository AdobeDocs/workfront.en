---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: "Troubleshooting: outlookIdentityToken error when using Workfront for Outlook"
description: If you get an outlookIdentityToken error when using Workfront for Outlook, you must enable Microsoft 365 legacy tokens for your organization.
author: Becky
feature: Workfront Integrations and Apps
---
# Troubleshooting: outlookIdentityToken error when using Workfront for Outlook

When using Workfront for Outlook, you may see the following error:

```
Unexpected error
Unable to get the outlookIdentityToken
```

To resolve this error, you must enable Microsoft 365 legacy tokens for for your organization. Because this must be done in Microsoft 365, Workfront cannot enable these tokens for your organization.

For instructions on enabling Microsoft 365 legacy tokens, see [Turn legacy Exchange Online tokens on or off](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in the Microsoft documentation.

For more information on legacy tokens, see [Can I turn Exchange Online legacy tokens back on?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in the Microsoft documentation.
