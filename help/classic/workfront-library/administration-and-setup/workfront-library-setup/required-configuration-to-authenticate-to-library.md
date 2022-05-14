---
filename: required-configuration-to-authenticate-to-library
product-previous: workfront-library
product-area: documents;system-administration;setup
navigation-topic: workfront-library-setup
title: Required configuration to authenticate to Workfront Library
description: In order to access Workfront Library, your users must login using the enhanced Workfront authentication experience. For more information on the enhanced authentication experience, see Enhanced Authentication overview.
---

# Required configuration to authenticate to Workfront Library

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

In order to access Workfront Library, your users must login using the enhanced Workfront authentication experience. For more information on the enhanced authentication experience, see [Enhanced Authentication overview](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

If your organization has not yet migrated to the enhanced experience, you can still set up authentication to Workfront Library if your system meets the following configuration requirements.

## Password management

Each user must have a unique user name, which is the user's Workfront email.

* User names in Workfront Library are not case-sensitive. 
* Each user must have a unique email address for their user name.
* Multiple users cannot use the same email address with different case.

## Single Sign-On configuration

If your organization uses Single Sign-On (SSO) functionality, you must meet the following requirements in order for your users to access Workfront Library using the enhanced authentication experience:

* Your SSO solution must be compliant with SAML 2.0.

  >[!NOTE]
  >
  >Active Directory, LDAP, and SAML 1.0 protocols are not supported.

* Auto-provisioning must be disabled. 
* User accounts must be manually created.

You can map only the following attributes for users:

* First name
* Last name
* Email
* User name
* Address
* Phone number

