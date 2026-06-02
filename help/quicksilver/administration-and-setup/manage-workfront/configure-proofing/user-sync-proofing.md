---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: User Synchronization Between Adobe Workfront and Workfront Proof
description: User information is synchronized from Adobe Workfront to Workfront Proof; it is not synchronized from Workfront Proof to Workfront. Because of this, anytime you create or modify users, you must make those changes within Workfront. You cannot make changes to users within Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
TQID: https://experienceleague.adobe.com/oHi8YTmAgh3KY1xfh6psNCLr4Gng0iniB3LUqbBzcOw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# User synchronization between Adobe Workfront and Workfront Proof

User information is synchronized from Adobe Workfront to Workfront Proof; it is not synchronized from Workfront Proof to Workfront. Because of this, anytime you create or modify users, you must make those changes within Workfront. You cannot make changes to users within Workfront Proof.

The following sections provide information about user synchronization from Workfront to Workfront Proof:

## Information that is synchronized

Workfront synchronizes the following user information to Workfront Proof:

* Name (the user's first and last name)
* Email address

## When synchronization occurs

User information is synchronized from Workfront to Workfront Proof in the following circumstances:

* A user's information is updated in Workfront
* A user is created in Workfront

Depending on whether a user with the same email address exists in Workfront Proof, either of the following occurs:

* **If no user with a matching email exists in Workfront Proof and** 

   * **Proofing is enabled for the user:** The user is created as a User in Workfront Proof.
   * **Proofing is not enabled for the user:** The user is created as a Contact in Workfront Proof.

* **If a user with a matching email exists in Workfront Proof:** Proofing is enabled for that user in Workfront (if it was not already enabled) and information is synchronized between the two users.

  For more information, see [Configure a user's proofing access](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Configure a user's proofing access](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >When a user with a matching email exists, in their own or in another proofing environment, Workfront creates an alias email address by adding the user's account id as a suffix to their email. For example, *username+accountid@domain.com*. Users will still receive proof notifications in the event an alias email is created.
