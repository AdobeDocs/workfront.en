---
filename: error-sso-users-unable-log-in-various-errors
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Error: SSO Users are Unable to Log In to Adobe Workfront Due to Various Errors
description: I am unable to log in to Workfront and received one of the following errors:
---

# Error: SSO Users are Unable to Log In to Adobe Workfront Due to Various Errors

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Problem

I am unable to log in to Workfront and received one of the following errors:

* Sorry, you can't access Workfront through this login screen. Workfront is set up for Federated Single Sign-On with SAML 2.0. Please contact your Workfront administrator.
* That username/password combination wasn't quite right. Make sure your caps lock isn't on and try again.
* Sorry, you do not have access to Workfront. Please contact your Workfront administrator to get a username and password.

## Solution

Your Workfront instance uses SSO, and you are trying to log in through an incorrect URL. Make sure you're logging in using the correct URL without anything after ".com"

>[!TIP]
>
>Remove any existing bookmarks that have invalid URLs.

