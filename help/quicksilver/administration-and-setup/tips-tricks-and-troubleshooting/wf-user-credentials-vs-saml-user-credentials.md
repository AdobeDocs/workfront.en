---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront User Credentials vs. SAML User Credentials
description: After user creation, you can edit the user and enable "Only Allow SAML 2.0 Authentication" so that their user and password are controlled by the SAML system. With this option enabled, the user is only allowed to log in via SAML.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
---
# Adobe Workfront user credentials vs. SAML user credentials

This article focuses specifically on [!DNL Adobe Workfront] and SAML and does not cover other SSO authentication methods.

In a database, [!DNL Workfront] stores eawch user's email address as their [!DNL Workfront] username, along with their [!DNL Workfront] password. These credentials are replicated in the Preview and Custom Refresh Sandboxes.

During user creation, if [!DNL Workfront] detects that SAML 2.0 is configured, it defaults to "Only Allow SAML 2.0 Authentication"" for the user. If the "Send an invite email to this person" box is enabled, [!DNL Workfront] disables "Only Allow SAML 2.0 Authentication" and hides this option. Once "Send an invite email to this person" is enabled, the user becomes a non-SAML [!DNL Workfront] user.

After user creation, you can edit the user and enable **[!UICONTROL Only Allow SAML 2.0 Authentication]** so that their user and password are controlled by the SAML system.

With this done, the user is can log in only via SAML. When they go to the [!DNL Workfront] URL, they are automatically redirected to the SAML system and prompted for their SAML username and password.

SAML credentials are stored in an external SAML system, such as Microsoft's ADFS, not in Workfront.
