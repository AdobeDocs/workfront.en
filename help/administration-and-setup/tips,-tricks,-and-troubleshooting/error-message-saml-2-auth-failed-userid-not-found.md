---
filename: error-message-saml-2-auth-failed-userid-not-found
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Error message: SAML 2.0 Authentication Failed: User Identifier Not Found {#error-message-saml-authentication-failed-user-identifier-not-found}



## Problem {#problem}

I am receiving this error when using SAML 2.0: "SAML 2.0 Authentication Failed: User Identifier Not Found."


## Cause {#cause}

This happens when a **UID** or **NAME ID** is not passed from the **ADFS Claim rules**.&nbsp;


In ADFS the **Relying Party Trust** needs to have a **Claim rule** that passes either a **UID** or a **NAME ID** value.  When you run a **`Workfront` Test Connection**, it should show this if successful.&nbsp;


## Solution {#solution}




1. When editing the&nbsp;****ADFS INFO****, in the **Relying Party Trusts**> Select object >** Edit Claim Rules.**

1. The **LDAP Attribute** (left column) should have **E-Mail Addresses** (or any unique identifier).

1. The **Outgoing Claim Type** (right column) should be **Name ID**.  


   >[!NOTE]
   >
   >It does not have to have the LDAP Attribute E-Mail Addresses. Any unique identifier that will identify the user can be used but it must be passed into `Workfront` as the **NAME ID**.





