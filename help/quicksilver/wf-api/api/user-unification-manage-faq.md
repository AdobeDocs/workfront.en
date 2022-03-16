---
filename: user-unification-manage-faq
content-type: api;faq
navigation-topic: api-navigation-topic
title: Adobe Workfront User Unification Management Initiative FAQ (Draft)
description: In order to make your work life easier, Adobe Workfront is streamlining the way you manage users and passwords by introducing our Unified User Management (UUM) initiative. UUM is designed to unify your users across all Workfront products and services by providing a consistent sign-in experience.
---

# Adobe Workfront User Unification Management Initiative FAQ (Draft)

In order to make your work life easier, Adobe Workfront is streamlining the way you manage users and passwords by introducing our Unified User Management (UUM) initiative. UUM is designed to unify your users across all Workfront products and services by providing a consistent sign-in experience.

## Benefits of UUM

Workfront UUM provides the following benefits:

* Usernames are no longer required to be unique across all instances of Workfront.
* Users experience a consistent sign-in across the following Workfront products and services:

  * Workfront
  * ProofHQ
  * Workfront Customer Support
  * Workfront Community
  * Workfront Training (Ascent)
  * Workfront Idea Exchange
  * Workfront Mobile App
  * Workfront Proof Mobile App

* Users can access new Workfront products without having to manage a new username and password.
* Your organization can more effectively support users that do not have credentials from your single sign-on (SSO) provider.
* If your organization utilizes multiple SAML 2.0 Identity Providers (IDPs), you can support all your IDPs with Workfront UUM.

## Frequently Asked Questions

### What if I use the same email address for multiple Workfront instances?

Typically, the email address associated with a user’s Workfront account is the user’s username. Workfront currently requires a unique email address for each instance of Workfront. Many users work around this requirement by utilizing a combination of uppercase and lowercase characters in their email address to create a unique username for each of their Workfront instances.

However, with the migration to Workfront UUM, users will need only one unique email address in order to access all Workfront products and services. Consequently, Workfront will no longer distinguish between uppercase and lowercase characters in email addresses.

If your email address is unique and uses a combination of uppercase and lowercase characters, you will still be able to log into Workfront.

### What if I have duplicated users by using the same email address, but with different combinations of letter case?

If you have multiple users in your Workfront instance that use the same email address except for having varying combinations of uppercase and lowercase characters, you will need to create a unique email address for each user.

The following are possible strategies for duplicating users within the same instance of Workfront:

* + email aliasing: Many email services allow you to add a plus sign (+) to an email address in order to reuse it and make it unique within a Workfront instance. For example, instead of the username&nbsp;*user*@workfront.com, you would use *user+customtext**@workfront.com.*

* . email aliasing: Many email services allow you to add a period (.) to an email address in order to reuse it and make it unique within a Workfront instance. For example, instead of *myuser*@workfront.com, you would use *my.user*@workfront.com

* New email account: Create a new email account with a valid email address and use it for the username.

Check with your email administrator to determine the best option for your organization. You can also test the validity of a strategy by sending yourself a sample email using the respective option. If you successfully receive the email, you know it is a viable solution.

>[!NOTE]
>
>All email addresses for your active and deactivated Workfront users must be in compliance with the requirement to be unique&nbsp;by September 1, 2018. Otherwise, Workfront will change your noncompliant usernames to meet the requirement, and your users might lose the ability to log in.

### Will I have to reset users' passwords after UUM migration?

Once migrated to Workfront UUM, all users within a Workfront instance, including non-SSO users, will be prompted to reset their Workfront password.

Currently, a system administrator can reset a user’s password without notifying that user. Once the Workfront UUM migration takes place, Workfront will remove this functionality in order to ensure the most secure user access experience.

You can still manually reset a user’s password, but instead of you providing a temporary password, Workfront will send the user an email that requests the user to reset their password.&nbsp;

>[!NOTE]
>
>You will not be able to retrieve a password for a Workfront user with an invalid email address.

### My users log in without specifying a domain. Will that change with UUM?

Currently, one of the ways a user can log in to Workfront is to specify the Workfront cluster to which the user is logging into, such as:

*cl01.my.workfront.com*

Once your organization migrates to Workfront UUM, Workfront will require the URL entered at login to specify the domain for which the user is logging in. For example,

*yourcompanydomain.*my.workfront.com.&nbsp;

### How does UUM affect my organization if we are already using single sign-on integrations?&nbsp;

Workfront currently supports SSO integrations with Active Directory, LDAP, and SAML 1.0 protocols.

After UUM migration Workfront will solely support SAML 2.0. If your SSO application is not SAML 2.0 compliant, you will need to upgrade your IDP.

If your organization currently uses SAML 2.0 for SSO, your users will not need to reset their passwords when you migrate to Workfront UUM. Instead, you will need to update your SSO settings to account for UUM. Contact Workfront Support for more details.

<!--
How will the migration take place?
-->

<!--
<add text here>
-->

<!--

-->

<!--

-->

<!--
Migration Plan for customers using SSO:
-->

<!--
<add text here>
-->

<!--

-->

<!--
Sandboxes and Other Workfront Instances
-->

<!--
<add text here>
-->

## Summary of UUM Functionality

| `Current Functionality`  | `Functionality After UUM`  | `System Admin Action`  |
|---|---|---|
| Users are required to have a unique username for each Workfront instance. |Users need only one unique username across all Workfront instances. |Ensure each user has a username that meets the new requirements.&nbsp; |
| Multiple users within the same Workfront instance can use the same email address (except for having varying combination of uppercase and lowercase letters). |Workfront no longer distinguishes between uppercase and lowercase letters. |Ensure each user has a unique email. If duplicating users within the same Workfront instance with one email address, try giving each user an email alias or a new, unique email address. |
| System admins can reset a user’s password and provide a temporary password. |System admin can reset a user’s password manually, but Workfront provides the user with a temporary password. |Once Workfront UUM is functional reset passwords for all users, include non-SSO users. |
| Users can log in to Workfront by specifying the cluster to which they want to log in. |Users must log in to Workfront by specifying the domain to which they want to log in. |Ensure user's login URL specifies the domain to which the user is logging in. |
| Workfront supports SSO integrations using Active Directory, LDAP, and SAML 1.0 protocols. |Work supports only SSO protocols that are SAML 2.0 compliant. |Ensure your IDP is SAML 2.0 compliant. |

&nbsp;
