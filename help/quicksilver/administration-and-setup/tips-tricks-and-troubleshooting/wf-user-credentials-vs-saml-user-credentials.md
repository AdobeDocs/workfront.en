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
TQID: https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Adobe Workfront user credentials vs. SAML user credentials

This article focuses specifically on [!DNL Adobe Workfront] and SAML and does not cover other SSO authentication methods.

In a database, [!DNL Workfront] stores eawch user's email address as their [!DNL Workfront] username, along with their [!DNL Workfront] password. These credentials are replicated in the Preview and Custom Refresh Sandboxes.

During user creation, if [!DNL Workfront] detects that SAML 2.0 is configured, it defaults to "Only Allow SAML 2.0 Authentication"" for the user. If the "Send an invite email to this person" box is enabled, [!DNL Workfront] disables "Only Allow SAML 2.0 Authentication" and hides this option. Once "Send an invite email to this person" is enabled, the user becomes a non-SAML [!DNL Workfront] user.

After user creation, you can edit the user and enable **[!UICONTROL Only Allow SAML 2.0 Authentication]** so that their user and password are controlled by the SAML system.

With this done, the user is can log in only via SAML. When they go to the [!DNL Workfront] URL, they are automatically redirected to the SAML system and prompted for their SAML username and password.

SAML credentials are stored in an external SAML system, such as Microsoft's ADFS, not in Workfront.
