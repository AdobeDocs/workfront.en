---
filename: user-sync-proofing
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: User synchronization between Adobe Workfront and Workfront Proof
description: User information is synchronized from Adobe Workfront to Workfront Proof; it is not synchronized from Workfront Proof to Workfront. Because of this, any time you create or modify users, you must make those changes within Workfront. You cannot make changes to users within Workfront Proof.
---

# User synchronization between Adobe Workfront and Workfront Proof

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

User information is&nbsp;synchronized from Adobe Workfront to Workfront Proof; it is not synchronized from Workfront Proof to Workfront. Because of this, any time you create or modify users, you must make those changes within Workfront. You cannot make changes to users within Workfront Proof.

The following sections provide information about user synchronization from Workfront to Workfront Proof:

## Information that is synchronized

Workfront synchronizes the following user information to Workfront Proof:

* Name (the user's first and last name)
* Email address

## When synchronization occurs

User information is synchronized from Workfront to Workfront Proof in the following circumstances:

* A&nbsp;user's information is updated in Workfront
* A&nbsp;user is created in Workfront

Depending on whether a user with the same email address exists in Workfront Proof, either of the following occurs:

* **If no user with a matching email exists in Workfront Proof and ... :**&nbsp;

   * **Proofing is enabled for the user:** The user is created as a User in Workfront Proof.
   * **Proofing is not enabled for the user:** The user is created as a Contact in Workfront Proof.

* **If a user with a matching email exists in Workfront Proof:** Proofing is enabled for that user in Workfront (if it was not already enabled) and information is&nbsp;synchronized between the two users.

  For more information, see [Configure a user's proofing access](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Configure a user's proofing access](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >When a user with a matching email exists, in their own or in another proofing environment, Workfront creates an alias email address by adding the user’s account id as a suffix to their email. For example, *username+accountid@domain.com*. If your email provider does not support email aliases, this could impact proofing notifications.

