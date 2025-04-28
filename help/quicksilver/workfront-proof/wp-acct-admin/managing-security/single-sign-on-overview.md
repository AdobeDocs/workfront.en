---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Single Sign-On in [!DNL Workfront Proof]
description: Single Sign-On (SSO) allows your users to log into [!DNL Workfront Proof] using your organization's existing username and password.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
---
# Single Sign-On in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

An [!UICONTROL Enterprise] [!DNL Workfront] Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://business.adobe.com/products/workfront/pricing.html).

Single Sign-On (SSO) allows your users to log into [!DNL Workfront Proof] using your organization's existing username and password.

To provide this capability, we use [!DNL Security Assertion Markup Language] (SAML) 2.0, an XML-based protocol that allows you to authorize data and exchange authentication between an identity provider and a web service.

This means that you will authenticate against your own log in system, not against [!DNL Workfront Proof]'s login page.

You must have a custom sub-domains or domains set up on your [!DNL Workfront] Proof account to enable SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* You can read more about fully customized domains in  [Brand the [!DNL Workfront Proof] site - advanced](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

See [Configure Single Sign-On for [!DNL Workfront Proof] users](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) for information about setting up SSO on your account.
