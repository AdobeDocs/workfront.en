---
filename: error-message-saml-2-auth-failed-userid-not-found
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error message: SAML 2.0 Authentication Failed: User Identifier Not Found"
description: "I am receiving this error when using SAML 2.0: 'SAML 2.0 Authentication Failed: User Identifier Not Found.'"
---

# Error message: SAML 2.0 Authentication Failed: User Identifier Not Found

## Problem

I am receiving this error when using SAML 2.0: "SAML 2.0 Authentication Failed: User Identifier Not Found."

## Cause

This happens when a **UID** or **NAME ID** is not passed from the **ADFS Claim rules**.&nbsp;

In ADFS the **Relying Party Trust** needs to have a **Claim rule** that passes either a **UID** or a **NAME ID** value.&nbsp; When you run a **Workfront Test Connection**, it should show this if successful.&nbsp;

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

1. When editing the&nbsp;**ADFS INFO**, in the **Relying Party Trusts**> Select object >**Edit Claim Rules.**

1. The **LDAP Attribute** (left column) should have **E-Mail Addresses** (or any unique identifier).

1. The **Outgoing Claim Type** (right column) should be **Name ID**.

   >[!NOTE]
   >
   >It does not have to have the LDAP Attribute E-Mail Addresses. Any unique identifier that will identify the user can be used but it must be passed into Adobe Workfront as the **NAME ID**.

