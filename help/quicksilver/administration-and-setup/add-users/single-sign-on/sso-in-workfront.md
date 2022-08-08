---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Overview of single sign-on in Adobe Workfront
description: Workfront provides a centrally managed single sign-on (SSO) configuration that easily integrates Workfront with your existing corporate SSO solution. This configuration is easy to set up and manage, and is available for both OnDemand and OnPremise Enterprise customers.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
---
# Overview of single sign-on in Adobe Workfront

{{important-admin-console-onboard}}


Workfront provides a centrally managed single sign-on (SSO) configuration that easily integrates Workfront with your existing corporate SSO solution. This configuration is easy to set up and manage, and is available for both OnDemand and OnPremise Enterprise customers. 

In order to use the SSO functionality in Workfront, your organization needs to setup an SSO application, such as LDAP or Active Directory. You can then configure Workfront so that it can communicate with your SSO solution.

Federated solutions allow users to log in to all their applications by entering their username and password in a centralized login portal.

![](assets/overview-sso-wf.png)


## Configure your firewall

When using Active Directory and LDAP, Workfront initiates a connection to your server on the specified port.

If you subscribe to Workfront on-demand, and if you have configured your firewall or mail server to allow access only to specific vendors, you need to add certain Workfront IP addresses to your firewall allowlist. For more information, see [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configure Single Sign-On

Workfront integrates with the following SSO solutions:

* LDAP

  For information about integrating Workfront with LDAP, see [Configure Adobe Workfront with LDAP](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-ldap.md).

* Active Directory

  For information about integrating Workfront with Active Directory, see [Configure Adobe Workfront with Active Directory](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-ad.md).

* Other federated solutions that support SAML 1.1

  For information about integrating Workfront with SAML 1.1, see [Configure Adobe Workfront with SAML 1.1](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-1.1.md).

* Other federated solutions that support SAML 2.0

  For information about integrating Workfront with SAML 2.0, see [Configure Adobe Workfront with SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Other federated solutions that support SAML 2.0 using ADFS

  For information about integrating Workfront with SAML 2.0 using ADFS, see [Configure Adobe Workfront with SAML 2.0 using ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
