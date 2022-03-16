---
filename: wf-user-credentials-vs-saml-user-credentials
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront user credentials vs. SAML user credentials
description: This article focuses specifically on Adobe Workfront and SAML and does not cover other SSO authentication methods such as AD and LDAP.
---

# Adobe Workfront user credentials vs. SAML user credentials

This article focuses specifically on Adobe Workfront and SAML and does not cover other SSO authentication methods such as AD and LDAP.

Workfront credentials are stored in the Workfront database, where the user's email address is their Workfront username. Their Workfront password is also stored. These credentials are replicated in&nbsp;the Preview and Custom Refresh Sandboxes.

SAML credentials are stored in an external SAML system, such as&nbsp;Microsoft's ADFS. They are not stored in Workfront.

During user creation, Workfront detects if SAML 2.0 is configured and if it is, defaults to `Only Allow SAML 2.0 Authentication`&nbsp;for the user.

If during user creation the `Send an invite email to this person` box is checked, Workfront disables `Only Allow SAML 2.0 Authentication` and hides this option. Once `Send an invite email to this person` is checked, this is a non-SAML Workfront user.

After user creation, you have the option to edit the user and check `Only Allow SAML 2.0 Authentication` where the user and password are controlled by the SAML system and the user is no longer using Workfront credentials.

With this option checked, the user is only allowed to log in via SAML. When they go to the Workfront URL, they are automatically redirected to the SAML system asking for their SAML username and password.
