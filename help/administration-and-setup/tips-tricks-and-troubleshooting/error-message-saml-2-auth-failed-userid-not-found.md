---
filename: error-message-saml-2-auth-failed-userid-not-found
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Error message: SAML 2.0 Authentication Failed: User Identifier Not Found
description: I am receiving this error when using SAML 2.0: "SAML 2.0 Authentication Failed: User Identifier Not Found."
---

# Error message: SAML 2.0 Authentication Failed: User Identifier Not Found

## Problem

I am receiving this error when using SAML 2.0: "SAML 2.0 Authentication Failed: User Identifier Not Found."

## Cause

This happens when a `UID` or `NAME ID` is not passed from the `ADFS Claim rules`.&nbsp;

In ADFS the `Relying Party Trust` needs to have a `Claim rule` that passes either a `UID` or a `NAME ID` value.  When you run a ` `Workfront` Test Connection`, it should show this if successful.&nbsp;

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

<ol> 
 <li value="1">When editing the&nbsp;<span class="bold"><span class="bold">ADFS INFO</span></span>, in the <span class="bold">Relying Party Trusts</span>> Select object ><span class="bold"> Edit Claim Rules.</span></li> 
 <li value="2">The <span class="bold">LDAP Attribute</span> (left column) should have <span class="bold">E-Mail Addresses</span> (or any unique identifier).</li> 
 <li value="3">The <span class="bold">Outgoing Claim Type</span> (right column) should be <span class="bold">Name ID</span>.<br><note type="note">
    It does not have to have the LDAP Attribute E-Mail Addresses. Any unique identifier that will identify the user can be used but it must be passed into 
   <span>Adobe Workfront</span> as the 
   <span class="bold">NAME ID</span>.
  </note></li> 
</ol>

