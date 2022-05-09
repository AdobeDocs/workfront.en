---
filename: login-error-following-field-invalid-emailaddr-cant-be-null
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Login Error: The following fields are invalid: emailAddr cannot be null"
description: When I try to log into Adobe Workfront with my URL (https://customerdomain.my.workfront.com), I am redirected to the SAML login portal and then redirected back to Workfront with the following error - EDIT ME.
---

# Login Error: The following fields are invalid: emailAddr cannot be null

## Problem&nbsp;

When I try to log into Adobe Workfront with my URL (https://customerdomain.my.workfront.com), I am redirected to the SAML login portal and then redirected back to Workfront with the following error:

"Let's try that again. The following fields are invalid:&nbsp;emailAddr cannot be null."

## Cause

This error is caused by an incorrect item in the Map User Attributes&nbsp;area of the SAML 2.0 configuration. For more information about mapping user attributes for SAML 2.0, see [Configure Adobe Workfront with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solution

Update the Attribute Mapping for the email address, and click **Save**.
