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
