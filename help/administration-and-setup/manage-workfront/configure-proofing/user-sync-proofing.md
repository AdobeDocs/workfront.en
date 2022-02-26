---
filename: user-sync-proofing
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: User synchronization between Adobe Workfront and Workfront Proof
description: User information is synchronized from Adobe Workfront to Workfront Proof; it is not synchronized from Workfront Proof to Workfront. Because of this, any time you create or modify users, you must make those changes within Workfront. You cannot make changes to users within Workfront Proof.
---

# User synchronization between *Adobe Workfront* and *Workfront Proof*

User information is&nbsp;synchronized from *Adobe Workfront* to *Workfront Proof*; it is not synchronized from *Workfront* Proof to *Workfront*. Because of this, any time you create or modify users, you must make those changes within *Workfront*. You cannot make changes to users within *Workfront Proof*.

The following sections provide information about user synchronization from *Workfront* to *Workfront Proof*:

## Information that is synchronized

*Workfront* synchronizes the following user information to *Workfront Proof*:

* Name (the user's first and last name)
* Email address

## When synchronization occurs

User information is synchronized from *Workfront* to *Workfront Proof* in the following circumstances:

* A&nbsp;user's information is updated in *Workfront*
* A&nbsp;user is created in *Workfront*

Depending on whether a user with the same email address exists in *Workfront Proof*, either of the following occurs:

<ul> 
 <li><span class="bold">If no user with a matching email exists in <em>Workfront Proof</em> and ... :</span>&nbsp; 
  <ul> 
   <li><span class="bold">Proofing is enabled for the user:</span> The user is created as a User in <em>Workfront Proof</em>.</li> 
   <li><span class="bold">Proofing is not enabled for the user:</span> The user is created as a Contact in <em>Workfront Proof</em>.</li> 
  </ul></li> 
 <li> <p><span class="bold">If a user with a matching email exists in <em>Workfront Proof</em>:</span> Proofing is enabled for that user in <em>Workfront</em> (if it was not already enabled) and information is&nbsp;synchronized between the two users.</p> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref" xrefformat="{para}">Configure a user's proofing access</a> in <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref" xrefformat="{para}">Configure a user's proofing access</a>.</p> <note type="important">
   When a user with a matching email exists, Workfront creates an alias email address based on the user email address that already exists in 
   <em>Workfront</em>. If your email provider does not support email aliases, this could impact proofing notifications. 
  </note> </li> 
</ul>

