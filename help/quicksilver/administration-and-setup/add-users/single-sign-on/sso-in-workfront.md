---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Overview of Single Sign-On in Adobe Workfront
description: Workfront provides a centrally managed single sign-on (SSO) configuration that easily integrates Workfront with your existing corporate SSO solution. This configuration is easy to set up and manage, and is available for both OnDemand and OnPremise Enterprise customers.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
---
# Overview of single sign-on in Adobe Workfront

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront provides a centrally managed single sign-on (SSO) configuration that integrates Workfront with your existing corporate SSO solution. This configuration is available for both OnDemand and OnPremise Enterprise customers. 

To use the SSO functionality in Workfront, your organization needs to set up an SSO application. You can then configure Workfront so that it can communicate with your SSO solution.

Federated solutions allow users to log in to all their applications by entering their username and password in a centralized login portal.

![](assets/overview-sso-wf-fed-only.png)


## Configure your firewall

When using an SSO solution, Workfront initiates a connection to your server on the specified port.

If your firewall or mail server is configured to allow access only to specific vendors, you must add certain Workfront IP addresses to your firewall allowlist. For more information, see [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configure Single Sign-On

Workfront integrates with the following SSO solutions:

* Federated solutions that support SAML 2.0

  For information about integrating Workfront with SAML 2.0, see [Configure Adobe Workfront with SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Federated solutions that support SAML 2.0 using ADFS

  For information about integrating Workfront with SAML 2.0 using ADFS, see [Configure Adobe Workfront with SAML 2.0 using ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
