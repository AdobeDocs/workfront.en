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
---
# Login Error: The following fields are invalid: emailAddr cannot be null

## Problem

When I try to log into [!DNL Adobe Workfront] with my URL (https://customerdomain.my.workfront.com), I am redirected to the SAML login portal and then redirected back to [!DNL Workfront] with the following error:

"Let's try that again. The following fields are invalid: emailAddr cannot be null."

## Cause

This error is caused by an incorrect item in the Map User Attributes area of the SAML 2.0 configuration. For more information about mapping user attributes for SAML 2.0, see [Configure Adobe Workfront with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solution

Update the Attribute Mapping for the email address, and click **[!UICONTROL Save]**.
