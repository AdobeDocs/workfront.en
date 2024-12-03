---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler settings can cause reduced performance
description: After user creation, you can edit the user and enable "Only Allow SAML 2.0 Authentication" so that their user and password are controlled by the SAML system. With this option enabled, the user is only allowed to log in via SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
---
# Workfront: ZScaler settings can cause reduced performance

>[!NOTE]
>
>This is an issue with ZScaler, and will not be fixed by Workfront.

ZScaler's web service uses `http/1.1` by default, which can cause reduced performance in Workfront.

To check and resolve this issue, configure your ZScaler software to use `http/2`. This cannot be configured in Workfront.

You can find information about `http/2` in the ZScaler documentation.
