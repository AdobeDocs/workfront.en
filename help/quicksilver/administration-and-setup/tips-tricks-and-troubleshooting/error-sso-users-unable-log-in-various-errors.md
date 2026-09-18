---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error: SSO Users are Unable to Log In to [!DNL Adobe Workfront] Due to Various Errors"
description: When you receive a login error about federated single sign-on, your username/password combination, or your access to [!DNL Workfront], the problem might be that your [!DNL Workfront] instance uses SSO and you are trying to log in using an incorrect URL.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs
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
# Error: SSO Users are Unable to Log In to [!DNL Adobe Workfront] Due to Various Errors

## Problem

I am unable to log in to [!DNL Workfront] and received one of the following errors:

* Sorry, you can't access [!DNL Workfront] through this login screen. [!DNL Workfront] is set up for Federated Single Sign-On with SAML 2.0. Please contact your [!DNL Workfront] administrator.
* That username/password combination wasn't quite right. Make sure your caps lock isn't on and try again.
* Sorry, you do not have access to [!DNL Workfront]. Please contact your [!DNL Workfront] administrator to get a username and password.

## Solution

Your [!DNL Workfront] instance uses SSO, and you are trying to log in through an incorrect URL. Make sure you're logging in using the correct URL without anything after ".com"

>[!TIP]
>
>Remove any existing bookmarks that have invalid URLs.
