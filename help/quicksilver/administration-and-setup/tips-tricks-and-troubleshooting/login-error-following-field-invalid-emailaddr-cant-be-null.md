---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Login Error: The following fields are invalid: emailAddr cannot be null"
description: When I try to log into [!DNL Adobe Workfront] the URL for my domain, I am redirected to the SAML login portal and then redirected back to [!DNL Workfront] with an error saying that the emailAddr field cannot be null.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
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
# Login Error: The following fields are invalid: emailAddr cannot be null

## Problem

When I try to log into [!DNL Adobe Workfront] with my URL (https://customerdomain.my.workfront.com), I am redirected to the SAML login portal and then redirected back to [!DNL Workfront] with the following error:

"Let's try that again. The following fields are invalid: emailAddr cannot be null."

## Cause

This error is caused by an incorrect item in the Map User Attributes area of the SAML 2.0 configuration. For more information about mapping user attributes for SAML 2.0, see [Configure Adobe Workfront with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solution

Update the Attribute Mapping for the email address, and click **[!UICONTROL Save]**.
